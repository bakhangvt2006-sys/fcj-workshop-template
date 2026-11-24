---

title: "Blog 2"
date: 2026-11-23
weight: 1
chapter: false
pre: "  **3.1.**  "
---

# MỘT QUYỀN IAM NHỎ CÓ THỂ GÂY RA RỦI RO LỚN NHƯ THẾ NÀO?

AWS IAM (Identity and Access Management) cho phép quản trị viên kiểm soát quyền truy cập của người dùng đối với các dịch vụ và tài nguyên trên AWS. Tuy nhiên, việc cấp quyền quá rộng, đặc biệt là **AdministratorAccess**, có thể tạo ra lỗ hổng bảo mật nghiêm trọng nếu tài khoản bị lộ thông tin đăng nhập hoặc bị chiếm quyền kiểm soát. Bài viết phân tích những rủi ro khi một tài khoản IAM có quyền quản trị toàn bộ AWS bị xâm nhập và các giải pháp để hạn chế chúng.

Các điểm chính cần nắm:

* AdministratorAccess là AWS Managed Policy cho phép thực hiện gần như toàn bộ thao tác quản trị trên tài khoản AWS, nên khi bị xâm nhập, kẻ tấn công có thể gây ảnh hưởng trên toàn hệ thống.
* **Amazon S3:** kẻ tấn công có thể tải xuống, xóa dữ liệu hoặc thay đổi quyền truy cập bucket → rò rỉ thông tin khách hàng và dữ liệu nội bộ.
* **Amazon EC2:** có thể khởi chạy instance trái phép để đào tiền mã hóa (Cryptojacking) hoặc xóa máy chủ đang chạy → chi phí tăng cao và hệ thống bị gián đoạn.
* **Amazon RDS:** có thể xóa database, xóa snapshot hoặc thay đổi thiết lập bảo mật → mất dữ liệu và ảnh hưởng ứng dụng.
* **AWS IAM:** có thể tạo user/role mới, gắn policy quản trị và tạo Access Keys để duy trì quyền truy cập → việc xử lý sự cố trở nên phức tạp hơn.
* **AWS CloudTrail:** có thể dừng hoặc thay đổi cấu hình ghi log → mất khả năng giám sát và điều tra nếu log không được bảo vệ độc lập.
* **Least Privilege:** chỉ cấp những quyền thực sự cần thiết, tránh dùng AdministratorAccess khi không có nhu cầu quản trị.
* **MFA:** bật xác thực đa yếu tố cho các tài khoản quan trọng để bảo vệ khi mật khẩu bị lộ.
* **IAM Roles và Temporary Credentials:** ưu tiên thông tin xác thực tạm thời thay vì lưu Access Keys dài hạn trong ứng dụng.
* **Permission Boundaries:** đặt giới hạn quyền tối đa mà IAM User hoặc Role có thể nhận được.
* **CloudTrail Monitoring:** theo dõi hoạt động API, đặc biệt là các thay đổi liên quan đến IAM và cấu hình bảo mật.
* **Regular Access Review:** thường xuyên kiểm tra, thu hồi quyền không còn cần thiết và phát hiện policy có phạm vi quá rộng.

Bài viết đặc biệt hữu ích cho những ai đang vận hành hệ thống trên AWS và muốn siết chặt việc cấp quyền, vì một quyền IAM nhỏ nhưng quá rộng cũng có thể dẫn đến hậu quả lớn.

### 
<img width="1322" height="651" alt="IAM drawio (3)" src="https://github.com/user-attachments/assets/510ba855-3880-4153-a4c5-7386a4a09008" />

https://www.facebook.com/share/p/1JTkReQuuU/

