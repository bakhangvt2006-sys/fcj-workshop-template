---
title: "Week 11 Worklog"
date: 2026-11-23
weight: 11
chapter: false
pre: " <b>1.11. </b>  "
---

### Week 11 Objectives:

* Review and consolidate the knowledge of the services learned in weeks 9 and 10: ELB, Auto Scaling, KMS, Secrets Manager, Bedrock, SES, and WAF.
* Strengthen weaker areas by redoing the simple hands-on labs.
* Combine a few services to build a small architecture and draw its diagram.

### Tasks to be carried out this week:

|Day|Task|Start Date|Completion Date|Reference Material|
|-|-|-|-|-|
|2|- Review **ELB** and **Auto Scaling** <br>&emsp; + ALB, NLB, Listeners, Target groups, Health checks <br>&emsp; + Launch template, Auto Scaling group, Scaling policies <br> - Redo the lab on an ALB with an Auto Scaling group|23/11/2026|23/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|3|- Review **KMS** and **Secrets Manager** <br>&emsp; + KMS keys and encrypting data on S3 <br>&emsp; + Storing and retrieving secrets <br> - Redo the lab on encrypting an S3 bucket and creating a secret|24/11/2026|24/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|4|- Review **Amazon Bedrock** and **Amazon SES** <br>&emsp; + Bedrock: foundation models, IAM permissions, pricing <br>&emsp; + SES: identity verification, sandbox, sending emails <br> - Redo the lab on trying a model and sending an email|25/11/2026|25/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|5|- Review **AWS WAF** <br>&emsp; + Web ACL, Managed rules, Rate-based rules <br> - Compare the roles of the security services (IAM, KMS, Secrets Manager, WAF) <br> - Compile summary notes for weeks 9 and 10|26/11/2026|26/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|6|- **Comprehensive hands-on (simple):** <br>&emsp; + Create an ALB in front of the EC2 instances of an Auto Scaling group <br>&emsp; + Associate WAF with the ALB <br>&emsp; + Create a secret in Secrets Manager <br>&emsp; + Draw the architecture diagram <br>&emsp; + Clean up resources to avoid unexpected costs|27/11/2026|27/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|


### Week 11 Achievements:

* Consolidated the knowledge of the services learned in weeks 9 and 10:
  * ELB and Auto Scaling
  * KMS and Secrets Manager
  * Bedrock and SES
  * WAF
* Strengthened weaker areas and redid the hands-on labs.
* Clearly distinguished the role of each service:
  * ELB: distributes requests across multiple servers
  * Auto Scaling: automatically adjusts the number of EC2 instances to match demand
  * KMS and Secrets Manager: encrypt data and store sensitive information securely
  * Bedrock: use foundation models through an API
  * SES: send emails from applications
  * WAF: filters malicious requests before they reach the application
* Successfully built a small architecture with an ALB, an Auto Scaling group, and WAF, and drew the corresponding architecture diagram.
* Built the habit of cleaning up resources after practice to keep costs under control.

