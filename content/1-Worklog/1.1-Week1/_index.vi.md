---
title: "Worklog Tuần 1"
date: 2026-01-05
weight: 1
chapter: false
pre: "<b>1.1. </b>"
---

### Mục tiêu tuần 1

- Kết nối và làm quen với các thành viên của First Cloud Journey (FCJ).
- Hiểu về tổ chức và các dịch vụ AWS cơ bản.

### Các công việc cần triển khai trong tuần này

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | - Tham gia buổi kick-off của FCJ.<br>- Tìm hiểu về tổ chức FCJ.<br>- Thành lập nhóm để cùng thực hiện dự án. | 05/01/2026 | 05/01/2026 | |
| 2 | - Tạo tài khoản AWS.<br>- Tìm hiểu các khái niệm điện toán đám mây.<br>- Vẽ kiến trúc mẫu bằng draw.io. | 06/01/2026 | 06/01/2026 | [THAM KHẢO](https://cloudjourney.awsstudygroup.com/) |
| 3 | - Tìm hiểu mục tiêu của chương trình First Cloud Journey và website AWS.<br>- Thực hiện cấu hình ban đầu trên tài khoản AWS:<br>&emsp;+ Tạo budget.<br>&emsp;+ Tạo user group.<br>&emsp;+ Bật xác thực hai lớp (2FA).<br>- Tìm hiểu AWS Support Center và cách gửi yêu cầu hỗ trợ. | 07/01/2026 | 07/01/2026 | [THAM KHẢO](https://cloudjourney.awsstudygroup.com/) |
| 4 | - Tạo VPC và cấu hình các thiết lập liên quan.<br>- Tạo và cấu hình Subnet (bao gồm public Subnet tự gán public IP).<br>- Thiết lập Internet Gateway và gắn vào VPC.<br>- Tạo và cấu hình Route Table, kết nối với Internet Gateway.<br>- Cấu hình Subnet Associations.<br>- Tạo Security Group (public và private). | 08/01/2026 | 11/01/2026 | [THAM KHẢO](https://cloudjourney.awsstudygroup.com/) |

### Kết quả đạt được tuần 1

- Đã tham gia thành công buổi kick-off FCJ và kết nối với các thành viên trong nhóm.
- Hiểu rõ hơn về tổ chức FCJ và các mục tiêu của chương trình.
- Đã thành lập nhóm để phối hợp thực hiện dự án.
- Đã tạo tài khoản AWS và hoàn thành các bước cấu hình ban đầu:
  - Thiết lập budget để theo dõi chi phí.
  - Tạo user group để quản lý quyền truy cập.
  - Bật xác thực hai lớp (2FA) để tăng cường bảo mật.
- Đã tìm hiểu các khái niệm cơ bản về cloud computing và vẽ thành công kiến trúc mẫu bằng draw.io.
- Đã biết cách sử dụng AWS Support Center và gửi yêu cầu hỗ trợ.
- Đã hoàn thành các hạng mục liên quan đến VPC:
  - Tạo và cấu hình VPC.
  - Thiết lập Subnet, bao gồm public Subnet tự gán public IP.
  - Tạo Internet Gateway và gắn vào VPC.
  - Cấu hình Route Table và kết nối với Internet Gateway.
  - Thiết lập Subnet Associations.
  - Tạo Security Group public và private để kiểm soát truy cập tài nguyên an toàn.

- **VPC:** Hiểu public/private networking và Security Group giúp mình debug vì sao frontend gọi API được/không được (timeout vs lỗi ứng dụng).
- **IAM:** Quyền truy cập AWS được kiểm soát bằng role/policy. Ứng dụng frontend (trình duyệt) không nên chứa AWS key; thay vào đó dùng cơ chế đăng nhập do backend cấp (JWT/session).
- **S3 (static resources):** Làm quen với ý tưởng lưu/serve tài nguyên tĩnh (ảnh, file build) từ S3 thông qua URL.
- **API Gateway:** Hiểu khái niệm “cửa vào API” để frontend gọi vào một endpoint tập trung (và có thể cấu hình CORS tập trung).
- **Route 53:** Hiểu vì sao nên dùng domain ổn định cho frontend/API thay vì hardcode IP.
