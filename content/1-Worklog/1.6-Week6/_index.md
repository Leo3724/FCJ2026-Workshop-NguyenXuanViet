---
title: "Week 6 Worklog"
date: 2026-02-09
weight: 6
chapter: false
pre: "<b>1.6. </b>"
---

### Week 6 Objectives

- Understand core AWS storage concepts.
- Continue learning basic Python.
- Refine the project architecture diagram and code skeleton.
- Join the "Reinventing DevSecOps with AWS Generative AI" webinar to learn DevSecOps practices and Amazon Q Developer.

### Tasks to be carried out this week

| Day | Task | Start Date | Completion Date | Reference Material |
|-----|------|------------|-----------------|---------------------|
| 1 | - Learn Amazon S3 fundamentals: Buckets, durability, and Static Website hosting.<br>- Review S3 Storage Classes (Standard, Standard-IA) and Glacier. | 09/02/2026 | 10/02/2026 | [REFER HERE](https://aws.amazon.com/s3/) |
| 2 | - Study AWS Storage Gateway (File, Volume, Tape).<br>- Learn Object Lifecycle Management.<br>- Continue basic Python practice.<br>- Attend the "Reinventing DevSecOps with AWS Generative AI" webinar (Hoang Kha). | 11/02/2026 | 12/02/2026 | [REFER HERE](https://aws.amazon.com/storagegateway/)<br>[REFER HERE](https://aws.amazon.com/events/) |
| 3 | - Learn Disaster Recovery concepts: RTO, RPO, and Backup & Restore.<br>- Explore AWS Backup.<br>- Practice creating an S3 Bucket, uploading files, and enabling Static Website hosting.<br>- Learn DevSecOps role and common tools (CI/CD, SAST, DAST, Terraform). | 13/02/2026 | 14/02/2026 | [REFER HERE](https://aws.amazon.com/backup/) |
| 4 | - Update the infrastructure architecture diagram.<br>- Restructure the code skeleton based on the updated design.<br>- Finalize project language and framework.<br>- Explore Amazon Q Developer. | 15/02/2026 | 16/02/2026 | [REFER HERE](https://aws.amazon.com/q/developer/) |

### Week 6 Achievements

- Understood key Amazon S3 concepts: Buckets, durability, Static Website hosting, and storage classes (Standard, Standard-IA, Glacier).
- Learned AWS Storage Gateway types and Object Lifecycle Management for data optimization.
- Completed hands-on S3 practice by creating a bucket and configuring website hosting.
- Improved basic Python skills and applied them to simple project tasks.
- Refined the infrastructure diagram and updated project data flows.
- Reorganized the code skeleton with a more suitable structure and configuration setup.
- Finalized the project language and framework.

### Frontend ↔ AWS touchpoints (from a FE perspective)

- **S3 (static resources):** Focus week. Learned patterns for serving static assets from S3 (Static Website hosting / public URLs) and why versioning/cache matters for frontend delivery.
- **IAM:** Confirmed best practice: don’t embed AWS credentials in the browser. For upload/download, prefer backend APIs or pre-signed URLs.
- **API Gateway:** If used, the frontend consumes S3-related features (upload/download APIs) through a single API entry point.
- **Route 53:** A stable domain helps keep frontend configs clean (same domain pattern across environments).
- **VPC:** Understood that storage and backend components may live in private networks; frontend calls only public endpoints.
