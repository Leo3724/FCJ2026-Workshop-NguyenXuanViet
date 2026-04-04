---
title: "Week 4 Worklog"
date: 2026-01-25
weight: 4
chapter: false
pre: "<b>1.4. </b>"
---

### Week 4 Objectives

- Stay aligned with the team’s learning timeline.
- Become confident in setting up and configuring AWS Transit Gateway.
- Strengthen knowledge of Amazon EC2 and its related capabilities.

### Tasks to be carried out this week

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 1 | - Study AWS Transit Gateway, including concepts, configuration steps, and required components.<br>- Identify key differences between VPC Peering and AWS Transit Gateway. | 25/01/2026 | 26/01/2026 | [REFER HERE](https://aws.amazon.com/transit-gateway/) |
| 2 | - Expand understanding of Amazon EC2 through Module 3 lectures (features, configuration options, and practical use cases). | 27/01/2026 | 28/01/2026 | [REFER HERE](https://youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&si=NtlkPHvTydrkH4rK) |
| 3 | - Learn and practice essential Git commands (commit, push, pull) to improve team collaboration. | 29/01/2026 | 30/01/2026 | [REFER HERE](https://www.youtube.com/watch?v=8O14qT3jdq0&list=PLodO7Gi1F7R0t9SyEZF5mwfKevCULLjgG&index=2) |
| 4 | - Propose solution ideas and allocate responsibilities to team members in preparation for the project proposal. | 31/01/2026 | 01/02/2026 | |

### Week 4 Achievements

- Successfully configured AWS Transit Gateway and understood its strengths compared to VPC Peering, especially for complex multi-VPC and multi-resource connectivity.
- Built a strong understanding of Amazon EC2 core capabilities:
  - Elastic scaling to increase or decrease resources based on workload.
  - Flexible instance configuration options.
  - Cost optimization using different pricing models.
- Understood how EC2 Auto Scaling works for automatic resource adjustment.
- Learned about Instance Store as part of EC2 storage options.
- Explored Amazon Lightsail as a straightforward and cost-effective option for small applications.
- Understood AWS Application Migration Service (MGN) and its role in migrating on-premises servers to AWS.
- Became comfortable using foundational Git commands (commit, push, pull) and collaborative Git workflows.
- Proposed project ideas and assigned team tasks, helping the team get ready for implementation.

### Frontend ↔ AWS touchpoints (from a FE perspective)

- **VPC:** Helped me understand system-level networking. For frontend, this translates into knowing why an API may be unreachable (private subnet, routing, security rules).
- **IAM:** Reconfirmed that IAM governs AWS-side permissions; frontend should rely on backend authentication/authorization and must not include AWS credentials.
- **S3 (static resources):** Considered S3 as a place to serve static assets for the UI or store downloadable files.
- **API Gateway:** Understood the benefit of a central API endpoint for frontend calls (routing, throttling, unified CORS).
- **Route 53:** Emphasized using DNS names for frontend configuration so API endpoints remain stable across deployments.
