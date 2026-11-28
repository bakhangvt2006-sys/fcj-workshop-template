---
title: "Week 8 Worklog"
date: 2026-11-02
weight: 8
chapter: false
pre: " <b>1.8. </b>  "
---

### Week 8 Objectives:

* Review and consolidate the knowledge of the services learned in weeks 6 and 7: Lambda, API Gateway, SNS, SQS, and EventBridge.
* Strengthen weaker areas by practicing again and explaining concepts in my own words.
* Combine these services to build a complete event-driven architecture.

### Tasks to be carried out this week:

|Day|Task|Start Date|Completion Date|Reference Material|
|-|-|-|-|-|
|2|- Review **AWS Lambda** <br>&emsp; + Function, Runtime, Handler <br>&emsp; + Triggers and Execution role <br>&emsp; + Memory, Timeout, Environment variables, Cold start <br>&emsp; + View logs in CloudWatch <br> - Redo the lab on creating a Lambda function and an S3 trigger|02/11/2026|02/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|3|- Review **Amazon API Gateway** <br>&emsp; + REST API and HTTP API <br>&emsp; + Resources, Methods, Lambda proxy integration <br>&emsp; + Stages, Deployment, CORS, Throttling <br>&emsp; + Authorization options <br> - Redo the lab on creating GET and POST APIs connected to Lambda|03/11/2026|03/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|4|- Review **Amazon SNS** and **Amazon SQS** <br>&emsp; + SNS: Topics, Subscriptions, Fan-out, Message filtering <br>&emsp; + SQS: Standard and FIFO queues, Visibility timeout, Long polling <br>&emsp; + Dead-letter queue (DLQ) <br> - Redo the lab on SNS fan-out to SQS|04/11/2026|04/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|5|- Review **Amazon EventBridge** <br>&emsp; + Event bus, Rules, Event patterns, Targets <br>&emsp; + Scheduled runs with cron / rate <br> - Compare SNS, SQS, and EventBridge <br> - Compile summary notes for weeks 6 and 7|05/11/2026|05/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|6|- **Comprehensive hands-on:** build an event-driven architecture <br>&emsp; + API Gateway receives requests and calls Lambda <br>&emsp; + Lambda publishes a message to an SNS topic, which forwards it to an SQS queue (with a DLQ) <br>&emsp; + Another Lambda reads messages from SQS and stores them in DynamoDB <br>&emsp; + An EventBridge rule that runs on a schedule <br>&emsp; + Monitor logs in CloudWatch <br>&emsp; + Draw the architecture diagram and clean up resources to avoid unexpected costs|06/11/2026|06/11/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|


### Week 8 Achievements:

* Consolidated the knowledge of the services learned in weeks 6 and 7:
  * Lambda and API Gateway
  * SNS and SQS
  * EventBridge
* Strengthened weaker areas and redid the important labs.
* Clearly distinguished the role of each service:
  * Lambda: runs code in response to events without managing servers
  * API Gateway: the entry point that receives external requests and passes them to Lambda
  * SNS: sends one notification to many recipients at once
  * SQS: a queue that stores messages for asynchronous processing and prevents data loss
  * EventBridge: routes events based on rules and runs tasks on a schedule
* Successfully built an event-driven architecture combining multiple services and drew the corresponding architecture diagram.
* Built the habit of cleaning up resources after practice to keep costs under control.
* ...
