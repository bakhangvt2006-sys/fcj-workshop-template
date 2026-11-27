---

title: "Blog 1"
date: 2026-11-22
weight: 1
chapter: false
pre: "<b> 3.1. </b>   "
---

# SQS FIFO CÓ THỰC SỰ ĐẢM BẢO “EXACTLY-ONCE PROCESSING”?

Một tình huống thú vị khi tìm hiểu hệ thống bất đồng bộ trên AWS: ứng dụng nhận sự kiện “Đơn hàng #1042 đã được tạo”. AWS Lambda xử lý message từ Amazon SQS FIFO và ghi dữ liệu vào DynamoDB thành công, nhưng ngay trước khi xóa message khỏi SQS thì hàm bị timeout. Sau đó, cùng message được nhận lại. Nếu đã dùng FIFO queue, vì sao việc xử lý lại vẫn có thể xảy ra? Bài viết làm rõ sự khác biệt giữa chống gửi trùng, bảo toàn thứ tự và chống tác động nghiệp vụ trùng lặp, dựa trên AWS Documentation.

Các điểm chính cần nắm:

* **Standard Queue** có thông lượng rất cao, cung cấp at-least-once delivery nhưng message có thể được nhận nhiều lần hoặc không đúng thứ tự. **FIFO Queue** hỗ trợ thứ tự trong từng `MessageGroupId` và cơ chế message deduplication; các group khác nhau có thể được xử lý song song.
* “Exactly-once” của SQS FIFO là chống gửi trùng ở tầng messaging, **không** đồng nghĩa toàn bộ nghiệp vụ trong Lambda chỉ chạy đúng một lần.
* **Deduplication chỉ có cửa sổ 5 phút:** nếu producer gửi lại cùng `MessageDeduplicationId` trong 5 phút, SQS không đưa thêm bản sao vào queue. Gửi lại sau khoảng đó, message có thể được coi là message mới.
* Khi bật content-based deduplication, SQS tạo deduplication ID từ SHA-256 của **message body**, không bao gồm message attributes. Vì vậy thay đổi attributes không tạo ra message khác về mặt deduplication.
* **Lambda + SQS vẫn có thể xử lý trùng:** event source mapping có semantics at-least-once. Nếu xử lý lỗi hoặc timeout, message hiện lại sau visibility timeout và được nhận lại, dù dữ liệu đã được ghi thành công.
* **Idempotency** nghĩa là thực hiện cùng một yêu cầu nhiều lần vẫn cho kết quả nghiệp vụ như xử lý một lần. Ví dụ dùng DynamoDB `PutItem` với `ConditionExpression: attribute\\\_not\\\_exists(eventId)` để lần xử lý sau không ghi đè item đã có.
* Điều kiện `PutItem` chỉ ngăn ghi trùng cho item đó, không tạo ra exactly-once end-to-end. Nếu workflow còn gửi email, gọi payment API hoặc cập nhật nhiều hệ thống, cần thêm transaction/outbox, trạng thái xử lý hoặc idempotency của downstream API.
* **Retry và partial batch response:** mặc định khi một message trong batch lỗi, cả batch có thể được thử lại. Bật `ReportBatchItemFailures` để chỉ báo các message thất bại. Với FIFO, nên dừng sau lỗi đầu tiên và báo cả các message chưa xử lý để không phá vỡ thứ tự.
* **Dead-Letter Queue (DLQ):** cấu hình redrive policy với `maxReceiveCount` để chuyển message lỗi liên tục sang DLQ; FIFO source queue phải dùng FIFO DLQ. DLQ giúp cô lập và điều tra lỗi, nhưng có thể làm mất thứ tự nghiệp vụ tuyệt đối khi tái xử lý và không đảm bảo message tự được xử lý thành công.
* **4 câu hỏi khi thiết kế hệ thống async:**

  1. Sự kiện có bắt buộc đúng thứ tự trong từng nhóm không? Nếu có, `MessageGroupId` phải đại diện đúng luồng nghiệp vụ, ví dụ `orderId`.
  2. Nếu message xuất hiện lại sau 5 phút hoặc Lambda retry, logic có an toàn khi chạy lại không?
  3. Visibility timeout, batch failure handling và retry policy có phù hợp với thời gian xử lý thực tế không?
  4. Nếu message thất bại lâu dài, đội vận hành sẽ phát hiện, xử lý và redrive DLQ thế nào?

Kết luận: “exactly-once delivery/deduplication” ở tầng messaging khác với “exactly-once business effect” ở tầng ứng dụng. Muốn workflow đáng tin cậy, cần thiết kế cùng lúc FIFO semantics, visibility timeout, retry/DLQ, idempotency và kiểm soát side effects.


![Blog 1 screenshot](../../images/3-BlogsPosted/3.1-Blog1/blog1.png)

https://www.facebook.com/share/p/1BmMVcWPia/

