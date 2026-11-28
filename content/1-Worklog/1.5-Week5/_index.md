---
title: "Week 5 Worklog"
date: 2026-10-12
weight: 5
chapter: false
pre: " <b>1.5. </b>  "
---

### Week 5 Objectives:

* Review and consolidate the knowledge of the AWS services learned during the first 4 weeks.
* Strengthen weaker areas by practicing again and explaining concepts in my own words.
* Combine multiple services to build a small, complete architecture on AWS.

### Tasks to be carried out this week:

|Day|Task|Start Date|Completion Date|Reference Material|
|-|-|-|-|-|
|2|- Review the **Networking & Security** group <br>&emsp; + VPC, CIDR block, Subnets (public / private) <br>&emsp; + Route table, Internet Gateway, NAT Gateway <br>&emsp; + Security Group and Network ACL <br>&emsp; + IAM: Users, Groups, Roles, Policies, MFA|12/10/2026|12/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|3|- Review the **Compute & Storage** group <br>&emsp; + Amazon EC2: Instance types, AMI, EBS, Elastic IP, SSH connection <br>&emsp; + Amazon S3: Buckets, Storage classes, Versioning, Bucket policy|13/10/2026|13/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|4|- Review the **Database & DNS** group <br>&emsp; + Amazon RDS: Multi-AZ, Read Replica, Snapshot <br>&emsp; + Amazon DynamoDB: Partition key, Sort key, GSI, Capacity mode <br>&emsp; + Amazon Route 53: Hosted zone, Records, Routing policies|14/10/2026|14/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|5|- Review the **Content Delivery & Monitoring** group <br>&emsp; + Amazon CloudFront: Distribution, Cache, OAC <br>&emsp; + Amazon CloudWatch: Metrics, Logs, Alarms <br>&emsp; + AWS CloudTrail: Event history, Trail <br> - Redo the labs from previous weeks that I was less confident about|15/10/2026|15/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|6|- **Comprehensive hands-on:** build a small architecture on AWS <br>&emsp; + A VPC with a public subnet and a private subnet <br>&emsp; + An EC2 web server in the public subnet and RDS in the private subnet <br>&emsp; + An IAM role for EC2 to access S3 <br>&emsp; + S3 and CloudFront for static content <br>&emsp; + CloudWatch alarms and CloudTrail for monitoring <br>&emsp; + Draw the architecture diagram and clean up resources to avoid unexpected costs|16/10/2026|16/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|


### Week 5 Achievements:

* Consolidated the knowledge of all learned services into groups:
  * Networking & Security: VPC, IAM
  * Compute & Storage: EC2, S3
  * Database & DNS: RDS, DynamoDB, Route 53
  * Content Delivery & Monitoring: CloudFront, CloudWatch, CloudTrail
* Strengthened weaker areas and redid the important labs.
* Understood the role of each service and how they connect within a system:
  * Users reach the application through Route 53 and CloudFront
  * EC2 runs the application and retrieves data from RDS, DynamoDB, and S3
  * IAM controls access, while CloudWatch and CloudTrail monitor the system
* Successfully built a small architecture combining multiple services and drew the corresponding architecture diagram.
* Built the habit of cleaning up resources after practice to keep costs under control.

