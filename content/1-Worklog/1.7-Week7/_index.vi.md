---
title: "Worklog Tuần 7"
date: 2026-10-26
weight: 7
chapter: false
pre: " <b>1.7. </b>  "
---

### Mục tiêu tuần 7:

* Nắm vững kiến thức cơ bản về 3 dịch vụ: Amazon SNS, Amazon SQS và Amazon EventBridge.
* Hiểu mô hình giao tiếp bất đồng bộ và cách tách rời (decouple) các thành phần trong hệ thống.
* Phân biệt được vai trò của SNS, SQS và EventBridge, biết khi nào nên dùng dịch vụ nào.

### Các công việc cần triển khai trong tuần này:

|Thứ|Công việc|Ngày bắt đầu|Ngày hoàn thành|Nguồn tài liệu|
|-|-|-|-|-|
|2|- Tìm hiểu **Amazon SNS** <br>  + Mô hình publish / subscribe <br>  + Topic, Publisher và Subscriber <br>  + Các loại subscription (Email, SMS, HTTP, Lambda, SQS) <br>  + Fan-out và Message filtering <br>  + Standard và FIFO topic|26/10/2026|26/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|3|- Tìm hiểu **Amazon SQS** <br>  + Queue, Producer và Consumer <br>  + Standard và FIFO queue <br>  + Visibility timeout và Message retention <br>  + Long polling và Delay queue <br>  + Dead-letter queue (DLQ)|27/10/2026|27/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|4|- Tìm hiểu **Amazon EventBridge** <br>  + Event bus (default và custom) <br>  + Rule và Event pattern <br>  + Target <br>  + Lịch chạy theo cron / rate <br> - So sánh SNS, SQS và EventBridge|28/10/2026|28/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|5|- **Thực hành SNS và SQS:** <br>  + Tạo SNS topic và đăng ký nhận email <br>  + Tạo SQS queue và đăng ký vào SNS topic (fan-out) <br>  + Publish message, nhận và xóa message trong queue <br>  + Cấu hình dead-letter queue và thử xử lý message lỗi|29/10/2026|29/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|6|- **Thực hành EventBridge và kết hợp các dịch vụ:** <br>  + Tạo rule chạy theo lịch để kích hoạt Lambda <br>  + Tạo rule bắt sự kiện thay đổi trạng thái EC2 và gửi thông báo qua SNS <br>  + Cho Lambda xử lý message từ SQS <br>  + Theo dõi log trên CloudWatch <br>  + Dọn dẹp tài nguyên để tránh phát sinh chi phí|30/10/2026|30/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|



### Kết quả đạt được tuần 7:

* Hiểu được các khái niệm cơ bản của Amazon SNS:

  * Mô hình publish / subscribe, Topic và Subscription
  * Fan-out và Message filtering
  * Standard và FIFO topic
* Hiểu được các khái niệm cơ bản của Amazon SQS:

  * Queue, Producer và Consumer
  * Standard và FIFO queue
  * Visibility timeout, Long polling
  * Dead-letter queue (DLQ)
* Hiểu được các khái niệm cơ bản của Amazon EventBridge:

  * Event bus, Rule, Event pattern và Target
  * Lịch chạy theo cron / rate
* Phân biệt được vai trò của từng dịch vụ:

  * SNS: gửi một thông báo đến nhiều nơi nhận cùng lúc
  * SQS: hàng đợi lưu message để xử lý bất đồng bộ, tránh mất dữ liệu
  * EventBridge: định tuyến sự kiện theo quy tắc và chạy theo lịch
* Đã thực hành thành công:

  * Tạo SNS topic, nhận thông báo qua email và đăng ký SQS vào topic
  * Gửi, nhận, xóa message trong SQS và cấu hình dead-letter queue
  * Tạo rule EventBridge chạy Lambda theo lịch và gửi thông báo khi EC2 đổi trạng thái
* Có thói quen dọn dẹp tài nguyên sau khi thực hành để kiểm soát chi phí.
* ...

