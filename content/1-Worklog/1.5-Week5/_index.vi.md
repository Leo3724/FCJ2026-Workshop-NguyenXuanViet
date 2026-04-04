---
title: "Worklog Tuần 5"
date: 2026-02-02
weight: 5
chapter: false
pre: "<b>1.5. </b>"
---

## Mục tiêu tuần 5

- Rà soát và làm rõ các nguyên nhân khiến chi phí AWS phát sinh chưa hợp lý.
- Xây dựng phương án kiến trúc hạ tầng và phân tách thành phần cho dự án.
- Khởi động bước cấu hình ban đầu, đồng thời phân chia trách nhiệm cho các thành viên.

## Các công việc cần triển khai trong tuần này

| STT | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 1 | - Phân tích các khoản chi bất thường trên tài khoản AWS và xác định nguyên nhân chính. | 02/02/2026 | 03/02/2026 | [Tham khảo tại đây](https://aws.amazon.com/aws-cost-management/aws-cost-explorer/) |
| 2 | - Thiết kế kiến trúc hạ tầng cho dự án và chia tách các khối chức năng.<br>- Đề xuất một số mẫu kiến trúc nền tảng để nhóm dễ đối chiếu và lựa chọn. | 04/02/2026 | 05/02/2026 | [Tham khảo tại đây](https://www.facebook.com/groups/awsstudygroupfcj) |
| 3 | - Dựng bộ khung mã nguồn (code skeleton) và cấu hình các tệp khởi tạo cần thiết cho dự án. | 06/02/2026 | 08/02/2026 | |

## Kết quả đạt được tuần 5

- Hoàn tất bản thiết kế kiến trúc hạ tầng và đưa ra các mẫu tham khảo phù hợp để nhóm triển khai.
- Xây dựng thành công code skeleton cùng bộ cấu hình ban đầu, tạo nền tảng ổn định cho các bước tiếp theo.
- Đăng ký và kích hoạt tài khoản AWS Skill Builder, bắt đầu tiếp cận hệ thống khóa học và tài liệu liên quan.
- Làm rõ nguyên nhân của chi phí bất thường: tài nguyên EC2 chưa được dọn dẹp triệt để và tài khoản người dùng còn thiếu kiểm soát; từ đó đề xuất hướng tối ưu chi phí.

- **VPC:** Hiểu backend có thể chạy trong private network; frontend chỉ nên gọi qua endpoint public đã được expose, không dùng private IP.
- **IAM:** Xác định ranh giới quyền: IAM role/policy bảo vệ tài nguyên AWS; frontend dùng token/cookie do backend cấp để gọi API.
- **S3 (static resources):** Dự kiến dùng S3 để lưu/serve tài nguyên tĩnh (ảnh, file build) để UI tải qua URL.
- **API Gateway:** Nếu áp dụng, API Gateway sẽ là endpoint tập trung để frontend gọi (routing + CORS tập trung).
- **Route 53:** Dùng domain cho URL frontend/API để tránh hardcode IP và hỗ trợ chuyển môi trường.
