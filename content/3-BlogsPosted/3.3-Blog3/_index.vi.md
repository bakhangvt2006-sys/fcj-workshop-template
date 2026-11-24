\---

title: "Blog 3"
date: 2026-11-23
weight: 2
chapter: false
pre: "  **3.2.**  "
---

# AWS ACCESS KEY BỊ LỘ TRÊN GITHUB: AWS ĐÃ TỰ ĐỘNG QUARANTINE, VẬY CHÚNG TA CÒN PHẢI LÀM GÌ?

Trước đây, khi đọc về sự cố lộ AWS Access Key, mình từng nghĩ AWS đã có cơ chế tự động phát hiện và xử lý nên rủi ro không quá đáng lo. Nhưng khi tìm hiểu kỹ hơn, mình nhận ra suy nghĩ đó chỉ đúng một phần: AWS có thể giúp phát hiện và hạn chế thiệt hại, nhưng không có nghĩa tài khoản của chúng ta đã an toàn. Bài viết giải thích AWS thực sự làm gì khi key bị lộ, các bước cần làm tiếp theo và cách phòng ngừa.

Các điểm chính cần nắm:

* AWS có cơ chế phát hiện credential bị công khai trên các nguồn như GitHub. Khi phát hiện, AWS có thể áp dụng quarantine policy (**AWSCompromisedKeyQuarantineV3** hoặc **V4**) cho IAM identity liên quan và gửi thông báo qua AWS Health hoặc Support Case.
* Trong một thử nghiệm của Unit 42, AWS gắn policy V3 chỉ khoảng 10 giây sau khi key bị công khai. Đây là kết quả của một thử nghiệm cụ thể, không phải thời gian phản ứng được đảm bảo trong mọi trường hợp.
* Quarantine policy **không** vô hiệu hóa access key. Nó chỉ bổ sung quyền Deny cho một số hành động cụ thể, còn các hành động khác vẫn phụ thuộc vào quyền IAM của identity đó.
* **Bước 1 – Cô lập credential:** xác định IAM user sở hữu key, đánh giá phạm vi quyền và chuyển key sang trạng thái Inactive. Chưa nên xóa key ngay để tiện đối chiếu.
* **Bước 2 – Khôi phục quyền truy cập hợp lệ:** xác định workload đang dùng key cũ, cập nhật credential hợp lệ và cân nhắc chuyển sang IAM Role dùng temporary credentials.
* **Bước 3 – Điều tra bằng CloudTrail:** xem API nào được gọi, thời điểm, IP nguồn, Region và các thay đổi bất thường về IAM. Cần dùng một principal quản trị độc lập để điều tra. Event History chủ yếu có management events, còn data events (như truy cập object S3) phải được cấu hình ghi log từ trước.
* **Bước 4 – Kiểm tra dấu hiệu xâm nhập trên toàn tài khoản:** IAM users/roles/policies mới hoặc bị thay đổi, EC2/Lambda lạ, S3 bị truy cập trái phép, Region ít dùng và chi phí Billing bất thường.
* **Bước 5 – Hoàn tất khắc phục:** không tự ý gỡ quarantine policy chỉ vì ứng dụng chạy lại; làm theo hướng dẫn trong AWS Support Case.
* **Phòng ngừa:** dùng IAM Role cho workload, IAM Identity Center/Federation cho người dùng, GitHub Actions OIDC thay cho access key dài hạn, bật GitHub Secret Scanning \& Push Protection và dùng pre-commit hook như git-secrets.
* Xóa secret khỏi file hoặc commit **không** có nghĩa credential đã an toàn. Nếu đã công khai, phải coi như nó có thể đã bị sao chép và xử lý theo quy trình ứng phó sự cố.

Điều mình rút ra: không có cơ chế tự động nào thay thế được việc quản lý danh tính, quyền truy cập và credential đúng cách. Trong môi trường Cloud, bảo mật không chỉ là ngăn truy cập trái phép mà còn phải biết phát hiện, điều tra, cô lập và khôi phục khi sự cố xảy ra.

Mọi người đang quản lý AWS credentials cho project cá nhân hoặc project nhóm như thế nào? Đặc biệt với GitHub Actions, mọi người dùng OIDC hay vẫn lưu access key trong GitHub Secrets? Mình muốn tham khảo thêm kinh nghiệm thực tế.

### 

https://www.facebook.com/share/p/1EAiomrDcV/

