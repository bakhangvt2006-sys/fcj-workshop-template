---

title: "Event 3"
date: 2026-10-24
weight: 3
chapter: false
pre: " <b> 4.3. </b>  "
---

# Event Summary Report: “First Cloud AI Journey: Weekly Meet Up”

* **Event name:** First Cloud AI Journey: Weekly Meet Up
* **Date \& time:** 09:00 – 12:00, Saturday, October 24, 2026
* **Venue:** 26th Floor, Bitexco Financial Tower, Ho Chi Minh City
* **Role:** Attendee

### Event Objectives

* Learn from real-world Cloud and AI Agent deployment experience shared directly by Tech Leads and enterprise engineers
* Explore practical perspectives on low-latency Vietnamese Voice AI, multi-account resource sharing, early security testing, and the platform for taking Agents to production
* Apply lessons on cost optimization, context/memory management, security guardrails, and running agents 24/7 to my own learning path
* Build confidence in networking, proactively connect with others, and put more effort into learning alongside the community

### Speakers

* **Mr. Kiệt Trần** – Revve AI
* **Mr. Long Huỳnh** – Styl Solution
* **Mr. Thịnh Nguyễn** – Styl Solution
* **Mr. Xuân An** – Leader, AWS Student Builder Group HCMUTE
* **Mr. Khoa Kiều** – Tech Lead, ACB
* **Mr. Nghi Danh** – AWS Community Builder

### Highlights

#### 1\. Hear, Think, Speak – Building a Vietnamese Voice-AI Call Center on AWS (Mr. Kiệt Trần – Revve AI)

* Explored the **Voice AI** architecture and the challenge of cutting response latency down to roughly **\~1.8s** so conversations flow smoothly
* The live demo featured an AI system placing a phone call to conduct a preliminary interview for a **Cloud Engineer** position in Vietnamese, which was impressive and natural

#### 2\. AWS Resource Access Manager (Mr. Long Huỳnh – Styl Solution)

* Showed how to share resources securely across accounts within an **AWS Organization**
* The solution helps save costs, centralize network management, and combine **IAM policy** with **SCP** so that no one can exceed their permission ceiling

#### 3\. AWS Pentest with AWS Continuum / Security Agent (Mr. Thịnh Nguyễn – Styl Solution)

* Introduced a suite for assessing infrastructure security early: reviewing **Terraform** code and integrating directly into **GitLab/GitHub PRs** to catch issues early
* Lets the **Security Agent** act as a real user to run automated pentests in **SIT/UAT** environments before real deployment

#### 4\. Amazon Bedrock AgentCore (Mr. Xuân An – Leader, AWS Student Builder Group HCMUTE)

* Gave a comprehensive view of two building blocks for taking Agents to production:

  * **Agent Runtime**: Runs **MicroVM** on **EC2 Spot** to save compute costs
  * **Memory**: Tiered into synchronous **Short-term** and asynchronous **Long-term** memory so the Agent understands user context in depth

#### 5\. Kiro Crew (Mr. Khoa Kiều – Tech Lead, ACB \& Mr. Nghi Danh – AWS Community Builder)

* My favorite session, covering how to let AI Agents run **24/7** to assist with code review and system checks, followed by an engaging technical Q\&A at the end:

  * **Artifacts**: Automatically scraping real job-market data and building visual statistical charts right inside the chat window
  * **Context Window Management**: The **Auto Compact** mechanism triggers when context reaches the **70–90%** threshold, and the **Break down context** feature lets you inspect token consumption by each component in detail
  * **Memory Management \& Guardrails**: Cleaning up old memories to prevent runaway costs, and setting up security guardrails so the AI cannot arbitrarily delete infrastructure or expose server secrets/credentials

### Key Takeaways

#### Multi-Account Management \& Early Security Assessment

* **Permission ceilings when sharing resources**: Combining **IAM policy** with **SCP** while sharing resources in an **AWS Organization** helps optimize costs, centralize network management, and keep permissions within the right limits
* **Catching infrastructure issues before real deployment**: Reviewing **Terraform** code on **GitLab/GitHub PRs** and running automated pentests with the **Security Agent** on **SIT/UAT** helps detect risks early

#### Running Agents in Production, Cost Control \& Security Guardrails

* **Runtime and tiered memory**: Taking Agents to production involves running **MicroVM** on **EC2 Spot** to optimize cost, combined with synchronous **Short-term** memory and asynchronous **Long-term** memory to preserve deep context
* **Controlling cost and preventing risk when running 24/7**: Managing the context window (**Auto Compact**, **Break down context**), cleaning up old memory, and setting guardrails help avoid cost bloat, accidental infrastructure deletion, or leaked secrets/credentials

### Applying to My Work

* **Combine IAM policy and SCP**: Apply the permission-ceiling mechanism when sharing resources across accounts in an **AWS Organization**
* **Embed security checks early**: Apply **Terraform** review on PRs and automated pentests on **SIT/UAT** before real deployment
* **Manage context, memory, and guardrails for Agents**: Control token usage, clean up old memory, and put protective guardrails around infrastructure, secrets, and credentials when working with AI Agents
* **Network with confidence and learn proactively**: Build confidence in communication, proactively connect with speakers and peers, and strive to learn more every day

### Event Experience

On the morning of Saturday, October 24, 2026, on the 26th floor of Bitexco Financial Tower, the event ran only from 9:00 – 12:00 AM yet left behind a great deal of practical knowledge and energy from listening to Tech Leads and engineers share about Cloud and AI Agents. The main experiences included:

#### Learning from Tech Leads and speakers

* The talks from **Revve AI**, **Styl Solution**, **AWS Student Builder Group HCMUTE**, **ACB**, and **AWS Community Builder** showed me how vast and exciting real-world knowledge can be.
* **Kiro Crew** was my favorite session, especially the technical Q\&A on creating **Artifacts**, **Auto Compact**, **Break down context**, cleaning up memory, and setting up **Guardrails** for Agents running **24/7**.

#### Exposure to hands-on practice and real architectures

* I was introduced to very concrete problems: reducing **Voice AI** latency to **\~1.8s** with a live demo of a Vietnamese preliminary **Cloud Engineer** interview, **AWS Resource Access Manager** combined with **IAM** and **SCP**, **Terraform** checks on PRs and automated pentests on **SIT/UAT**, and **Amazon Bedrock AgentCore** (**Agent Runtime** on **EC2 Spot** MicroVM and tiered **Memory**).

#### Connection and community spirit

* The open sharing atmosphere on the 26th floor of Bitexco gave me extra motivation on my Cloud and AI learning journey.
* After the meet-up, I saw even more clearly that I need to network with confidence, proactively connect, and put more effort into learning.

#### Lessons learned

* Real-world AI and Cloud systems require balancing processing capability (such as voice latency and deep context), operating cost, and safety guardrails.
* When letting an AI Agent run long-term or **24/7**, managing context/memory and setting guardrails to prevent infrastructure deletion or leaked secrets/credentials is key.
* Confidence in connecting, proactiveness, and persistence in learning will make my Cloud journey steadier and more motivating.

#### Some event photos

<img width="2560" height="1920" alt="image" src="https://github.com/user-attachments/assets/dbb2a9e7-e9d5-4f18-b6a8-cc3da658d7bf" />
<img width="1920" height="2560" alt="image" src="https://github.com/user-attachments/assets/561f7ca3-276e-4a2c-b501-cb7de1e3a219" />


> Overall, the meet-up delivered a great deal of practical insight through 5 high-quality sessions—from Voice AI and multi-account management to early pentesting and guardrails for Agents—while also energizing me to connect confidently and learn more.

