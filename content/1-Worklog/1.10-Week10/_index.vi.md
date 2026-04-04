---
title: "Worklog Tuần 10"
date: 2026-03-16
weight: 10
chapter: false
pre: "<b>1.10. </b>"
---

### Mục tiêu tuần 10

- Ổn định việc tích hợp frontend với backend API được triển khai trên AWS EC2.
- Tập trung xử lý các vấn đề tích hợp như CORS, xác thực và kết nối API.
- Tiếp tục phát triển và kiểm thử các tính năng frontend như Read và Delete.
- Cải thiện hiểu biết về quy trình triển khai và kiểm thử hệ thống sau khi tích hợp.
- Tham gia trao đổi kỹ thuật với các thành viên để xử lý các vấn đề của dự án.

---

### Các công việc cần triển khai trong tuần này

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
|-----|----------|------------|-----------------|---------------------|
| 2 | - Debug lỗi CORS ảnh hưởng tới request API từ frontend.<br>- Kiểm tra API endpoint và response header.<br>- Test kết nối frontend sau khi backend cập nhật. | 16/03/2026 | 16/03/2026 | Tài liệu API, tài liệu AWS EC2 |
| 3 | - Cải thiện chức năng Read (UI hiển thị danh sách dữ liệu).<br>- Đảm bảo dữ liệu từ backend API hiển thị đúng trên giao diện.<br>- Xử lý loading state và thông báo lỗi. | 17/03/2026 | 17/03/2026 | Tài liệu nội bộ dự án |
| 4 | - Tiếp tục tích hợp frontend với backend API đã deploy.<br>- Test các thao tác CRUD từ giao diện người dùng.<br>- Hiển thị dữ liệu hệ thống thành công trên web. | 18/03/2026 | 18/03/2026 | Mã nguồn frontend |
| 5 | - Triển khai và kiểm thử chức năng Delete từ frontend.<br>- Debug các lỗi liên quan xác thực khi gọi API có bảo vệ.<br>- Kiểm tra validate request và quyền truy cập. | 19/03/2026 | 19/03/2026 | Công cụ test API |
| 6 | - Tham gia thảo luận kỹ thuật cùng các thành viên.<br>- Rà soát các lỗi tích hợp còn tồn đọng.<br>- Áp dụng hướng xử lý được đề xuất và retest các tính năng bị ảnh hưởng. | 20/03/2026 | 20/03/2026 | Trao đổi trong nhóm |

---

### Kết quả đạt được tuần 10

- Khắc phục thành công một số lỗi tích hợp frontend liên quan đến CORS và kết nối API.
- Hoàn thành tích hợp frontend với các dịch vụ backend được triển khai trên AWS EC2.
- Triển khai thành công chức năng Read (hiển thị dữ liệu) và Delete (xóa dữ liệu) trên giao diện web.
- Hiểu rõ hơn về luồng xác thực giữa frontend và backend.
- Xác định và phân tích một số vấn đề kỹ thuật quan trọng như:
  - Lỗi xác thực khi gọi các API được bảo vệ.
  - Response API không đúng làm ảnh hưởng hiển thị trên frontend.
  - Sự cố kết nối liên quan quá trình triển khai.
- Hiểu thêm về các thành phần hạ tầng AWS hỗ trợ hệ thống:
  - EC2: nơi chạy backend.
  - RDS: cơ sở dữ liệu chính (frontend truy cập thông qua API).
  - VPC: hạ tầng mạng an toàn.
  - IAM: khái niệm quản lý quyền.
  - Route 53: định tuyến domain (nếu áp dụng).
- Cải thiện kỹ năng kiểm thử bằng cách xác minh tính năng sau khi triển khai.

---

### Tổng kết tuần 10

- Việc tích hợp giữa frontend và backend trở nên ổn định hơn.
- Các tính năng cốt lõi của frontend đã được kiểm thử thành công trên hệ thống đã triển khai.
- Nâng cao khả năng debug các lỗi phát sinh trong môi trường triển khai thực tế.
- Có thêm kinh nghiệm làm việc với kiến trúc ứng dụng triển khai trên cloud.
- Dự án tiến tới giai đoạn user testing cơ bản với các tính năng frontend đã hoạt động.
