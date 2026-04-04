---
title: "Worklog Tuần 2"
date: 2026-01-11
weight: 2
chapter: false
pre: "<b>1.2. </b>"
---

### Mục tiêu tuần 2

- Hoàn thành Module 2, tập trung vào việc hiểu EC2 và VPC.
- Chuẩn bị các tài nguyên cần thiết để khởi tạo một EC2 instance.
- Tìm hiểu Route 53 và các khái niệm liên quan.

### Các công việc cần triển khai trong tuần này

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | - Đào sâu kiến thức về VPC và các dịch vụ/tài nguyên liên quan.<br>- Tìm hiểu các nguyên tắc thiết kế kiến trúc trên AWS.<br>- Ôn lại các kiến thức từ bài giảng của Mentor Gia Hung. | 11/01/2026 | 12/01/2026 | [THAM KHẢO](https://cloudjourney.awsstudygroup.com/) |
| 2 | - Tạo các tài nguyên trong VPC để chuẩn bị cho việc tạo EC2 instance.<br>- Khởi tạo EC2 instance bằng các tài nguyên đã chuẩn bị.<br>- Tìm hiểu Security Group và Network ACL. | 12/01/2026 | 13/01/2026 | [THAM KHẢO](https://docs.aws.amazon.com/ec2/) |
| 3 | - Xử lý vấn đề xác thực tài khoản AWS và gửi các tài liệu xác minh cần thiết. | 13/01/2026 | 16/01/2026 | [THAM KHẢO](https://aws.amazon.com/support/) |
| 4 | - Tham gia sự kiện Cloud Day.<br>- Cập nhật thêm kiến thức về AI và Data thông qua sự kiện.<br>- Kết nối với các mentor nổi bật. | 14/01/2026 | 14/01/2026 | |

### Kết quả đạt được tuần 2

- Nắm được kiến thức nền tảng về VPC và EC2, bao gồm các khái niệm và cấu hình cốt lõi.
- Hiểu các bước và tài nguyên cần thiết để khởi tạo một EC2 instance.
- Đã tạo và cấu hình thành công các tài nguyên thiết yếu để thiết lập EC2, bao gồm:
  - Subnet để phân tách mạng.
  - Internet Gateway để kết nối ra bên ngoài.
  - Quy tắc Route Table để quản lý định tuyến lưu lượng.
  - Security Group để kiểm soát lưu lượng vào và ra cho EC2 instance.
- Đã xử lý vấn đề xác thực tài khoản AWS bằng cách gửi tài liệu xác minh.
- Tham gia sự kiện Cloud Day, mở rộng kết nối với mentor và nhận được nhiều chia sẻ hữu ích.
- Nâng cao hiểu biết về AI và Data, bao gồm nhu cầu thị trường hiện tại và tiềm năng phát triển của AI trong tương lai.

- **VPC:** Hiểu ranh giới mạng và rule (SG/NACL) có thể chặn API dù code frontend đúng.
- **IAM:** Quyền nằm ở IAM (role/policy). Frontend thường xác thực bằng token/cookie do backend cấp, không dùng AWS access key.
- **S3 (static resources):** Biết cách tài nguyên tĩnh có thể được phân phối qua S3 (phục vụ asset hoặc file download cho UI).
- **API Gateway:** Hiểu cách frontend có thể gọi một API endpoint được quản lý tập trung (routing + xử lý CORS).
- **Route 53:** Ưu tiên cấu hình API URL theo domain (ổn định, dễ đổi môi trường) thay vì nhúng IP.
