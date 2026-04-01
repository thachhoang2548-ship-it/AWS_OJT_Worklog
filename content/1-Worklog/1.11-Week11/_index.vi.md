---
title: "Week 11 Worklog"
date: 2026-03-23
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Trọng tâm của Tuần 11

Trọng điểm tuần này là khâu rà soát tích hợp, đẩy cao hiệu năng, nghiệm thu hạ tầng, và gia cố lớp áo giáp bảo mật (hardening) để ứng dụng hoàn toàn sẵn sàng ra trận trên môi trường production.

- **Kiểm định Chéo (Integration Testing)**:
  - Khởi chạy các kịch bản test end-to-end trên toàn bộ nền tảng.
  - Thẩm định luồng thông tin chạy giữa các vi mạch chức năng.
  - Vá kịp thời các kẽ hở phát sinh khi ráp nối.

- **Ép xung Hiệu năng**:
  - Gọt giũa lại các câu lệnh truy vấn DB và khối logic xử lý chậm.
  - Kéo giảm độ trễ, tăng vọt ngưỡng chịu tải của server.
  - Tối ưu hóa việc ngốn RAM/CPU.

- **Nghiệm thu Hạ tầng Đám mây**:
  - Check lại toàn bộ thông số trên máy ảo EC2, RDS, S3.
  - Khẳng định khả năng phình to (scale) và độ liền mạch.
  - Diễn tập kịch bản sập nguồn và tự phục hồi (failover).

- **Gia cố Bảo mật Production**:
  - Ốp chuẩn các tiêu chuẩn bảo mật khắt khe nhất.
  - Khóa kín các biến môi trường và chìa khóa (secrets).
  - Thắt chặt quyền ra vào cổng và bung rộng khả năng ghi log.

---

### Chi tiết nhiệm vụ

| Ngày | Chi tiết công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
|:----:|--------------------|:-------:|:----------:|----------------|
|  2   | **Tích hợp & Test**:<br>- Quét E2E rà soát lỗi<br>- Duyệt lại luồng dữ liệu | 23/03/2026 | 24/03/2026 | Nội bộ |
|  3   | **Fix Lỗi**:<br>- Xử lý ngẽn cổ chai<br>- Đưa app về trạng thái ổn định | 25/03/2026 | 26/03/2026 | Nội bộ |
|  4   | **Tối ưu Tốc độ**:<br>- Tune lại Query<br>- Ép thời gian phản hồi | 27/03/2026 | 28/03/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  5   | **Chốt Hạ tầng**:<br>- Kiểm duyệt Service AWS<br>- Giả lập tải thực tế | 29/03/2026 | 30/03/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  6   | **Thắt chặt An ninh**:<br>- Áp rule bảo mật<br>- Bật tool cào log | 31/03/2026 | 01/04/2026 | Security Docs |

---

### Thành quả Tuần 11

#### Cột mốc đạt được

- Chạy thông thạo quy trình **kiểm thử tích hợp cặn kẽ** mọi ngóc ngách.
- Tiêu diệt các bug nghiêm trọng nhất, trả lại sự mượt mà cho hệ thống.
- Ép xung thành công dàn Backend và trạm dữ liệu RDS.
- Dán tem chất lượng cho dàn cấu hình **hạ tầng cloud**.
- Đắp thêm **lớp giáp bảo mật tiêu chuẩn Production**.
- Đưa hệ thống vào vạch xuất phát, đợi lệnh là có thể Go-live.

#### Định hướng Kiến trúc

- **Lớp Kiểm định (QA)**: Đánh trận giả E2E và Tích hợp.
- **Chỉ số Tốc độ**: Tối giản hóa thời gian tiêu hao của DB & Backend.
- **Khung Hạ tầng**: AWS (EC2, RDS, S3) đã kinh qua sát hạch.
- **Tiêu chuẩn An ninh**: Hardening triệt để, Log chi tiết, Ẩn Config tốt.
- **Giai đoạn (Phase)**: Pre-production / Đóng gói chờ cất cánh.
