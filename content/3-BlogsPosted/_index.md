---
title: "Blogs Posted"
date: 2026-11-24
weight: 3
chapter: false
pre: " <b> 3. </b> "
---

This section will list and introduce the blogs you have posted to [AWS Study Group](https://www.facebook.com/groups/awsstudygroupfcj). For example:

###  [Blog 1 - DOES SQS FIFO REALLY GUARANTEE “EXACTLY-ONCE PROCESSING”](3.1-Blog1/)
This blog introduces the newly added session policies feature in Amazon EKS Pod Identity, which allows you to narrow IAM permissions flexibly and precisely for each pod without needing to create multiple separate IAM roles. This is an important step forward that helps apply the principle of least privilege more effectively in large-scale Kubernetes environments.

###  [Blog 2 - HOW CAN A SMALL IAM PERMISSION CAUSE A BIG RISK](3.2-Blog2/)
AWS IAM (Identity and Access Management) lets administrators control user access to AWS services and resources. However, granting overly broad permissions, especially AdministratorAccess, can create serious security vulnerabilities if the account's credentials are leaked or the account is compromised. This post analyzes the risks when an IAM account with full administrative access to AWS is breached, and the solutions to reduce them.

###  [Blog 3 - AWS ACCESS KEY LEAKED ON GITHUB: AWS AUTOMATICALLY QUARANTINED IT, SO WHAT ELSE DO WE NEED TO DO](3.3-Blog3/)
When I first read about AWS Access Key exposure incidents, I assumed AWS already had automatic detection and handling, so the risk wasn't too worrying. After looking into it more closely, I realized that was only partly true: AWS can help detect and limit the damage, but that doesn't mean our account is safe. This post explains what AWS actually does when a key is exposed, the steps we still need to take, and how to prevent it.
