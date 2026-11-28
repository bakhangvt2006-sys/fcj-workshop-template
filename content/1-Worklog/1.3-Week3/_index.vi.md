---
title: "Worklog Tuần 3"
date: 2026-09-28
weight: 3
chapter: false
pre: " <b>1.3. </b>  "
---

### Mục tiêu tuần 3:

* Nắm vững kiến thức cơ bản về 3 dịch vụ: Amazon RDS, Amazon DynamoDB và Amazon Route 53.
* Phân biệt được cơ sở dữ liệu quan hệ (RDS) và cơ sở dữ liệu NoSQL (DynamoDB), biết khi nào nên dùng loại nào.
* Thực hành tạo và quản lý cơ sở dữ liệu, cấu hình DNS và kết nối các dịch vụ với nhau.

### Các công việc cần triển khai trong tuần này:

|Thứ|Công việc|Ngày bắt đầu|Ngày hoàn thành|Nguồn tài liệu|
|-|-|-|-|-|
|2|- Tìm hiểu **Amazon RDS** <br>  + Các database engine (MySQL, PostgreSQL, ...) <br>  + Instance class và storage <br>  + DB subnet group và Security Group <br>  + Multi-AZ và Read Replica <br>  + Backup và Snapshot|28/09/2026|28/09/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|3|- Tìm hiểu **Amazon DynamoDB** <br>  + Table, Item, Attribute <br>  + Partition key và Sort key <br>  + Capacity mode (On-demand / Provisioned) <br>  + Secondary Index (GSI, LSI) <br>  + TTL <br> - **Thực hành:** <br>  + Tạo table <br>  + Thêm, sửa, xóa và truy vấn item<br />- Tham gia sự kiện|29/09/2026|29/09/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|4|- Tìm hiểu **Amazon Route 53** <br>  + Hosted zone <br>  + Các loại record (A, AAAA, CNAME, MX, Alias) <br>  + Routing policy (Simple, Weighted, Latency, Failover) <br>  + Health check|30/09/2026|30/09/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|5|- **Thực hành RDS:** <br>  + Tạo RDS instance trong private subnet <br>  + Kết nối từ EC2 vào database <br>  + Tạo snapshot và khôi phục <br>  + Tìm hiểu Multi-AZ và Read Replica trên Console|01/10/2026|01/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|6|- **Thực hành kết hợp DynamoDB và Route 53:** <br>  + Tạo Global Secondary Index cho DynamoDB table <br>  + So sánh Query và Scan <br>  + Tạo hosted zone và record trỏ về EC2 <br>  + Kiểm tra phân giải DNS bằng `nslookup` <br>  + Dọn dẹp tài nguyên để tránh phát sinh chi phí|02/10/2026|02/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|



### Kết quả đạt được tuần 3:

* Hiểu được các khái niệm cơ bản của Amazon RDS:

  * Database engine, instance class và storage
  * DB subnet group và Security Group
  * Multi-AZ, Read Replica
  * Backup và Snapshot
* Hiểu được các khái niệm cơ bản của Amazon DynamoDB:

  * Table, Item, Attribute
  * Partition key, Sort key
  * Capacity mode (On-demand / Provisioned)
  * Secondary Index và TTL
* Hiểu được các khái niệm cơ bản của Amazon Route 53:

  * Hosted zone và các loại record
  * Routing policy
  * Health check
* Phân biệt được khi nào dùng RDS (dữ liệu quan hệ, truy vấn phức tạp) và khi nào dùng DynamoDB (truy cập nhanh theo key, dễ mở rộng).
* Đã thực hành thành công:

  * Tạo RDS instance, kết nối từ EC2, tạo snapshot và khôi phục
  * Tạo DynamoDB table, thao tác với item và tạo Global Secondary Index
  * Tạo hosted zone, record DNS và kiểm tra phân giải
* Có thói quen dọn dẹp tài nguyên sau khi thực hành để kiểm soát chi phí.


