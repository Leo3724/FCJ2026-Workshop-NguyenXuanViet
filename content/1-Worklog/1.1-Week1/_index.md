---
title: "Week 1 Worklog"
date: 2026-01-05
weight: 1
chapter: false
pre: "<b>1.1. </b>"
---

### Week 1 Objectives

- Connect and get acquainted with members of First Cloud Journey (FCJ).
- Understand the organization and basic AWS services.

### Tasks to be carried out this week

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 1 | - Attend the FCJ kick-off session.<br>- Learn about the FCJ organization.<br>- Form a team for collaborative project work. | 05/01/2026 | 05/01/2026 | |
| 2 | - Create an AWS account.<br>- Study cloud computing concepts.<br>- Draw a sample architecture using draw.io. | 06/01/2026 | 06/01/2026 | [REFER HERE](https://cloudjourney.awsstudygroup.com/) |
| 3 | - Explore the objectives of the First Cloud Journey program and the AWS website.<br>- Perform initial setup on the AWS account:<br>&emsp;+ Create a budget.<br>&emsp;+ Create user groups.<br>&emsp;+ Enable two-factor authentication (2FA).<br>- Learn about the AWS Support Center and how to submit support requests. | 07/01/2026 | 07/01/2026 | [REFER HERE](https://cloudjourney.awsstudygroup.com/) |
| 4 | - Create a VPC and configure its settings.<br>- Create and configure Subnets (including a public Subnet with auto-assigned public IPs).<br>- Set up an Internet Gateway and attach it to the VPC.<br>- Create and configure a Route Table, connecting it to the Internet Gateway.<br>- Configure Subnet Associations.<br>- Create Security Groups (public and private). | 08/01/2026 | 11/01/2026 | [REFER HERE](https://cloudjourney.awsstudygroup.com/) |

### Week 1 Achievements

- Successfully participated in the FCJ kick-off session and connected with team members.
- Gained an understanding of the FCJ organization and its objectives.
- Formed a team to collaborate on projects.
- Created an AWS account and completed initial setup tasks:
  - Set up a budget to monitor costs.
  - Created user groups for access management.
  - Enabled two-factor authentication (2FA) for enhanced security.
- Studied basic cloud computing concepts and successfully drew a sample architecture using draw.io.
- Learned how to navigate the AWS Support Center and submit support requests.
- Successfully completed VPC-related tasks:
  - Created and configured a VPC.
  - Set up Subnets, including a public Subnet with auto-assigned public IPs.
  - Created and attached an Internet Gateway to the VPC.
  - Configured a Route Table and connected it to the Internet Gateway.
  - Established Subnet Associations.
  - Created public and private Security Groups for secure resource access.
- **IAM (users/groups, MFA):** Learned the security mindset early (least privilege, MFA). In real frontend work, I don’t embed AWS keys; access to AWS resources is usually via backend roles and controlled endpoints.

### Frontend ↔ AWS touchpoints (what I learned for FE later)

- **VPC:** Understanding public/private networking and Security Groups helped me debug why the frontend can/can’t reach backend APIs (timeout vs app error).
- **IAM:** Reinforced that AWS permissions are enforced on the cloud side (roles/policies). A browser frontend should not store AWS keys; it should use backend-issued auth (e.g., JWT/session).
- **S3 (static resources):** Introduced the idea that static assets (images/build output) can be served from S3 via URLs.
- **API Gateway:** Learned the concept of an API “front door” that a frontend calls as a single endpoint (and why CORS can be configured centrally).
- **Route 53:** Understood why a stable domain is important for frontend configuration instead of hardcoding IP addresses.
