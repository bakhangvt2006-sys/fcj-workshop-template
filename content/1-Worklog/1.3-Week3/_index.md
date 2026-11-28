---
title: "Week 3 Worklog"
date: 2026-09-28
weight: 3
chapter: false
pre: " <b>1.3. </b>  "
---

### Week 3 Objectives:

* Gain a solid understanding of three services: Amazon RDS, Amazon DynamoDB, and Amazon Route 53.
* Distinguish between relational databases (RDS) and NoSQL databases (DynamoDB), and know when to use each.
* Practice creating and managing databases, configuring DNS, and connecting services together.

### Tasks to be carried out this week:

|Day|Task|Start Date|Completion Date|Reference Material|
|-|-|-|-|-|
|2|- Learn about **Amazon RDS** <br>  + Database engines (MySQL, PostgreSQL, ...) <br>  + Instance class and storage <br>  + DB subnet group and Security Group <br>  + Multi-AZ and Read Replica <br>  + Backup and Snapshot|28/09/2026|28/09/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|3|- Learn about **Amazon DynamoDB** <br>  + Table, Item, Attribute <br>  + Partition key and Sort key <br>  + Capacity mode (On-demand / Provisioned) <br>  + Secondary Index (GSI, LSI) <br>  + TTL <br> - **Hands-on:** <br>  + Create a table <br>  + Add, update, delete, and query items<br />- Attend event|29/09/2026|29/09/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|4|- Learn about **Amazon Route 53** <br>  + Hosted zone <br>  + Record types (A, AAAA, CNAME, MX, Alias) <br>  + Routing policies (Simple, Weighted, Latency, Failover) <br>  + Health check|30/09/2026|30/09/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|5|- **RDS hands-on:** <br>  + Create an RDS instance in a private subnet <br>  + Connect to the database from EC2 <br>  + Create a snapshot and restore it <br>  + Explore Multi-AZ and Read Replica in the Console|01/10/2026|01/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|
|6|- **Combined hands-on with DynamoDB and Route 53:** <br>  + Create a Global Secondary Index for a DynamoDB table <br>  + Compare Query and Scan <br>  + Create a hosted zone and a record pointing to EC2 <br>  + Verify DNS resolution with `nslookup` <br>  + Clean up resources to avoid unexpected costs|02/10/2026|02/10/2026|[https://cloudjourney.awsstudygroup.com/](https://cloudjourney.awsstudygroup.com/)|



### Week 3 Achievements:

* Understood the basic concepts of Amazon RDS:

  * Database engines, instance class, and storage
  * DB subnet group and Security Group
  * Multi-AZ and Read Replica
  * Backup and Snapshot
* Understood the basic concepts of Amazon DynamoDB:

  * Table, Item, Attribute
  * Partition key and Sort key
  * Capacity mode (On-demand / Provisioned)
  * Secondary Index and TTL
* Understood the basic concepts of Amazon Route 53:

  * Hosted zone and record types
  * Routing policies
  * Health check
* Learned when to use RDS (relational data, complex queries) and when to use DynamoDB (fast key-based access, easy scaling).
* Successfully completed the following hands-on tasks:

  * Created an RDS instance, connected from EC2, and created and restored a snapshot
  * Created a DynamoDB table, worked with items, and created a Global Secondary Index
  * Created a hosted zone and DNS records, and verified DNS resolution
* Built the habit of cleaning up resources after practice to keep costs under control.
* ...

