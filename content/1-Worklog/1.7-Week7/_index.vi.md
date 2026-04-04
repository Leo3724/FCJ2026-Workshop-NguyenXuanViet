---
title: "Worklog Tuần 7"
date: 2026-02-23
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:

* Tập trung ôn tập và củng cố kiến thức cốt lõi để chuẩn bị hiệu quả cho bài kiểm tra giữa kỳ.
* Hoàn thành các bài lab và trắc nghiệm trên AWS Builders và AWSboy để làm quen cấu trúc đề và dạng câu hỏi.
* Hệ thống và tóm tắt các khái niệm quan trọng của các dịch vụ AWS thiết yếu như EC2, S3, VPC, IAM và RDS.

---

### Công việc đã hoàn thành trong tuần:

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài nguyên |
| :--- | :--- | :--- | :--- | :--- |
| Thứ Hai | - Ôn tập và tổng hợp nhóm dịch vụ Compute gồm EC2 và Lambda.<br>- Thực hành lab tạo, cấu hình và quản lý vòng đời một EC2 instance. | 23/02/2026 | 23/02/2026 | AWS Builders, AWSboy |
| Thứ Ba | - Ôn lại nhóm dịch vụ Storage như S3, EBS và EFS.<br>- Thực hành bài tập về các lớp lưu trữ S3 (Standard, Infrequent Access, Glacier) và cấu hình EBS. | 24/02/2026 | 24/02/2026 | AWS Builders, AWSboy |
| Thứ Tư | - Củng cố kiến thức Networking gồm VPC, Subnet, Route Table, Internet Gateway và Security Group.<br>- Làm bài tập về cấu hình VPC và quy tắc Security Group/NACL. | 25/02/2026 | 25/02/2026 | AWS Builders, AWSboy |
| Thứ Năm | - Ôn tập dịch vụ Database (RDS, DynamoDB) cùng nhóm Identity & Security (IAM).<br>- Thực hành trọng tâm về IAM Policy và IAM Role. | 26/02/2026 | 26/02/2026 | AWS Builders, AWSboy |
| Thứ Sáu | - Tổng ôn và làm bài thi thử trên AWS Builders và AWSboy.<br>- Xác định phần kiến thức còn yếu để ôn lại. | 27/02/2026 | 27/02/2026 | AWS Builders, AWSboy |

---

### Kết quả đạt được tuần 7:

* Hoàn thành ôn tập toàn diện các nhóm dịch vụ AWS chính: Compute, Storage, Networking, Database và Security.
* Thực hành nhiều bài lab và câu hỏi trắc nghiệm trên cả AWS Builders và AWSboy.
* Nắm chắc các thành phần quan trọng của EC2 (Instance Types, AMI, EBS) và các khái niệm S3 (bucket, object, storage class).
* Hiểu rõ hơn cách các thành phần trong VPC tương tác, đặc biệt là khác biệt giữa subnet public/private và cơ chế định tuyến.
* Tăng sự tự tin về kiến thức nền tảng AWS và sẵn sàng cho kỳ kiểm tra giữa kỳ sắp tới.

---

- **VPC:** Giải thích vấn đề reachability khi frontend gọi API (private/public networking, security rule).
- **IAM:** IAM role/policy kiểm soát quyền phía AWS; frontend chỉ dùng cơ chế auth do backend cấp (JWT/cookie), không dùng AWS key.
- **S3 (static resources):** Frontend tải image/file qua URL; upload/download nên đi qua backend hoặc pre-signed URL.
- **API Gateway:** Nếu có, đây là endpoint API duy nhất frontend gọi (routing + CORS tập trung).
- **Route 53:** DNS routing giúp endpoint frontend/API ổn định và tránh hardcode IP.
