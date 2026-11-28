---
title: "Week 9 Worklog"
date: 2026-11-09
weight: 9
chapter: false
pre: " <b>1.9. </b>  "
---

### Week 9 Objectives:

* Gain foundational knowledge of Elastic Load Balancing (ELB) and EC2 Auto Scaling.
* Gain foundational knowledge of AWS KMS and AWS Secrets Manager.
* Complete simple hands-on labs to get familiar with each service.

### Tasks to be carried out this week:

|Day|Task|Start Date|Completion Date|Reference Material|
|-|-|-|-|-|
|2|- Learn about **Elastic Load Balancing (ELB)** <br>&emsp; + Application Load Balancer (ALB) and Network Load Balancer (NLB) <br>&emsp; + Listeners and Target groups <br>&emsp; + Health checks|09/11/2026|09/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|3|- Learn about **EC2 Auto Scaling** <br>&emsp; + Launch template <br>&emsp; + Auto Scaling group (min, desired, max) <br>&emsp; + Scaling policies <br>&emsp; + Integration with ELB|10/11/2026|10/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|4|- Learn about **AWS KMS** and **AWS Secrets Manager** <br>&emsp; + KMS: encryption keys (AWS managed key, customer managed key) <br>&emsp; + Encrypting data on S3, EBS, RDS <br>&emsp; + Secrets Manager: storing and retrieving passwords and API keys|11/11/2026|11/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|5|- **ELB and Auto Scaling hands-on (simple):** <br>&emsp; + Create a Launch template for an EC2 web server <br>&emsp; + Create an Auto Scaling group with 2 instances <br>&emsp; + Create an Application Load Balancer and a Target group <br>&emsp; + Open the ALB DNS name to check the web page|12/11/2026|12/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|6|- **KMS and Secrets Manager hands-on (simple):** <br>&emsp; + Create a KMS key <br>&emsp; + Enable KMS encryption for an S3 bucket and upload a test file <br>&emsp; + Create a secret in Secrets Manager and view its value <br>&emsp; + Clean up resources to avoid unexpected costs|13/11/2026|13/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|


### Week 9 Achievements:

* Understood the basic concepts of Elastic Load Balancing:
  * Load balancer types (ALB, NLB)
  * Listeners, Target groups, and Health checks
* Understood the basic concepts of EC2 Auto Scaling:
  * Launch template and Auto Scaling group
  * Scaling policies and integration with ELB
* Understood the basic concepts of AWS KMS and Secrets Manager:
  * KMS keys and encrypting data across AWS services
  * Storing and retrieving secrets securely instead of hard-coding them
* Successfully completed the following hands-on tasks:
  * Built an ALB that distributes requests to EC2 instances managed by an Auto Scaling group
  * Encrypted an S3 bucket with a KMS key
  * Created and viewed a secret in Secrets Manager
* Built the habit of cleaning up resources after practice to keep costs under control.

