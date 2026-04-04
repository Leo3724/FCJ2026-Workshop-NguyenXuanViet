---
title: "Week 3 Worklog"
date: 2026-01-18
weight: 3
chapter: false
pre: "<b>1.3. </b>"
---

### Week 3 Goals

- Resolve AWS account issues and prepare a replacement account when needed.
- Learn how to implement Hybrid DNS with Route 53 Resolver.
- Practice VPC Peering to enable communication across separate VPCs.
- Sync with teammates on project direction and selected technologies.

### Weekly Activities

| Day | Task | Start Date | End Date | References |
| --- | --- | --- | --- | --- |
| 1 | - Register a new Visa card.<br>- Create a new AWS account and complete the baseline configuration. | 18/01/2026 | 20/01/2026 | [REFER HERE](https://aws.amazon.com/getting-started/) |
| 2 | - Finish Lab 10 focused on Route 53.<br>- Configure Hybrid DNS with Route 53 Resolver.<br>- Deploy a virtual machine to validate DNS behavior. | 21/01/2026 | 22/01/2026 | [REFER HERE](https://youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&si=NtlkPHvTydrkH4rK) |
| 3 | - Set up VPC Peering between multiple VPC environments.<br>- Prepare required supporting resources for peering.<br>- Clean up unused resources after lab completion. | 22/01/2026 | 23/01/2026 | [REFER HERE](https://youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&si=NtlkPHvTydrkH4rK) |
| 4 | - Join a team alignment session.<br>- Finalize the primary programming language and assign learning tasks. | 25/01/2026 | 25/01/2026 | |

### Week 3 Outcomes

- Completed registration of a new AWS account and finished initial setup to continue FCJ project work.
- Built a practical understanding of Route 53 and Hybrid DNS, including:
  - Creating and configuring Route 53 Resolver Outbound Endpoints.
  - Setting up Inbound Endpoints for DNS query resolution.
  - Validating connectivity through an RD Gateway Server.
- Understood how VPC Peering provides secure private communication between VPCs without routing through the public internet.
- Practiced infrastructure provisioning using AWS CloudFormation templates.
- Learned how to configure Cross-Zone and Cross-Region DNS Resolution for VPC Peering:
  - Enabling EC2 instances in different VPCs to resolve private DNS names correctly.
  - Recognizing that missing this setting can cause DNS to resolve to public IPs and send traffic out of the private network.
- Joined planning meetings, agreed on the technology stack, and aligned the team learning schedule.

### Frontend ↔ AWS touchpoints (from a FE perspective)

- **Route 53:** Reinforced that the frontend should target a correct domain for API endpoints (instead of private DNS names or IPs).
- **VPC:** Better understood how private networking decisions affect whether services are reachable publicly or only inside a VPC.
- **API Gateway:** If used, it becomes the public API entry point the frontend calls, even when backend services live in private subnets.
- **IAM:** Confirmed the security model: IAM is used to protect AWS resources on the backend side; frontend access is through secured HTTP APIs (JWT/cookies).
- **S3 (static resources):** Noted that S3 can serve static documents/assets to the frontend via URL, while keeping backend services private.
