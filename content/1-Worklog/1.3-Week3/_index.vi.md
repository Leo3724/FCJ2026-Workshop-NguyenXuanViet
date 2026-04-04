---
title: "Worklog Tuần 3"
date: 2026-01-18
weight: 3
chapter: false
pre: "<b>1.3. </b>"
---

### Mục tiêu tuần 3

- Khắc phục các vấn đề liên quan đến tài khoản AWS và tạo tài khoản thay thế khi cần.
- Tìm hiểu cách triển khai Hybrid DNS bằng Route 53 Resolver.
- Thực hành cấu hình VPC Peering để các VPC có thể giao tiếp với nhau.
- Đồng bộ với các thành viên trong nhóm về hướng dự án và công nghệ sử dụng.

### Hoạt động trong tuần

| Ngày | Công việc                                                                                                                                                                          | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
| --- |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------| --- | --- | --- |
| 1 | - Đăng ký thẻ Visa mới.<br>- Tạo thêm một tài khoản AWS và hoàn tất cấu hình cơ bản.                                                                                               | 18/01/2026 | 20/01/2026 | [THAM KHẢO](https://aws.amazon.com/getting-started/) |
| 2 | - Hoàn thành Lab 10 tập trung vào Route 53.<br>- Cấu hình Hybrid DNS bằng Route 53 Resolver.<br>- Triển khai một máy ảo để kiểm thử cấu hình DNS.                                  | 21/01/2026 | 22/01/2026 | [THAM KHẢO](https://youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&si=NtlkPHvTydrkH4rK) |
| 3 | - Triển khai VPC Peering để kết nối nhiều mạng VPC.<br>- Chuẩn bị các tài nguyên hỗ trợ cho kết nối peering.<br>- Dọn dẹp các tài nguyên không còn sử dụng sau khi hoàn thành lab. | 22/01/2026 | 23/01/2026 | [THAM KHẢO](https://youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&si=NtlkPHvTydrkH4rK) |
| 4 | - Tham gia buổi thảo luận với nhóm.<br>- Chốt ngôn ngữ lập trình chính và phân công nhiệm vụ học tập cho từng thành viên.                                                          | 25/01/2026 | 25/01/2026 | |

### Kết quả đạt được tuần 3

- Đã đăng ký thành công tài khoản AWS mới và hoàn tất cấu hình ban đầu để tiếp tục các hoạt động dự án cùng nhóm FCJ.
- Nắm rõ hơn về Route 53 và cấu hình Hybrid DNS, bao gồm:
  - Tạo và cấu hình Route 53 Resolver Outbound Endpoints.
  - Thiết lập Inbound Endpoints cho quá trình phân giải DNS.
  - Kiểm thử kết nối thông qua RD Gateway Server.
- Hiểu được cách VPC Peering cho phép giao tiếp nội bộ an toàn giữa các VPC mà không đi qua internet công cộng.
- Thực hành triển khai hạ tầng bằng AWS CloudFormation templates.
- Nắm được cách bật Cross-Zone và Cross-Region DNS Resolution cho VPC Peering:
  - Giúp EC2 ở các VPC khác nhau phân giải private DNS chính xác.
  - Hiểu rằng nếu không cấu hình, truy vấn DNS có thể trả về public IP làm luồng dữ liệu đi ra khỏi mạng private.
- Tham gia các buổi họp kế hoạch dự án, thống nhất công nghệ sử dụng và lộ trình học của các thành viên.

- **Route 53:** Củng cố việc frontend nên trỏ đúng domain public của API (tránh dùng private DNS name hoặc IP).
- **VPC:** Hiểu việc thiết kế private networking ảnh hưởng việc service có public access hay chỉ chạy trong VPC.
- **API Gateway:** Nếu dùng, API Gateway là điểm vào public mà frontend gọi tới, dù backend/service nằm private subnet.
- **IAM:** IAM bảo vệ tài nguyên AWS ở phía backend; frontend truy cập qua HTTP API đã được bảo vệ (JWT/cookie).
- **S3 (static resources):** S3 có thể serve document/asset cho frontend qua URL, trong khi backend vẫn giữ private.
