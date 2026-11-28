---
title: "Week 4 Worklog"
date: 2026-10-05
weight: 4
chapter: false
pre: " <b>1.4. </b>  "
---

### Week 4 Objectives:

* Gain a solid understanding of three services: Amazon CloudFront, Amazon CloudWatch, and AWS CloudTrail.
* Learn how to deliver content quickly and securely through a network of edge locations.
* Learn how to monitor resources, set up alarms, and track the history of actions in an AWS account.

### Tasks to be carried out this week:

|Day|Task|Start Date|Completion Date|Reference Material|
|-|-|-|-|-|
|2|- Learn about **Amazon CloudFront** <br>&emsp; + Distribution and Edge locations <br>&emsp; + Origins (S3, Load Balancer, ...) <br>&emsp; + Cache behavior and TTL <br>&emsp; + Invalidation <br>&emsp; + Origin Access Control (OAC) and HTTPS|05/10/2026|05/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|3|- Learn about **Amazon CloudWatch** <br>&emsp; + Metrics <br>&emsp; + Logs (Log group, Log stream) <br>&emsp; + Alarms <br>&emsp; + Dashboards <br>&emsp; + CloudWatch Agent|06/10/2026|06/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|4|- Learn about **AWS CloudTrail** <br>&emsp; + Event history <br>&emsp; + Management events and Data events <br>&emsp; + Trails and storing logs in S3 <br>&emsp; + Differences between CloudTrail and CloudWatch|07/10/2026|07/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|5|- **CloudFront hands-on:** <br>&emsp; + Create an S3 bucket hosting a static website <br>&emsp; + Create a CloudFront distribution with S3 as the origin <br>&emsp; + Configure OAC to block direct access to the bucket <br>&emsp; + Check cache hits / misses and perform an invalidation|08/10/2026|08/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|6|- **Combined hands-on with CloudWatch and CloudTrail:** <br>&emsp; + Create a CloudWatch alarm monitoring EC2 CPU and send an email via SNS <br>&emsp; + Create a dashboard showing key metrics <br>&emsp; + View Event history and find the actions of an IAM user <br>&emsp; + Create a trail that stores logs in S3 <br>&emsp; + Clean up resources to avoid unexpected costs|09/10/2026|09/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|


### Week 4 Achievements:

* Understood the basic concepts of Amazon CloudFront:
  * Distribution, Edge locations, and Origins
  * Cache behavior, TTL, and Invalidation
  * Origin Access Control (OAC) and HTTPS
* Understood the basic concepts of Amazon CloudWatch:
  * Metrics, Logs, Alarms, and Dashboards
  * CloudWatch Agent
* Understood the basic concepts of AWS CloudTrail:
  * Event history, Management events, and Data events
  * Trails and storing logs in S3
* Learned to distinguish CloudWatch (monitoring performance, logs, and alerts) from CloudTrail (recording who did what in the account).
* Successfully completed the following hands-on tasks:
  * Delivered a static website from S3 through CloudFront, blocking direct bucket access with OAC
  * Created an EC2 CPU alarm and received alerts by email
  * Created a dashboard, looked up Event history, and created a trail
* Built the habit of cleaning up resources after practice to keep costs under control.

