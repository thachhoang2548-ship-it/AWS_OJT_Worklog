---
title: "Worklog Tuần 7"
date: 2026-02-24
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Trọng tâm của Tuần 7

Trọng tâm tuần này là xúc tiến việc xây dựng dự án mới, trải dọc từ khâu thiết kế dữ liệu, chốt ý tưởng đến việc phác họa giao diện UI rập khuôn. Song song đó, chúng tôi cũng tham gia một buổi tập huấn chuyên sâu để củng cố kỹ năng giám sát hệ thống (observability) trên AWS.

- **Định hình Sản phẩm**:
  - Gọt giũa lại tầm nhìn và giới hạn tính năng.
  - Lập danh sách các khối chức năng lõi của hệ thống.
  - Chốt sơ đồ kiến trúc tổng thể.

- **Thiết kế Đáy (Database Layer)**:
  - Lập mô hình cơ sở dữ liệu cho sản phẩm.
  - Khai báo cấu trúc bảng, các trường dữ liệu và ràng buộc.
  - Đảm bảo tính mở rộng cho các luồng nghiệp vụ sau này.

- **Giao diện Người dùng (UI)**:
  - Phác họa (wireframe) các màn hình cốt lõi.
  - Chuẩn hóa luồng thao tác (user flow) cho người dùng cuối.
  - Tạo tiền đề cho team Frontend tiến hành viết code.

- **Lớp học Thực chiến (Workshop)**:
  - Đồng hành cùng sự kiện **Building Full-Stack Observability on AWS with Datadog**.
  - Thực hành thu thập metrics, logs và traces trực tiếp trên hạ tầng AWS.
  - Mở mang tư duy về Observability cho kiến trúc phân tán.

---

### Chi tiết nhiệm vụ

| Ngày | Chi tiết công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
|:----:|--------------------|:-------:|:----------:|----------------|
|  2   | **Chốt hạ ý tưởng**:<br>- Tinh chỉnh concept<br>- Giới hạn scope và chốt kiến trúc | 24/02/2026 | 24/02/2026 | Internal |
|  3   | **Xây Database**:<br>- Thiết kế schema<br>- Quy định các bảng và khóa liên kết | 25/02/2026 | 25/02/2026 | Personal Notes |
|  4   | **Phác thảo UX/UI**:<br>- Lên wireframe<br>- Tạo luồng trải nghiệm khách hàng | 26/02/2026 | 26/02/2026 | Figma / Internal |
|  5   | **Thực hành Giám sát**:<br>- Dự Workshop Datadog<br>- Trải nghiệm giám sát metrics/logs/traces | 27/02/2026 | 27/02/2026 | Event |

---

### Thành quả Tuần 7

#### Cột mốc đạt được

- Chốt phương án **triển khai và giới hạn chức năng** một cách gãy gọn.
- Tạo xong bộ khung **thiết kế cơ sở dữ liệu** làm gốc rễ cho dự án.
- Hoàn tất bộ **wireframe giao diện** và luồng tương tác người dùng.
- Tiếp thu thêm nhiều kỹ năng về **Observability trên nền AWS**.
- Tích lũy kinh nghiệm từ workshop thực tế về các mảng:
  - Metrics (Số đo hiệu năng)
  - Logs (Ghi chú hệ thống)
  - Traces (Theo vết phân tán)
  - Root cause analysis (Truy vết lỗi tận gốc)

#### Định hướng Kiến trúc

- **Quản lý Dự án**: Làm rõ scope, mô tả chức năng và toàn cảnh hệ thống.
- **Lớp Dữ liệu**: Tổ chức schema và sự ràng buộc giữa các thực thể.
- **Lớp Hiển thị**: Đóng gói wireframe định hướng trải nghiệm.
- **Lớp Giám sát**: Áp dụng chuẩn Observability tân tiến qua Datadog.