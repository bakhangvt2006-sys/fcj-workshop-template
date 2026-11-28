---
title: "Worklog Tuần 4"
date: 2026-10-05
weight: 4
chapter: false
pre: " <b>1.4. </b>  "
---

### Mục tiêu tuần 4:

* Nắm vững kiến thức cơ bản về 3 dịch vụ: Amazon CloudFront, Amazon CloudWatch và AWS CloudTrail.
* Biết cách phân phối nội dung nhanh và an toàn thông qua mạng lưới edge location.
* Biết cách giám sát tài nguyên, đặt cảnh báo và theo dõi lịch sử thao tác trên tài khoản AWS.

### Các công việc cần triển khai trong tuần này:

|Thứ|Công việc|Ngày bắt đầu|Ngày hoàn thành|Nguồn tài liệu|
|-|-|-|-|-|
|2|- Tìm hiểu **Amazon CloudFront** <br>&emsp; + Distribution và Edge location <br>&emsp; + Origin (S3, Load Balancer, ...) <br>&emsp; + Cache behavior và TTL <br>&emsp; + Invalidation <br>&emsp; + Origin Access Control (OAC) và HTTPS|05/10/2026|05/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|3|- Tìm hiểu **Amazon CloudWatch** <br>&emsp; + Metrics <br>&emsp; + Logs (Log group, Log stream) <br>&emsp; + Alarms <br>&emsp; + Dashboards <br>&emsp; + CloudWatch Agent|06/10/2026|06/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|4|- Tìm hiểu **AWS CloudTrail** <br>&emsp; + Event history <br>&emsp; + Management events và Data events <br>&emsp; + Trail và lưu log vào S3 <br>&emsp; + Phân biệt CloudTrail và CloudWatch|07/10/2026|07/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|5|- **Thực hành CloudFront:** <br>&emsp; + Tạo S3 bucket chứa website tĩnh <br>&emsp; + Tạo CloudFront distribution với origin là S3 <br>&emsp; + Cấu hình OAC để chặn truy cập trực tiếp vào bucket <br>&emsp; + Kiểm tra cache hit / miss và thực hiện invalidation|08/10/2026|08/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|6|- **Thực hành kết hợp CloudWatch và CloudTrail:** <br>&emsp; + Tạo CloudWatch alarm theo dõi CPU của EC2 và gửi email qua SNS <br>&emsp; + Tạo dashboard hiển thị các chỉ số chính <br>&emsp; + Xem Event history và tìm thao tác của một IAM user <br>&emsp; + Tạo trail lưu log vào S3 <br>&emsp; + Dọn dẹp tài nguyên để tránh phát sinh chi phí|09/10/2026|09/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|


### Kết quả đạt được tuần 4:

* Hiểu được các khái niệm cơ bản của Amazon CloudFront:
  * Distribution, Edge location và Origin
  * Cache behavior, TTL và Invalidation
  * Origin Access Control (OAC) và HTTPS
* Hiểu được các khái niệm cơ bản của Amazon CloudWatch:
  * Metrics, Logs, Alarms và Dashboards
  * CloudWatch Agent
* Hiểu được các khái niệm cơ bản của AWS CloudTrail:
  * Event history, Management events và Data events
  * Trail và lưu log vào S3
* Phân biệt được CloudWatch (giám sát hiệu năng, log và cảnh báo) với CloudTrail (ghi lại ai đã làm gì trên tài khoản).
* Đã thực hành thành công:
  * Phân phối website tĩnh từ S3 qua CloudFront, chặn truy cập trực tiếp vào bucket bằng OAC
  * Tạo alarm CPU cho EC2 và nhận cảnh báo qua email
  * Tạo dashboard, tra cứu Event history và tạo trail
* Có thói quen dọn dẹp tài nguyên sau khi thực hành để kiểm soát chi phí.

