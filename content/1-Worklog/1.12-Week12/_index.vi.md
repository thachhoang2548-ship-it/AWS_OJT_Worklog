---
title: "Worklog Tuần 12"
date: 2026-03-30
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Trọng tâm của Tuần 12

Tâm điểm của tuần này là đưa "đứa con tinh thần" lên sàn đấu production, mắc các thiết bị theo dõi sinh tồn của hệ thống, và dọn đường để chính thức đón làn sóng người dùng đầu tiên.

- **Lên sóng Production**:
  - Vận chuyển toàn bộ module lên hạ tầng thật (live).
  - Trỏ tên miền (domain) và thiết lập mạng lưới cloud.
  - Kích hoạt app và rà soát độ tĩnh tâm của máy chủ.

- **Lắp đặt Trạm gác (Monitoring)**:
  - Giăng bẫy cảnh báo (alerts) và tool theo dõi (monitoring).
  - Bơm log ứng dụng tập trung về một mối để dễ mổ xẻ.
  - Dựng các bảng điều khiển (dashboard) chớp nháy số liệu thời gian thực.

- **Sẵn sàng Nhấn nút**:
  - Chạy kịch bản tổng kiểm tra trước giờ G.
  - Soạn thảo và bàn giao bộ cẩm nang vận hành (playbooks).
  - Khai thông luồng phục vụ User thực chiến.

---

### Chi tiết nhiệm vụ

| Ngày | Chi tiết công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
|:----:|--------------------|:-------:|:----------:|----------------|
|  2   | **Đưa App lên Live**:<br>- Deploy mã nguồn thật<br>- Chỉnh biến môi trường live | 30/03/2026 | 31/03/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  3   | **Chốt dịch vụ Cloud**:<br>- Trỏ DNS Domain<br>- Gõ thử các API live | 01/04/2026 | 02/04/2026 | Nội bộ |
|  4   | **Dựng Radar theo dõi**:<br>- Nhúng CloudWatch Log<br>- Đặt mốc báo động (Alerts) | 03/04/2026 | 04/04/2026 | CloudWatch |
|  5   | **Rà quét lần cuối (UAT)**:<br>- Check luồng hoạt động<br>- Ký nghiệm thu nội bộ | 05/04/2026 | 06/04/2026 | Nội bộ |
|  6   | **Thủ tục Bàn giao**:<br>- Làm Docs vận hành<br>- Sang tên bộ máy | 07/04/2026 | 08/04/2026 | Nội bộ |

---

### Thành quả Tuần 12

#### Cột mốc đạt được

- Kéo quân an toàn lên **môi trường Production**.
- Cắm mắt thành công **trạm gác giám sát và cảnh báo tự động**.
- Đạt chứng nhận ổn định khi chạy trên nền tải thật.
- Khép lại chuỗi ngày UAT bằng các chữ ký nghiệm thu.
- Trao tay bộ hành trang tài liệu vận hành cho đội Ops.
- Toàn bộ cơ ngơi đã khoác áo **Sẵn sàng Go-live**.

#### Định hướng Kiến trúc

- **Đích đến**: Cụm máy chủ Production tiêu chuẩn.
- **Trạm quan sát**: Metric chỉ số, Log trung tâm, Chuông báo động.
- **Hành trang**: Tài liệu hướng dẫn & Quy trình bàn giao.
- **Hướng di chuyển**: Dòng User → Cụm Máy Chủ → Tool Giám Sát → Admin.
- **Giai đoạn (Phase)**: Bấm còi / Chính thức đi vào đời sống.
