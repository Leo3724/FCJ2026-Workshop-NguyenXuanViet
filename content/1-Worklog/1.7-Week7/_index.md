---
title: "Week 7 Worklog"
date: 2026-02-23
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Week 7 Objectives:

* Concentrate on reviewing and reinforcing core knowledge to prepare effectively for the mid-term examination.
* Complete lab practices and multiple-choice exercises on AWS Builders and AWSboy to become familiar with exam structure and question styles.
* Organize and summarize key concepts of essential AWS services such as EC2, S3, VPC, IAM, and RDS.

---

### Tasks Completed This Week:

| Day | Task | Start Date | Completion Date | Resources |
| :--- | :--- | :--- | :--- | :--- |
| Monday | - Review and summarize Compute services including EC2 and Lambda.<br>- Practice hands-on labs for creating, configuring, and managing the lifecycle of an EC2 instance. | 23/02/2026 | 23/02/2026 | AWS Builders, AWSboy |
| Tuesday | - Revisit Storage services such as S3, EBS, and EFS.<br>- Practice exercises on S3 storage classes (Standard, Infrequent Access, Glacier) and EBS configurations. | 24/02/2026 | 24/02/2026 | AWS Builders, AWSboy |
| Wednesday | - Strengthen Networking concepts including VPC, Subnets, Route Tables, Internet Gateway, and Security Groups.<br>- Complete exercises on VPC setup and Security Group/NACL rules. | 25/02/2026 | 25/02/2026 | AWS Builders, AWSboy |
| Thursday | - Review Database services (RDS, DynamoDB) together with Identity and Security services (IAM).<br>- Practice IAM Policies and IAM Roles. | 26/02/2026 | 26/02/2026 | AWS Builders, AWSboy |
| Friday | - Perform overall review and mock testing through practice exams on AWS Builders and AWSboy.<br>- Identify weak areas and revise them further. | 27/02/2026 | 27/02/2026 | AWS Builders, AWSboy |

---

### Week 7 Achievements:

* Completed a thorough revision of major AWS service categories: Compute, Storage, Networking, Database, and Security.
* Practiced a large number of labs and quiz questions on both AWS Builders and AWSboy platforms.
* Built a solid understanding of EC2 components (Instance Types, AMIs, EBS volumes) and S3 concepts (buckets, objects, storage classes).
* Improved understanding of interactions inside a VPC, especially differences between public/private subnets and routing behavior.
* Increased confidence in AWS foundational knowledge and readiness for the upcoming mid-term assessment.

---

### Frontend ↔ AWS touchpoints (service mapping recap)

- **VPC:** Explains reachability issues when frontend calls APIs (private/public networking, security rules).
- **IAM:** AWS-side access control is handled via IAM roles/policies; frontend should only use backend-issued auth (JWT/cookies), not AWS keys.
- **S3 (static resources):** Frontend can load images/files from S3 via URL; uploads/downloads should go through backend or pre-signed URLs.
- **API Gateway:** If present, it’s the single API endpoint the frontend calls (routing + centralized CORS).
- **Route 53:** Domain routing keeps API/frontend endpoints stable and avoids hardcoded IPs.
