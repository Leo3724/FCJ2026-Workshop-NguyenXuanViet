---
title: "Worklog Tuần 4"
date: 2026-01-25
weight: 4
chapter: false
pre: "<b>1.4. </b>"
---

### Mục tiêu tuần 4

- Duy trì tiến độ học tập đồng bộ với cả nhóm.
- Thành thạo quy trình thiết lập và cấu hình AWS Transit Gateway.
- Củng cố kiến thức về Amazon EC2 và các tính năng liên quan.

### Các công việc cần triển khai trong tuần này

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | - Tìm hiểu AWS Transit Gateway, bao gồm khái niệm, các bước cấu hình và những thành phần cần thiết.<br>- So sánh các điểm khác nhau giữa VPC Peering và AWS Transit Gateway. | 25/01/2026 | 26/01/2026 | [THAM KHẢO](https://aws.amazon.com/transit-gateway/) |
| 2 | - Mở rộng kiến thức về Amazon EC2 thông qua bài giảng Module 3 (tính năng, tùy chọn cấu hình và các tình huống ứng dụng thực tế). | 27/01/2026 | 28/01/2026 | [THAM KHẢO](https://youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&si=NtlkPHvTydrkH4rK) |
| 3 | - Học và thực hành các lệnh Git cơ bản (commit, push, pull) để cải thiện khả năng cộng tác trong nhóm. | 29/01/2026 | 30/01/2026 | [THAM KHẢO](https://www.youtube.com/watch?v=8O14qT3jdq0&list=PLodO7Gi1F7R0t9SyEZF5mwfKevCULLjgG&index=2) |
| 4 | - Đề xuất ý tưởng giải pháp và phân công trách nhiệm cho các thành viên nhằm chuẩn bị cho phần proposal của dự án. | 31/01/2026 | 01/02/2026 | |

### Kết quả đạt được tuần 4

- Đã cấu hình thành công AWS Transit Gateway và hiểu rõ các điểm mạnh so với VPC Peering, đặc biệt trong các mô hình kết nối nhiều VPC và nhiều loại tài nguyên.
- Nắm vững các năng lực cốt lõi của Amazon EC2:
  - Khả năng co giãn tài nguyên theo nhu cầu tải.
  - Tùy chọn cấu hình instance linh hoạt.
  - Tối ưu chi phí thông qua nhiều mô hình định giá.
- Hiểu cách EC2 Auto Scaling hoạt động để tự động điều chỉnh tài nguyên.
- Tìm hiểu Instance Store như một tùy chọn lưu trữ trong hệ sinh thái EC2.
- Khám phá Amazon Lightsail như một lựa chọn đơn giản và tiết kiệm chi phí cho các ứng dụng quy mô nhỏ.
- Hiểu về AWS Application Migration Service (MGN) và vai trò của dịch vụ trong việc di chuyển máy chủ on-premises lên AWS.
- Sử dụng thành thạo các lệnh Git nền tảng (commit, push, pull) và quy trình làm việc cộng tác với Git.
- Đề xuất được các ý tưởng cho dự án và phân công công việc trong nhóm, tạo nền tảng sẵn sàng cho giai đoạn triển khai.

- **VPC:** Hiểu networking mức hệ thống; với frontend điều này giúp biết vì sao API có thể không truy cập được (private subnet, routing, security rule).
- **IAM:** IAM quản lý quyền ở phía AWS; frontend dựa vào cơ chế authN/authZ của backend và không được nhúng AWS credential.
- **S3 (static resources):** Xem S3 như nơi phục vụ asset tĩnh cho UI hoặc lưu file để tải về.
- **API Gateway:** Nhìn thấy lợi ích của một endpoint API tập trung cho frontend (routing, throttling, cấu hình CORS thống nhất).
- **Route 53:** Dùng DNS name giúp endpoint ổn định qua các lần deploy, tránh hardcode IP trong frontend.
