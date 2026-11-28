---
title: "Week 7 Worklog"
date: 2026-10-26
weight: 7
chapter: false
pre: " <b>1.7. </b>  "
---

### Week 7 Objectives:

* Gain a solid understanding of three services: Amazon SNS, Amazon SQS, and Amazon EventBridge.
* Understand the asynchronous communication model and how to decouple components in a system.
* Distinguish the roles of SNS, SQS, and EventBridge, and know when to use each.

### Tasks to be carried out this week:

|Day|Task|Start Date|Completion Date|Reference Material|
|-|-|-|-|-|
|2|- Learn about **Amazon SNS** <br>  + The publish / subscribe model <br>  + Topics, Publishers, and Subscribers <br>  + Subscription types (Email, SMS, HTTP, Lambda, SQS) <br>  + Fan-out and Message filtering <br>  + Standard and FIFO topics|26/10/2026|26/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|3|- Learn about **Amazon SQS** <br>  + Queues, Producers, and Consumers <br>  + Standard and FIFO queues <br>  + Visibility timeout and Message retention <br>  + Long polling and Delay queues <br>  + Dead-letter queue (DLQ)|27/10/2026|27/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|4|- Learn about **Amazon EventBridge** <br>  + Event bus (default and custom) <br>  + Rules and Event patterns <br>  + Targets <br>  + Scheduled runs with cron / rate <br> - Compare SNS, SQS, and EventBridge|28/10/2026|28/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|5|- **SNS and SQS hands-on:** <br>  + Create an SNS topic and subscribe an email address <br>  + Create an SQS queue and subscribe it to the SNS topic (fan-out) <br>  + Publish a message, then receive and delete it from the queue <br>  + Configure a dead-letter queue and test handling of failed messages|29/10/2026|29/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|6|- **EventBridge hands-on and combining services:** <br>  + Create a scheduled rule that triggers Lambda <br>  + Create a rule that catches EC2 state-change events and sends a notification through SNS <br>  + Let Lambda process messages from SQS <br>  + Monitor logs in CloudWatch <br>  + Clean up resources to avoid unexpected costs|30/10/2026|30/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|



### Week 7 Achievements:

* Understood the basic concepts of Amazon SNS:

  * The publish / subscribe model, Topics, and Subscriptions
  * Fan-out and Message filtering
  * Standard and FIFO topics
* Understood the basic concepts of Amazon SQS:

  * Queues, Producers, and Consumers
  * Standard and FIFO queues
  * Visibility timeout and Long polling
  * Dead-letter queue (DLQ)
* Understood the basic concepts of Amazon EventBridge:

  * Event bus, Rules, Event patterns, and Targets
  * Scheduled runs with cron / rate
* Learned to distinguish the role of each service:

  * SNS: sends one notification to many recipients at once
  * SQS: a queue that stores messages for asynchronous processing and prevents data loss
  * EventBridge: routes events based on rules and runs tasks on a schedule
* Successfully completed the following hands-on tasks:

  * Created an SNS topic, received email notifications, and subscribed an SQS queue to the topic
  * Sent, received, and deleted messages in SQS and configured a dead-letter queue
  * Created EventBridge rules that run Lambda on a schedule and send a notification when EC2 changes state
* Built the habit of cleaning up resources after practice to keep costs under control.


