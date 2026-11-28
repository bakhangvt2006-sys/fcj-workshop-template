---
title: "Worklog Tuần 6"
date: 2026-10-19
weight: 6
chapter: false
pre: " <b>1.6. </b>  "
---

### Mục tiêu tuần 6:

* Nắm vững kiến thức cơ bản về AWS Lambda và Amazon API Gateway.
* Hiểu mô hình serverless và biết khi nào nên dùng Lambda thay cho EC2.
* Biết cách xây dựng một API đơn giản bằng cách kết hợp API Gateway, Lambda và DynamoDB.

### Các công việc cần triển khai trong tuần này:

|Thứ|Công việc|Ngày bắt đầu|Ngày hoàn thành|Nguồn tài liệu|
|-|-|-|-|-|
|2|- Tìm hiểu **AWS Lambda** <br>&emsp; + Mô hình serverless <br>&emsp; + Function, Runtime và Handler <br>&emsp; + Trigger và Execution role <br>&emsp; + Memory, Timeout và Environment variables <br>&emsp; + Cold start và cách tính phí|19/10/2026|19/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|3|- **Thực hành Lambda:** <br>&emsp; + Tạo function bằng Python <br>&emsp; + Chạy thử với test event <br>&emsp; + Dùng Environment variables <br>&emsp; + Xem log trên CloudWatch Logs <br>&emsp; + Tạo trigger: tự động chạy khi có file upload lên S3|20/10/2026|20/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|4|- Tìm hiểu **Amazon API Gateway** <br>&emsp; + REST API và HTTP API <br>&emsp; + Resource và Method <br>&emsp; + Lambda proxy integration <br>&emsp; + Stage và Deployment <br>&emsp; + CORS, Throttling và API key <br>&emsp; + Các cách xác thực (IAM, Lambda authorizer, ...)|21/10/2026|21/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|5|- **Thực hành API Gateway và Lambda:** <br>&emsp; + Tạo API với các method GET và POST <br>&emsp; + Kết nối với Lambda qua proxy integration <br>&emsp; + Bật CORS và deploy lên stage <br>&emsp; + Gọi thử API bằng Postman hoặc `curl`|22/10/2026|22/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|6|- **Thực hành kết hợp API Gateway, Lambda và DynamoDB:** <br>&emsp; + Tạo API đơn giản để thêm, đọc và xóa dữ liệu <br>&emsp; + Gán IAM role cho Lambda theo nguyên tắc least privilege <br>&emsp; + Theo dõi log và lỗi trên CloudWatch <br>&emsp; + Dọn dẹp tài nguyên để tránh phát sinh chi phí|23/10/2026|23/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|


### Kết quả đạt được tuần 6:

* Hiểu được các khái niệm cơ bản của AWS Lambda:
  * Mô hình serverless và các thành phần của một function
  * Trigger, Execution role
  * Memory, Timeout, Environment variables
  * Cold start và cách tính phí
* Hiểu được các khái niệm cơ bản của Amazon API Gateway:
  * REST API và HTTP API
  * Resource, Method và Lambda proxy integration
  * Stage, Deployment, CORS và Throttling
  * Các cách xác thực cơ bản
* Phân biệt được khi nào nên dùng Lambda (tác vụ ngắn, theo sự kiện, tải không đều) và khi nào nên dùng EC2.
* Đã thực hành thành công:
  * Tạo Lambda function, chạy thử và xem log trên CloudWatch
  * Tạo trigger từ S3 cho Lambda
  * Tạo API bằng API Gateway, kết nối với Lambda và gọi thử bằng Postman hoặc `curl`
  * Xây dựng API đơn giản kết hợp API Gateway, Lambda và DynamoDB
* Có thói quen dọn dẹp tài nguyên sau khi thực hành để kiểm soát chi phí.
* ...
