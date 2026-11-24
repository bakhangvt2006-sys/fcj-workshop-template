---
title: "Blog 2"
date: 2026-11-23
weight: 2
chapter: false
pre: " <b> 3.2. </b> "
---

# HOW CAN A SMALL IAM PERMISSION CAUSE A BIG RISK?

AWS IAM (Identity and Access Management) lets administrators control user access to AWS services and resources. However, granting overly broad permissions, especially **AdministratorAccess**, can create serious security vulnerabilities if the account's credentials are leaked or the account is compromised. This post analyzes the risks when an IAM account with full administrative access to AWS is breached, and the solutions to reduce them.

Key points to remember:

* AdministratorAccess is an AWS Managed Policy that allows almost every administrative action in an AWS account, so if it is compromised, an attacker can affect the entire system.
* **Amazon S3:** an attacker can download or delete data, or change bucket access permissions → leakage of customer information and internal data.
* **Amazon EC2:** an attacker can launch unauthorized instances for cryptocurrency mining (Cryptojacking) or delete running servers → higher costs and service disruption.
* **Amazon RDS:** an attacker can delete databases, delete snapshots, or change security settings → data loss and impact on applications.
* **AWS IAM:** an attacker can create new users/roles, attach administrator policies, and create Access Keys to maintain access → incident response becomes more complicated.
* **AWS CloudTrail:** an attacker can stop or change logging configuration → loss of monitoring and investigation capability if logs are not protected independently.
* **Least Privilege:** grant only the permissions that are truly needed, and avoid AdministratorAccess when administration is not required.
* **MFA:** enable multi-factor authentication for important accounts to protect them when passwords are leaked.
* **IAM Roles and Temporary Credentials:** prefer temporary credentials over storing long-term Access Keys in applications.
* **Permission Boundaries:** set the maximum permissions that an IAM User or Role can receive.
* **CloudTrail Monitoring:** monitor API activity, especially changes related to IAM and security configuration.
* **Regular Access Review:** regularly review and revoke permissions that are no longer needed, and detect overly broad policies.

This post is especially useful for anyone operating systems on AWS who wants to tighten permission management, because a small but overly broad IAM permission can lead to major consequences.
<img width="800" height="500" alt="IAM drawio (3)" src="https://github.com/user-attachments/assets/edce8fff-1754-4385-8d3a-aed6b423735b" />

https://www.facebook.com/share/p/1JTkReQuuU/
