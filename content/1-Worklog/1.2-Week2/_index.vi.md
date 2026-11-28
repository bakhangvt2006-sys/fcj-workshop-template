---
title: "Worklog Tuần 2"
date: 2026-09-21
weight: 2
chapter: false
pre: " <b>1.2. </b>  "
---

### Mục tiêu tuần 2:

* Nắm vững kiến thức cơ bản về 3 dịch vụ nền tảng của AWS: IAM, S3 và EC2.
* Thực hành tạo và quản lý tài nguyên từng dịch vụ trên AWS Console và AWS CLI.
* Biết cách kết hợp IAM, S3 và EC2 để các dịch vụ truy cập nhau một cách an toàn.

### Các công việc cần triển khai trong tuần này:

|Thứ|Công việc|Ngày bắt đầu|Ngày hoàn thành|Nguồn tài liệu|
|-|-|-|-|-|
|2|- Tìm hiểu **IAM** <br>  + User, Group <br>  + Role <br>  + Policy (JSON) <br>  + Nguyên tắc least privilege <br>  + Root account và MFA|21/09/2026|21/09/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|3|- Tìm hiểu **Amazon S3** <br>  + Bucket và Object <br>  + Các lớp lưu trữ (Storage classes) <br>  + Versioning <br>  + Bucket policy và quyền truy cập <br> - **Thực hành:** <br>  + Tạo bucket <br>  + Upload, download và xóa object|22/09/2026|22/09/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|4|- Tìm hiểu **Amazon EC2** <br>  + Instance types <br>  + AMI <br>  + EBS volume <br>  + Security Group <br>  + Elastic IP <br> - **Thực hành:** <br>  + Tạo EC2 instance <br>  + Kết nối SSH <br>  + Gắn EBS volume|23/09/2026|23/09/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|5|- **Thực hành IAM:** <br>  + Tạo IAM user và group <br>  + Gán policy theo nguyên tắc least privilege <br>  + Bật MFA cho tài khoản <br>  + Tạo IAM role cho EC2|24/09/2026|24/09/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|6|- **Thực hành kết hợp IAM, S3 và EC2:** <br>  + Gắn IAM role vào EC2 instance <br>  + Từ EC2 truy cập S3 bằng AWS CLI (không dùng access key) <br>  + Kiểm tra quyền truy cập đúng và sai <br>  + Dọn dẹp tài nguyên để tránh phát sinh chi phí|25/09/2026|25/09/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|



### Kết quả đạt được tuần 2:

* Hiểu và phân biệt được các thành phần của IAM:

  * User, Group, Role
  * Policy và nguyên tắc least privilege
  * Root account và MFA
* Nắm được kiến thức cơ bản về Amazon S3:

  * Bucket, Object và các lớp lưu trữ
  * Versioning
  * Bucket policy và quyền truy cập
* Nắm được kiến thức cơ bản về Amazon EC2:

  * Instance types, AMI, EBS volume
  * Security Group và Elastic IP
* Đã thực hành thành công:

  * Tạo bucket S3, upload, download và xóa object
  * Tạo EC2 instance, kết nối SSH và gắn EBS volume
  * Tạo IAM user, group, policy, role và bật MFA
* Biết cách cấp quyền cho EC2 truy cập S3 thông qua IAM role thay vì dùng access key.
* Có thói quen dọn dẹp tài nguyên sau khi thực hành để kiểm soát chi phí.


