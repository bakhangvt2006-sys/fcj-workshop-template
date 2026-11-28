---
title: "Worklog Tuần 9"
date: 2026-11-09
weight: 9
chapter: false
pre: " <b>1.9. </b>  "
---

### Mục tiêu tuần 9:

* Nắm kiến thức cơ bản về Elastic Load Balancing (ELB) và EC2 Auto Scaling.
* Nắm kiến thức cơ bản về AWS KMS và AWS Secrets Manager.
* Thực hành các bài lab đơn giản để làm quen với từng dịch vụ.

### Các công việc cần triển khai trong tuần này:

|Thứ|Công việc|Ngày bắt đầu|Ngày hoàn thành|Nguồn tài liệu|
|-|-|-|-|-|
|2|- Tìm hiểu **Elastic Load Balancing (ELB)** <br>&emsp; + Application Load Balancer (ALB) và Network Load Balancer (NLB) <br>&emsp; + Listener và Target group <br>&emsp; + Health check|09/11/2026|09/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|3|- Tìm hiểu **EC2 Auto Scaling** <br>&emsp; + Launch template <br>&emsp; + Auto Scaling group (min, desired, max) <br>&emsp; + Scaling policy <br>&emsp; + Kết hợp với ELB|10/11/2026|10/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|4|- Tìm hiểu **AWS KMS** và **AWS Secrets Manager** <br>&emsp; + KMS: khóa mã hóa (AWS managed key, customer managed key) <br>&emsp; + Mã hóa dữ liệu trên S3, EBS, RDS <br>&emsp; + Secrets Manager: lưu và lấy mật khẩu, khóa API|11/11/2026|11/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|5|- **Thực hành ELB và Auto Scaling (đơn giản):** <br>&emsp; + Tạo Launch template cho EC2 chạy web server <br>&emsp; + Tạo Auto Scaling group với 2 instance <br>&emsp; + Tạo Application Load Balancer và Target group <br>&emsp; + Truy cập DNS của ALB để kiểm tra trang web|12/11/2026|12/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|6|- **Thực hành KMS và Secrets Manager (đơn giản):** <br>&emsp; + Tạo một KMS key <br>&emsp; + Bật mã hóa bằng KMS cho S3 bucket và upload thử một file <br>&emsp; + Tạo một secret trong Secrets Manager và xem lại giá trị <br>&emsp; + Dọn dẹp tài nguyên để tránh phát sinh chi phí|13/11/2026|13/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|


### Kết quả đạt được tuần 9:

* Hiểu được các khái niệm cơ bản của Elastic Load Balancing:
  * Các loại load balancer (ALB, NLB)
  * Listener, Target group và Health check
* Hiểu được các khái niệm cơ bản của EC2 Auto Scaling:
  * Launch template và Auto Scaling group
  * Scaling policy và cách kết hợp với ELB
* Hiểu được các khái niệm cơ bản của AWS KMS và Secrets Manager:
  * KMS key và việc mã hóa dữ liệu trên các dịch vụ AWS
  * Lưu trữ và truy xuất secret an toàn thay vì ghi trực tiếp trong code
* Đã thực hành thành công:
  * Dựng ALB phân phối request đến các EC2 do Auto Scaling group quản lý
  * Mã hóa S3 bucket bằng KMS key
  * Tạo và xem secret trong Secrets Manager
* Có thói quen dọn dẹp tài nguyên sau khi thực hành để kiểm soát chi phí.
* ...
