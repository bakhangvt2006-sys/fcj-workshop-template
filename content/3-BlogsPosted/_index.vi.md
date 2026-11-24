---
title: "Các bài blogs đã đăng"
date: 2026-11-24
weight: 3
chapter: false
pre: " <b> 3. </b> "
---

Tại đây sẽ là phần liệt kê, giới thiệu các blogs mà các bạn đã đăng trên [AWS Study Group](https://www.facebook.com/groups/awsstudygroupfcj).

###  [Blog 1 - SQS FIFO CÓ THỰC SỰ ĐẢM BẢO “EXACTLY-ONCE PROCESSING”](3.1-Blog1/)
AWS Lambda xử lý message từ Amazon SQS FIFO và ghi dữ liệu vào DynamoDB thành công, nhưng ngay trước khi xóa message khỏi SQS thì hàm bị timeout. Sau đó, cùng message được nhận lại. Nếu đã dùng FIFO queue, vì sao việc xử lý lại vẫn có thể xảy ra? Bài viết làm rõ sự khác biệt giữa chống gửi trùng, bảo toàn thứ tự và chống tác động nghiệp vụ trùng lặp, dựa trên AWS Documentation.

###  [Blog 2 - MỘT QUYỀN IAM NHỎ CÓ THỂ GÂY RA RỦI RO LỚN NHƯ THẾ NÀO](3.2-Blog2/)
AWS IAM (Identity and Access Management) cho phép quản trị viên kiểm soát quyền truy cập của người dùng đối với các dịch vụ và tài nguyên trên AWS. Tuy nhiên, việc cấp quyền quá rộng, đặc biệt là AdministratorAccess, có thể tạo ra lỗ hổng bảo mật nghiêm trọng nếu tài khoản bị lộ thông tin đăng nhập hoặc bị chiếm quyền kiểm soát. Bài viết phân tích những rủi ro khi một tài khoản IAM có quyền quản trị toàn bộ AWS bị xâm nhập và các giải pháp để hạn chế chúng.

###  [Blog 3 - AWS Access Key bị lộ trên GitHub: AWS đã tự động quarantine, vậy chúng ta còn phải làm gì?](3.3-Blog3/)
Trước đây, khi đọc về sự cố lộ AWS Access Key, mình từng nghĩ AWS đã có cơ chế tự động phát hiện và xử lý nên rủi ro không quá đáng lo. Nhưng khi tìm hiểu kỹ hơn, mình nhận ra suy nghĩ đó chỉ đúng một phần: AWS có thể giúp phát hiện và hạn chế thiệt hại, nhưng không có nghĩa tài khoản của chúng ta đã an toàn. Bài viết giải thích AWS thực sự làm gì khi key bị lộ, các bước cần làm tiếp theo và cách phòng ngừa.
