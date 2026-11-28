---
title: "Worklog Tuần 5"
date: 2026-10-12
weight: 5
chapter: false
pre: " <b>1.5. </b>  "
---

### Mục tiêu tuần 5:

* Ôn tập và hệ thống lại kiến thức các dịch vụ AWS đã học trong 4 tuần đầu.
* Củng cố những phần còn chưa chắc bằng cách thực hành lại và tự giải thích bằng lời của mình.
* Kết hợp nhiều dịch vụ để dựng một kiến trúc nhỏ hoàn chỉnh trên AWS.

### Các công việc cần triển khai trong tuần này:

|Thứ|Công việc|Ngày bắt đầu|Ngày hoàn thành|Nguồn tài liệu|
|-|-|-|-|-|
|2|- Ôn tập nhóm **Networking \& Security** <br>  + VPC, CIDR block, Subnet (public / private) <br>  + Route table, Internet Gateway, NAT Gateway <br>  + Security Group và Network ACL <br>  + IAM: User, Group, Role, Policy, MFA|12/10/2026|12/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|3|- Ôn tập nhóm **Compute \& Storage** <br>  + Amazon EC2: Instance types, AMI, EBS, Elastic IP, kết nối SSH <br>  + Amazon S3: Bucket, Storage classes, Versioning, Bucket policy|13/10/2026|13/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|4|- Ôn tập nhóm **Database \& DNS** <br>  + Amazon RDS: Multi-AZ, Read Replica, Snapshot <br>  + Amazon DynamoDB: Partition key, Sort key, GSI, Capacity mode <br>  + Amazon Route 53: Hosted zone, Record, Routing policy|14/10/2026|14/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|5|- Ôn tập nhóm **Content Delivery \& Monitoring** <br>  + Amazon CloudFront: Distribution, Cache, OAC <br>  + Amazon CloudWatch: Metrics, Logs, Alarms <br>  + AWS CloudTrail: Event history, Trail <br> - Làm lại các bài thực hành chưa chắc ở những tuần trước|15/10/2026|15/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|6|- **Thực hành tổng hợp:** dựng kiến trúc nhỏ trên AWS <br>  + VPC có public subnet và private subnet <br>  + EC2 web server ở public subnet, RDS ở private subnet <br>  + IAM role cho EC2 truy cập S3 <br>  + S3 và CloudFront cho nội dung tĩnh <br>  + CloudWatch alarm và CloudTrail để giám sát <br>  + Vẽ sơ đồ kiến trúc và dọn dẹp tài nguyên để tránh phát sinh chi phí|16/10/2026|16/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|



### Kết quả đạt được tuần 5:

* Hệ thống hóa được kiến thức các dịch vụ đã học theo từng nhóm:

  * Networking \& Security: VPC, IAM
  * Compute \& Storage: EC2, S3
  * Database \& DNS: RDS, DynamoDB, Route 53
  * Content Delivery \& Monitoring: CloudFront, CloudWatch, CloudTrail
* Củng cố được những phần còn chưa chắc và thực hành lại các bài lab quan trọng.
* Hiểu được vai trò của từng dịch vụ và cách chúng kết nối với nhau trong một hệ thống:

  * Người dùng truy cập qua Route 53 và CloudFront
  * EC2 xử lý ứng dụng, lấy dữ liệu từ RDS, DynamoDB và S3
  * IAM kiểm soát quyền truy cập, CloudWatch và CloudTrail giám sát hệ thống
* Đã dựng thành công một kiến trúc nhỏ kết hợp nhiều dịch vụ và vẽ được sơ đồ kiến trúc tương ứng.
* Có thói quen dọn dẹp tài nguyên sau khi thực hành để kiểm soát chi phí.
* ...

