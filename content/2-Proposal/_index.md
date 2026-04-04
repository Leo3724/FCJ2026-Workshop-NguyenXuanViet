---
title: "Proposal"
date: 2026-01-01
weight: 2
chapter: false
pre: " <b> 2. </b> "
---

# AI-Assisted Electronics Production Management System
*(A unified AWS-based platform for production planning and monitoring)*

## 1. Executive Summary

The AI-Assisted Production Management System is designed for small and medium-sized electronics manufacturing enterprises (SMEs) to improve order management, production planning, and production monitoring. The system supports multiple production lines (SMT, DIP, testing) and can scale as the number of orders and lines increases.

The platform provides centralized management of production data, visualizes progress, and detects delays early at each stage. The solution leverages AWS services such as Amazon ECS, Amazon ECR, Amazon RDS, Amazon S3, Amazon CloudFront, Amazon Route 53, Amazon CloudWatch, AWS Secrets Manager, Amazon SNS, Amazon SQS, and Amazon SES to ensure stability, security, scalability, and cost optimization.

In addition, the system integrates an AI component to help users quickly look up information related to orders, production schedules, OEE indicators, Gantt charts, and simple delay scenarios. Users can ask natural-language questions such as:
- “Which stage is order X currently in?”
- “What is today’s OEE on SMT line 1?”
- “Which stage is causing delays for this week’s plan?”

The system answers based on collected and aggregated production data.

## 2. Problem Statement

### Problem

In electronics manufacturing SMEs, common issues include:
- Production planning is done manually in Excel, making it difficult to optimize lines and capacity.
- No real-time tracking of production progress at each stage.
- Order, work order, and reporting data are scattered across many files and systems.
- Difficult to assess line capability, waiting time, and bottlenecks in the process.
- Internal systems are hard to scale, rely on on-premise infrastructure, and lack centralized monitoring.

### Solution

The system provides a centralized web platform for production management and analytics:
- A backend that handles business logic (orders, work orders, plans, reports) running as containers on ECS.
- A web interface for management, progress tracking, and dashboards of line status.
- Business data stored in RDS with a relational model to support reporting queries.
- Production documents (POM/SOOP, forms) and deployment artifacts stored separately in three S3 buckets.
- Background tasks (e.g., sending notifications, batch processing) use SQS to decouple from the main request flow.
- SNS and SES send alerts and email notifications to managers/engineers when incidents occur.
- CloudWatch and Secrets Manager provide monitoring and secure management of connection information and system configuration.
- An AI component is integrated to query production data using natural language, helping users quickly see order status, production schedules, OEE, Gantt charts, bottlenecks, and simple delays without manually filtering through many screens and reports.

### Benefits and Return on Investment

- Reduce manual work in managing and aggregating production data.
- Improve the ability to track progress and detect delays early on production lines.
- Create a centralized data source to support analytics, reporting, and future AI applications.
- Use AWS infrastructure to reduce upfront capital expenditure, pay per use, and scale with factory growth.

## 3. Solution Architecture

The system uses a cloud architecture deployed on AWS:
- Users access the system via a web interface hosted on Amazon S3 and delivered through CloudFront.
- DNS and routing are managed via Amazon Route 53.
- Requests are routed to the backend running on Amazon ECS.
- The backend processes data and stores it in a relational database on Amazon RDS.

### File / Artifact Storage Strategy (3 S3 buckets)

- **S3 Bucket 1 (POM/SOOP & production documents):** stores POM/SOOP files and related production documents.
- **S3 Bucket 2 (Frontend hosting):** stores the built frontend (React app) for S3 static hosting.
- **S3 Bucket 3 (Artifacts & packages):** stores deployment artifacts and application packages to support the deployment pipeline.

### Asynchronous Processing & Notifications

- Background and asynchronous tasks use Amazon SQS.
- Notifications and alerts use Amazon SNS and Amazon SES.

### Security & Observability

- Sensitive data (DB credentials, API keys, email configuration) is stored in AWS Secrets Manager.
- Logs, metrics, and alarms are monitored centrally via Amazon CloudWatch.

### Proposal Image

![Solution Architecture Diagram](/images/2-Proposal/aws.png)

### AWS Services Used

- **Amazon ECS**: runs backend production management services.
- **Amazon ECR**: stores Docker images for backend services.
- **Amazon RDS (PostgreSQL/MySQL)**: stores production data (orders, work orders, plans, progress).
- **Amazon S3 (Bucket 1)**: stores POM/SOOP files and production documents.
- **Amazon S3 (Bucket 2)**: hosts the frontend (React app).
- **Amazon S3 (Bucket 3)**: stores deployment artifacts and application packages.
- **Amazon CloudFront**: delivers the frontend via CDN.
- **Amazon Route 53**: manages domain and DNS routing.
- **Amazon SES**: sends emails (notifications, alerts, scheduled reports).
- **Amazon SQS**: message queue for background tasks, batch jobs, and retries.
- **Amazon SNS**: sends alerts/notifications and integrates with other channels.
- **Amazon CloudWatch**: monitors logs, metrics, and sets alarms.
- **AWS Secrets Manager**: securely stores sensitive information (DB passwords, API keys).

### Component Design

**Frontend**
- Hosted on S3.
- Delivered via CloudFront.
- Provides dashboards and management UI for production (orders, plans, lines).

**Backend**
- Runs on ECS as containers.
- Handles business logic: orders, work orders, scheduling, reporting, and APIs for the frontend.
- Publishes/consumes messages with SQS/SNS to handle background tasks.

**Database**
- RDS stores orders, production plans, progress, production history, and reports.

**File Storage**
- POM/SOOP S3 bucket stores process documents and production instructions.
- Frontend S3 bucket stores the built web application.
- Artifact S3 bucket stores deployment packages and configuration backups.

**Security & Monitoring**
- Secrets Manager stores sensitive configuration.
- CloudWatch collects logs/metrics and triggers alerts via SNS/SES.

## 4. Technical Implementation

### Implementation Phases

The project is developed in four phases:
1. Analyze requirements and design the architecture based on the actual AWS stack.
2. Build backend containers, push images to ECR, and deploy on ECS.
3. Deploy the frontend to S3 + CloudFront and configure the domain via Route 53.
4. Integrate RDS, SQS, SNS, SES, Secrets Manager, and CloudWatch; perform end-to-end testing.

### Technical Requirements

**System Requirements**
- Web application for end users.
- Support storing production content and related documents.
- Provide monitoring, alerting, and email notification mechanisms.

**Technology Stack**
- Backend: Spring Boot (containerized).
- Frontend: React.
- Database: Amazon RDS (PostgreSQL/MySQL).
- Cloud: AWS (S3, CloudFront, ECS, ECR, Route 53, CloudWatch, Secrets Manager, SNS, SQS, SES).

## 5. Timeline & Milestones

- Pre-development: Clarify functional scope, design the architecture, and define naming for the three S3 buckets.
- Development phase: Complete backend on ECS/ECR and integrate RDS, SQS, SNS, SES.
- Deployment phase: Deploy frontend via S3/CloudFront and connect the domain with Route 53.
- Post-launch: Monitor with CloudWatch and optimize cost and performance based on real data.

## 6. Budget Estimation

Infrastructure costs are usage-based monthly costs for a small-scale setup.

| Service | Monthly Cost (USD) |
|---|---:|
| Amazon ECS | 6.00 |
| Amazon ECR | 1.00 |
| Amazon RDS | 12.00 |
| Amazon S3 (3 buckets) | 2.00 |
| Amazon CloudFront | 1.50 |
| Amazon Route 53 | 0.50 |
| Amazon SQS + Amazon SNS | 2.00 |
| Amazon SES | 0.50 |
| AWS Secrets Manager | 0.80 |
| Amazon CloudWatch | 2.50 |
| **Total** | **28.80** |

**Annual cost:** ~ $345.60 / year

**Development cost:**
- No physical server investment.
- Uses existing development environment.
- AI API cost depends on usage.

## 7. Risk Assessment

### Risks

- Increased costs when traffic grows quickly or RDS queries are not optimized.
- SQS backlog during peak hours.
- Misconfigured secrets causing service connectivity issues.

### Mitigation Strategies

- Set up CloudWatch alarms for ECS, RDS, SQS, and SES.
- Optimize queries and indexing on RDS.
- Apply least-privilege IAM and centralized secret management.
- Configure retries and monitor failed messages in queues.

### Contingency Plans

- Take regular RDS snapshots and test restore procedures.
- Maintain stable image versions in ECR for quick rollback.
- Send immediate alerts via SNS/email when thresholds are exceeded.

## 8. Expected Outcomes

### Technical Improvements

- Stable system operation with clear separation of frontend, backend, and data layers.
- Increased scalability and availability thanks to AWS container-based architecture.
- Improved observability and incident handling with CloudWatch + SNS + SES.
- An AI layer that supports Q&A about orders, schedules, OEE, Gantt charts, and simple delays—helping users access information faster and rely less on specialist analysts.

### Long-term Value

- A solid technical foundation for extending the production management and analytics system (e.g., load forecasting, schedule optimization, delay root-cause analysis).
- Standardized deployment and operations for future versions.
- Optimized operational costs aligned with production growth.
