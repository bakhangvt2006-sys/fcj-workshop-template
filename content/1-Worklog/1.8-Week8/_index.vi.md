---
title: "Worklog Tuần 8"
date: 2026-11-02
weight: 8
chapter: false
pre: " <b>1.8. </b>  "
---

### Mục tiêu tuần 8:

* Ôn tập và hệ thống lại kiến thức các dịch vụ đã học ở tuần 6 và tuần 7: Lambda, API Gateway, SNS, SQS và EventBridge.
* Củng cố những phần còn chưa chắc bằng cách thực hành lại và tự giải thích bằng lời của mình.
* Kết hợp các dịch vụ để dựng một kiến trúc hướng sự kiện (event-driven) hoàn chỉnh.

### Các công việc cần triển khai trong tuần này:

|Thứ|Công việc|Ngày bắt đầu|Ngày hoàn thành|Nguồn tài liệu|
|-|-|-|-|-|
|2|- Ôn tập **AWS Lambda** <br>&emsp; + Function, Runtime, Handler <br>&emsp; + Trigger và Execution role <br>&emsp; + Memory, Timeout, Environment variables, Cold start <br>&emsp; + Xem log trên CloudWatch <br> - Làm lại bài thực hành tạo Lambda và trigger từ S3|02/11/2026|02/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|3|- Ôn tập **Amazon API Gateway** <br>&emsp; + REST API và HTTP API <br>&emsp; + Resource, Method, Lambda proxy integration <br>&emsp; + Stage, Deployment, CORS, Throttling <br>&emsp; + Các cách xác thực <br> - Làm lại bài thực hành tạo API GET và POST kết nối với Lambda|03/11/2026|03/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|4|- Ôn tập **Amazon SNS** và **Amazon SQS** <br>&emsp; + SNS: Topic, Subscription, Fan-out, Message filtering <br>&emsp; + SQS: Standard và FIFO queue, Visibility timeout, Long polling <br>&emsp; + Dead-letter queue (DLQ) <br> - Làm lại bài thực hành SNS fan-out đến SQS|04/11/2026|04/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|5|- Ôn tập **Amazon EventBridge** <br>&emsp; + Event bus, Rule, Event pattern, Target <br>&emsp; + Lịch chạy theo cron / rate <br> - So sánh SNS, SQS và EventBridge <br> - Tổng hợp ghi chú tóm tắt kiến thức tuần 6 và tuần 7|05/11/2026|05/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|6|- **Thực hành tổng hợp:** dựng kiến trúc hướng sự kiện <br>&emsp; + API Gateway nhận request và gọi Lambda <br>&emsp; + Lambda gửi message vào SNS topic, SNS chuyển đến SQS queue (có DLQ) <br>&emsp; + Một Lambda khác lấy message từ SQS và lưu vào DynamoDB <br>&emsp; + EventBridge rule chạy theo lịch <br>&emsp; + Theo dõi log trên CloudWatch <br>&emsp; + Vẽ sơ đồ kiến trúc và dọn dẹp tài nguyên để tránh phát sinh chi phí|06/11/2026|06/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|


### Kết quả đạt được tuần 8:

* Hệ thống hóa được kiến thức các dịch vụ đã học ở tuần 6 và tuần 7:
  * Lambda và API Gateway
  * SNS và SQS
  * EventBridge
* Củng cố được những phần còn chưa chắc và thực hành lại các bài lab quan trọng.
* Phân biệt rõ vai trò của từng dịch vụ:
  * Lambda: chạy code theo sự kiện, không cần quản lý máy chủ
  * API Gateway: cổng nhận request từ bên ngoài và chuyển đến Lambda
  * SNS: gửi một thông báo đến nhiều nơi nhận cùng lúc
  * SQS: hàng đợi lưu message để xử lý bất đồng bộ, tránh mất dữ liệu
  * EventBridge: định tuyến sự kiện theo quy tắc và chạy theo lịch
* Đã dựng thành công một kiến trúc hướng sự kiện kết hợp nhiều dịch vụ và vẽ được sơ đồ kiến trúc tương ứng.
* Có thói quen dọn dẹp tài nguyên sau khi thực hành để kiểm soát chi phí.

