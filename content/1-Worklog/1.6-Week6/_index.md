---
title: "Week 6 Worklog"
date: 2026-10-19
weight: 6
chapter: false
pre: " <b>1.6. </b>  "
---

### Week 6 Objectives:

* Gain a solid understanding of AWS Lambda and Amazon API Gateway.
* Understand the serverless model and know when to use Lambda instead of EC2.
* Learn how to build a simple API by combining API Gateway, Lambda, and DynamoDB.

### Tasks to be carried out this week:

|Day|Task|Start Date|Completion Date|Reference Material|
|-|-|-|-|-|
|2|- Learn about **AWS Lambda** <br>&emsp; + The serverless model <br>&emsp; + Function, Runtime, and Handler <br>&emsp; + Triggers and Execution role <br>&emsp; + Memory, Timeout, and Environment variables <br>&emsp; + Cold start and pricing|19/10/2026|19/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|3|- **Lambda hands-on:** <br>&emsp; + Create a function in Python <br>&emsp; + Run it with a test event <br>&emsp; + Use Environment variables <br>&emsp; + View logs in CloudWatch Logs <br>&emsp; + Create a trigger: run automatically when a file is uploaded to S3|20/10/2026|20/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|4|- Learn about **Amazon API Gateway** <br>&emsp; + REST API and HTTP API <br>&emsp; + Resources and Methods <br>&emsp; + Lambda proxy integration <br>&emsp; + Stages and Deployment <br>&emsp; + CORS, Throttling, and API keys <br>&emsp; + Authorization options (IAM, Lambda authorizer, ...)|21/10/2026|21/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|5|- **API Gateway and Lambda hands-on:** <br>&emsp; + Create an API with GET and POST methods <br>&emsp; + Connect it to Lambda through proxy integration <br>&emsp; + Enable CORS and deploy to a stage <br>&emsp; + Test the API with Postman or `curl`|22/10/2026|22/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|6|- **Combined hands-on with API Gateway, Lambda, and DynamoDB:** <br>&emsp; + Build a simple API to add, read, and delete data <br>&emsp; + Assign an IAM role to Lambda following the principle of least privilege <br>&emsp; + Monitor logs and errors in CloudWatch <br>&emsp; + Clean up resources to avoid unexpected costs|23/10/2026|23/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|


### Week 6 Achievements:

* Understood the basic concepts of AWS Lambda:
  * The serverless model and the components of a function
  * Triggers and Execution role
  * Memory, Timeout, and Environment variables
  * Cold start and pricing
* Understood the basic concepts of Amazon API Gateway:
  * REST API and HTTP API
  * Resources, Methods, and Lambda proxy integration
  * Stages, Deployment, CORS, and Throttling
  * Basic authorization options
* Learned when to use Lambda (short tasks, event-driven workloads, uneven traffic) and when to use EC2.
* Successfully completed the following hands-on tasks:
  * Created a Lambda function, ran it, and viewed logs in CloudWatch
  * Created an S3 trigger for Lambda
  * Created an API with API Gateway, connected it to Lambda, and tested it with Postman or `curl`
  * Built a simple API combining API Gateway, Lambda, and DynamoDB
* Built the habit of cleaning up resources after practice to keep costs under control.
* ...
