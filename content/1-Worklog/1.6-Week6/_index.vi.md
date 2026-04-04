---
title: "Worklog Tuần 6"
date: 2026-02-09
weight: 6
chapter: false
pre: "<b>1.6. </b>"
---

### Mục tiêu tuần 6

- Hiểu các khái niệm cốt lõi về dịch vụ lưu trữ trên AWS.
- Tiếp tục học Python cơ bản.
- Hoàn thiện sơ đồ kiến trúc và cấu trúc code skeleton của dự án.
- Tham gia webinar "Reinventing DevSecOps with AWS Generative AI" để tìm hiểu về DevSecOps và Amazon Q Developer.

### Công việc triển khai trong tuần

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
|-----|-----------|--------------|-----------------|--------------------|
| 1 | - Tìm hiểu Amazon S3: Bucket, độ bền dữ liệu và Static Website Hosting.<br>- Ôn tập các lớp lưu trữ S3 (Standard, Standard-IA) và Glacier. | 09/02/2026 | 10/02/2026 | [THAM KHẢO](https://aws.amazon.com/s3/) |
| 2 | - Tìm hiểu AWS Storage Gateway (File, Volume, Tape).<br>- Học Object Lifecycle Management.<br>- Tiếp tục luyện Python cơ bản.<br>- Tham gia webinar "Reinventing DevSecOps with AWS Generative AI" (Hoàng Kha). | 11/02/2026 | 12/02/2026 | [THAM KHẢO](https://aws.amazon.com/storagegateway/)<br>[THAM KHẢO](https://aws.amazon.com/events/) |
| 3 | - Học các khái niệm Disaster Recovery: RTO, RPO và Backup & Restore.<br>- Tìm hiểu AWS Backup.<br>- Thực hành tạo S3 Bucket, tải file lên và cấu hình Static Website Hosting.<br>- Tìm hiểu vai trò DevSecOps và các công cụ phổ biến (CI/CD, SAST, DAST, Terraform). | 13/02/2026 | 14/02/2026 | [THAM KHẢO](https://aws.amazon.com/backup/) |
| 4 | - Cập nhật sơ đồ kiến trúc hạ tầng.<br>- Tái cấu trúc code skeleton theo thiết kế mới.<br>- Chốt ngôn ngữ lập trình và framework cho dự án.<br>- Khám phá Amazon Q Developer. | 15/02/2026 | 16/02/2026 | [THAM KHẢO](https://aws.amazon.com/q/developer/) |

### Kết quả đạt được tuần 6

- Nắm được các khái niệm quan trọng của Amazon S3: Bucket, độ bền, Static Website Hosting và các storage class (Standard, Standard-IA, Glacier).
- Hiểu vai trò của AWS Storage Gateway và Object Lifecycle Management trong tối ưu dữ liệu.
- Hoàn thành bài thực hành tạo S3 Bucket và cấu hình website tĩnh.
- Củng cố kiến thức Python cơ bản và áp dụng vào một số tác vụ nhỏ trong dự án.
- Cập nhật sơ đồ kiến trúc, điều chỉnh luồng dữ liệu và bố cục triển khai.
- Tái cấu trúc code skeleton với cấu trúc thư mục và file cấu hình phù hợp hơn.
- Chốt ngôn ngữ và framework sử dụng cho dự án.

- **S3 (static resources):** Tuần trọng tâm. Hiểu cách frontend có thể tải asset tĩnh từ S3 (Static Website hosting/public URL) và lý do cần cache/version.
- **IAM:** Xác nhận best practice: không nhúng AWS credential vào trình duyệt. Nếu có upload/download file thì nên đi qua backend API hoặc dùng pre-signed URL.
- **API Gateway:** Nếu dùng, frontend gọi các API upload/download thông qua một endpoint tập trung thay vì gọi trực tiếp từng service.
- **Route 53:** Domain ổn định giúp cấu hình frontend sạch hơn (đổi môi trường dễ, không hardcode URL/IP).
- **VPC:** Hiểu rằng backend/storage có thể ở private network; frontend chỉ truy cập qua endpoint public.
