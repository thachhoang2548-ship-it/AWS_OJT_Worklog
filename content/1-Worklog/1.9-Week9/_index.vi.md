---
title: "Worklog Tuần 9"
date: 2026-03-09
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Trọng tâm của Tuần 9

Tuần này dồn sức vào công tác đưa ứng dụng lên môi trường staging (chạy thử), kiểm thử toàn diện và khắc phục các vấn đề phát sinh trong lúc ráp nối các module.

- **Đưa Ứng dụng lên Mây (Deployment)**:
  - Triển khai source code lên máy chủ Amazon EC2 thực.
  - Khai báo cấu hình nối với RDS, S3 và bản đồ AWS.
  - Xác nhận tín hiệu thông suốt giữa các block kiến trúc.

- **Kiểm định Chất lượng (Testing)**:
  - Chạy thử nghiệm các kịch bản người dùng (user flows).
  - Rà soát mức độ thân thiện của giao diện UX/UI.
  - Bắt mạch luồng dữ liệu truyền tải giữa Frontend và Backend.

- **Truy vết và Sửa lỗi (Fixing & Tuning)**:
  - Xử lý triệt để các bug được report trong quá trình test.
  - Sắp xếp lại code (refactor) để bịt các lỗ hổng tiềm ẩn.
  - Đẩy nhanh tốc độ xử lý ở những điểm thắt cổ chai.

- **Nghiệm thu Hệ thống**:
  - Đảm bảo app chạy trơn tru không sập nguồn.
  - Chốt hạ phiên bản phần mềm để chuẩn bị cho buổi demo nghiệm thu.

---

### Chi tiết nhiệm vụ

| Ngày | Chi tiết công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
|:----:|--------------------|:-------:|:----------:|----------------|
|  2   | **Setup Deployment**:<br>- Đưa code lên EC2<br>- Khai báo biến môi trường | 09/03/2026 | 09/03/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  3   | **Kiểm thử E2E**:<br>- Test nghiệp vụ chính<br>- Theo dõi data flow | 10/03/2026 | 10/03/2026 | Internal |
|  4   | **Sửa Bug**:<br>- Check log hệ thống<br>- Vá lỗi phần mềm | 11/03/2026 | 11/03/2026 | Internal |
|  5   | **Tối ưu Hóa**:<br>- Refactor mã nguồn<br>- Cải thiện tốc độ phản hồi | 12/03/2026 | 12/03/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  6   | **Nghiệm thu**:<br>- Chạy rà soát tổng thể<br>- Đóng gói bản demo | 13/03/2026 | 13/03/2026 | Internal |

---

### Thành quả Tuần 9

#### Cột mốc đạt được

- Chuyển giao thành công ứng dụng lên máy ảo **Amazon EC2**.
- Chốt chặt kết nối với các cỗ máy phụ trợ của AWS:
  - Mỏ dữ liệu **Amazon RDS**
  - Kho tệp tin **Amazon S3**
  - Dịch vụ định vị **AWS Map**
- Quét qua toàn bộ vòng đời sử dụng (end-to-end testing) của tính năng lõi.
- Xóa bỏ hàng loạt lỗi phần mềm tìm thấy trong khâu QA.
- Trải nghiệm người dùng và sức mạnh hệ thống được nâng cấp rõ rệt.
- Trạng thái sản phẩm hiện tại: **Trực chiến, sẵn sàng Demo**.

#### Định hướng Kiến trúc

- **Máy trạm (Compute)**: Dùng EC2 chạy gốc.
- **Dữ liệu (DB)**: Dùng RDS bản SQL Server.
- **Tập tin (Storage)**: Đẩy về bucket S3.
- **Tiện ích bản đồ (Location)**: Tích hợp AWS Map.
- **Đường truyền (Data Flow)**: UI phía Frontend → Logic Backend → Hạ tầng AWS.
- **Giai đoạn (Phase)**: Kiểm thử / Chuẩn bị mồi (Pre-production).
