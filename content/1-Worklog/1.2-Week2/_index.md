---
title: "Week 2 Worklog"
date: 2026-01-11
weight: 2
chapter: false
pre: "<b>1.2. </b>"
---

### Week 2 Objectives

- Complete Module 2, focusing on understanding EC2 and VPC.
- Prepare necessary resources for launching an EC2 instance.
- Explore Route 53 and its related concepts.

### Tasks to be carried out this week

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 1 | - Deepen understanding of VPC and its services/resources.<br>- Study AWS architecture design principles.<br>- Review concepts from Mentor Gia Hung's lectures. | 11/01/2026 | 12/01/2026 | [REFER HERE](https://cloudjourney.awsstudygroup.com/) |
| 2 | - Create resources within a VPC to prepare for EC2 instance creation.<br>- Launch an EC2 instance using prepared resources.<br>- Learn about Security Groups and Network ACLs. | 12/01/2026 | 13/01/2026 | [REFER HERE](https://docs.aws.amazon.com/ec2/) |
| 3 | - Resolve AWS account authentication issues and submit required verification documents. | 13/01/2026 | 16/01/2026 | [REFER HERE](https://aws.amazon.com/support/) |
| 4 | - Attend the Cloud Day event.<br>- Gain insights into AI and Data through the event.<br>- Network with prominent mentors. | 14/01/2026 | 14/01/2026 | |

### Week 2 Achievements

- Gained foundational knowledge of VPC and EC2, including their core concepts and configurations.
- Understood the necessary steps and resources required to launch an EC2 instance.
- Successfully created and configured essential resources for EC2 setup, including:
  - Subnets for network segmentation.
  - An Internet Gateway for external connectivity.
  - Route Table rules to manage traffic routing.
  - Security Groups to control inbound and outbound traffic for EC2 instances.
- Resolved AWS account authentication issues by submitting verification documents.
- Participated in the Cloud Day event, networking with mentors and gaining valuable insights.
- Enhanced understanding of AI and Data, including current market demands and the future potential of AI.

### Frontend ↔ AWS touchpoints (from a FE perspective)

- **VPC:** Explained how network boundaries and rules can block API calls even when frontend code is correct.
- **IAM:** Clarified that permissions live in IAM (roles/policies). Frontend typically authenticates via backend mechanisms (tokens/cookies), not AWS access keys.
- **S3 (static resources):** Understood how static files can be delivered from S3 (useful for frontend assets or downloads).
- **API Gateway:** Learned how the frontend can call a single managed API endpoint, and why API Gateway is often used for routing + centralized CORS.
- **Route 53:** Learned to prefer a domain-based API URL (stable, easier environment switching) rather than embedding IPs in the frontend.
