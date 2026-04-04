---
title: "Worklog Tuần 9"
date: 2026-03-10
weight: 9
chapter: false
pre: "<b>1.9. </b>"
---

### Mục tiêu tuần 9

- Tiếp tục phát triển các tính năng frontend và tích hợp với backend API được triển khai trên AWS EC2.
- Refactor các UI component để tăng khả năng bảo trì và hiệu năng.
- Khắc phục các lỗi tích hợp giữa frontend và backend sau khi triển khai.
- Cải thiện hiểu biết về cách frontend tương tác với các dịch vụ AWS trong kiến trúc dự án.

---

### Các công việc cần triển khai trong tuần này

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
|-----|----------|------------|-----------------|---------------------|
| 2 | - Tìm hiểu cấu trúc API do backend cung cấp.<br>- Cập nhật frontend component theo cấu trúc response từ API.<br>- Refactor các component có thể tái sử dụng. | 10/03/2026 | 10/03/2026 | Tài liệu nội bộ, đặc tả API |
| 3 | - Phát triển các màn hình CRUD (Create, Read, Update, Delete) cho các chức năng quản trị hệ thống.<br>- Kết nối các form frontend với backend API.<br>- Xử lý validate và hiển thị thông báo lỗi. | 11/03/2026 | 12/03/2026 | Tài liệu dự án |
| 4 | - Debug các lỗi tích hợp giữa frontend và backend.<br>- Khắc phục lỗi CORS và sai endpoint API.<br>- Kiểm thử các tính năng sau khi backend được deploy trên EC2. | 12/03/2026 | 13/03/2026 | Tài liệu AWS EC2, công cụ test API |
| 5 | - Cải thiện trải nghiệm UI và điều chỉnh layout dựa trên phản hồi.<br>- Tối ưu các API call để giảm request không cần thiết.<br>- Cải thiện xử lý lỗi trên frontend. | 13/03/2026 | 14/03/2026 | Tài liệu React |
| 6 | - Kiểm thử hệ thống sau khi triển khai.<br>- Xác minh kết nối frontend với các dịch vụ backend.<br>- Kiểm thử truy cập domain qua Route 53 (nếu áp dụng). | 14/03/2026 | 14/03/2026 | Tài liệu AWS |

---

### Kết quả đạt được tuần 9

- Hoàn thành một số giao diện CRUD frontend và tích hợp với backend API chạy trên AWS EC2.
- Cải thiện cấu trúc code bằng cách refactor các React component dùng chung.
- Khắc phục các lỗi tích hợp ảnh hưởng tới việc frontend giao tiếp với backend.
- Hiểu rõ hơn về kiến trúc hệ thống, bao gồm:
  - EC2: nơi chạy backend.
  - RDS: cơ sở dữ liệu của hệ thống (frontend truy cập thông qua API).
  - VPC: hạ tầng mạng.
  - IAM: khái niệm quản lý quyền.
  - Route 53: định tuyến domain.
- Cải thiện kỹ năng debug khi frontend không kết nối được tới backend sau khi deploy.
- Tối ưu các API call và cải thiện xử lý lỗi để nâng cao trải nghiệm người dùng.
- Kiểm thử các tính năng sau khi triển khai để đảm bảo độ ổn định của hệ thống.

---

### Tổng kết tuần 9

- Hoàn thành phát triển một số tính năng quan trọng cho frontend.
- Nâng chất lượng code frontend thông qua refactor.
- Tích hợp thành công frontend với backend đã triển khai.
- Có thêm kinh nghiệm thực tế khi làm việc với kiến trúc hệ thống trên cloud.
- Hiểu rõ hơn cách một frontend developer phối hợp với backend và hạ tầng cloud trong dự án.
