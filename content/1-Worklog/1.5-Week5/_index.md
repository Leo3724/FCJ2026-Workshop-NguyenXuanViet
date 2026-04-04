---
title: "Week 5 Worklog"
date: 2026-02-02
weight: 5
chapter: false
pre: "<b>1.5. </b>"
---

## Week 5 Objectives

- Review and pinpoint the root causes of unreasonable AWS service costs.
- Design the project infrastructure architecture and split it into clear components.
- Start initial environment setup and assign roles across the project team.

## Tasks to be carried out this week

| No. | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 1 | - Analyze unusual AWS spending patterns and identify the primary causes. | 02/02/2026 | 03/02/2026 | [Refer here](https://aws.amazon.com/aws-cost-management/aws-cost-explorer/) |
| 2 | - Design the project infrastructure architecture and break it into functional blocks.<br>- Propose baseline architecture patterns for team review and selection. | 04/02/2026 | 05/02/2026 | [Refer here](https://www.facebook.com/groups/awsstudygroupfcj) |
| 3 | - Build the initial code skeleton and configure the required bootstrap files for the project. | 06/02/2026 | 08/02/2026 | |

## Week 5 Achievements

- Finalized the infrastructure architecture design and provided practical reference patterns for the team.
- Successfully established the code skeleton and initial configuration files, creating a solid base for implementation.
- Registered and activated an AWS Skill Builder account, then started exploring relevant learning paths and materials.
- Identified the main reasons for abnormal costs: EC2 resources were not fully cleaned up and user account governance was insufficient; then proposed cost-optimization actions.

## Frontend ↔ AWS touchpoints (how the FE fits the architecture)

- **VPC:** Understood that backend services may run in private networks; frontend should talk to an exposed public endpoint, not private IPs.
- **IAM:** Defined the permission boundary: IAM roles/policies protect AWS resources; frontend uses backend-issued auth (JWT/cookies) to call APIs.
- **S3 (static resources):** Planned to store/serve static assets (images/build artifacts) from S3 so the UI can load them via URLs.
- **API Gateway:** If adopted, it provides a single managed endpoint for the frontend (routing + centralized CORS handling).
- **Route 53:** Planned to use domains for frontend/API URLs to avoid hardcoding IPs and to support environment switching.
