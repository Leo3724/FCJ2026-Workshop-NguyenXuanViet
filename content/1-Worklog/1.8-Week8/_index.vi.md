---
title: "Worklog Tuần 8"
date: 2026-03-02
weight: 8
chapter: false
pre: "<b>1.8. </b>"
---

### Mục tiêu tuần 8

- Phát triển và tích hợp các tính năng frontend với backend API được triển khai trên AWS EC2.
- Thực hành xử lý các vấn đề khi tích hợp API từ phía frontend như CORS và xác thực.
- Hiểu quy trình nghiệp vụ của vai trò Manager để hỗ trợ phát triển UI.
- Cải thiện hiểu biết về cách frontend tương tác với các thành phần hạ tầng AWS.

### Các công việc cần triển khai trong tuần này

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
|-----|----------|------------|-----------------|---------------------|
| 2-4 | - Phát triển giao diện frontend và tích hợp với backend API.<br>- Kiểm thử phản hồi API và xử lý ngoại lệ.<br>- Điều chỉnh UI theo cấu trúc dữ liệu từ backend. | 03/02/2026 | 04/02/2026 | Tài liệu nội bộ, đặc tả API |
| 5 | - Xử lý lỗi CORS giữa frontend và backend.<br>- Triển khai luồng đăng nhập và xử lý token từ backend API.<br>- Kiểm tra kết nối sau khi backend được triển khai trên EC2. | 05/02/2026 | 05/02/2026 | Tài liệu backend, tham khảo JWT |
| 6 | - Tìm hiểu quy trình nghiệp vụ của vai trò Manager.<br>- Triển khai các màn hình/chức năng frontend tương ứng.<br>- Kiểm thử user flow theo yêu cầu nghiệp vụ. | 06/02/2026 | 06/02/2026 | Tài liệu yêu cầu nghiệp vụ |

### Kết quả đạt được tuần 8

- Phát triển thành công các chức năng frontend và tích hợp với backend API chạy trên AWS EC2.
- Có kinh nghiệm thực tế trong việc xử lý các vấn đề khi tích hợp API như lỗi CORS và lỗi xác thực.
- Hiểu rõ hơn cách frontend giao tiếp với các dịch vụ backend có kết nối tới Amazon RDS.
- Hiểu vai trò của các thành phần hạ tầng AWS hỗ trợ hệ thống:
  - VPC: phục vụ kết nối mạng giữa các dịch vụ.
  - IAM: quản lý quyền truy cập.
  - S3: lưu trữ tài nguyên tĩnh (nếu có).
  - API Gateway: quản lý các API endpoint.
  - Route 53: cấu hình định tuyến domain.
- Hoàn thành phát triển UI cho các tính năng của Manager dựa trên luồng nghiệp vụ.
- Cải thiện kỹ năng debug khi xử lý các vấn đề liên quan đến kết nối API sau khi triển khai.
- Biết cách kiểm thử API bằng browser developer tools và Postman song song với quá trình tích hợp frontend.
