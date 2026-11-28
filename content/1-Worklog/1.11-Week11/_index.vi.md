---
title: "Worklog Tuần 11"
date: 2026-11-23
weight: 11
chapter: false
pre: " <b>1.11. </b>  "
---

### Mục tiêu tuần 11:

* Ôn tập và hệ thống lại kiến thức các dịch vụ đã học ở tuần 9 và tuần 10: ELB, Auto Scaling, KMS, Secrets Manager, Bedrock, SES và WAF.
* Củng cố những phần còn chưa chắc bằng cách làm lại các bài thực hành đơn giản.
* Kết hợp một số dịch vụ để dựng một kiến trúc nhỏ và vẽ sơ đồ.

### Các công việc cần triển khai trong tuần này:

|Thứ|Công việc|Ngày bắt đầu|Ngày hoàn thành|Nguồn tài liệu|
|-|-|-|-|-|
|2|- Ôn tập **ELB** và **Auto Scaling** <br>&emsp; + ALB, NLB, Listener, Target group, Health check <br>&emsp; + Launch template, Auto Scaling group, Scaling policy <br> - Làm lại bài thực hành ALB kết hợp Auto Scaling group|23/11/2026|23/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|3|- Ôn tập **KMS** và **Secrets Manager** <br>&emsp; + KMS key và mã hóa dữ liệu trên S3 <br>&emsp; + Lưu và lấy secret <br> - Làm lại bài thực hành mã hóa S3 bucket và tạo secret|24/11/2026|24/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|4|- Ôn tập **Amazon Bedrock** và **Amazon SES** <br>&emsp; + Bedrock: foundation model, quyền IAM, cách tính phí <br>&emsp; + SES: xác minh danh tính, sandbox, gửi email <br> - Làm lại bài thực hành thử model và gửi email|25/11/2026|25/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|5|- Ôn tập **AWS WAF** <br>&emsp; + Web ACL, Managed rule, Rate-based rule <br> - So sánh vai trò các dịch vụ bảo mật (IAM, KMS, Secrets Manager, WAF) <br> - Tổng hợp ghi chú tóm tắt kiến thức tuần 9 và tuần 10|26/11/2026|26/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|6|- **Thực hành tổng hợp (đơn giản):** <br>&emsp; + Tạo ALB đặt trước các EC2 của Auto Scaling group <br>&emsp; + Gắn WAF vào ALB <br>&emsp; + Tạo một secret trong Secrets Manager <br>&emsp; + Vẽ sơ đồ kiến trúc <br>&emsp; + Dọn dẹp tài nguyên để tránh phát sinh chi phí|27/11/2026|27/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|


### Kết quả đạt được tuần 11:

* Hệ thống hóa được kiến thức các dịch vụ đã học ở tuần 9 và tuần 10:
  * ELB và Auto Scaling
  * KMS và Secrets Manager
  * Bedrock và SES
  * WAF
* Củng cố được những phần còn chưa chắc và làm lại các bài thực hành.
* Phân biệt được vai trò của từng dịch vụ:
  * ELB: phân phối request đến nhiều máy chủ
  * Auto Scaling: tự động tăng giảm số lượng EC2 theo nhu cầu
  * KMS và Secrets Manager: mã hóa dữ liệu và lưu thông tin nhạy cảm an toàn
  * Bedrock: dùng các foundation model qua API
  * SES: gửi email từ ứng dụng
  * WAF: lọc request độc hại trước khi vào ứng dụng
* Đã dựng thành công một kiến trúc nhỏ gồm ALB, Auto Scaling group và WAF, và vẽ được sơ đồ kiến trúc tương ứng.
* Có thói quen dọn dẹp tài nguyên sau khi thực hành để kiểm soát chi phí.

