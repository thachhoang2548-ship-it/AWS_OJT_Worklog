---
title: "Week 13 Worklog"
date: 2026-04-06
weight: 13
chapter: false
pre: " <b> 1.13. </b> "
---

### Trọng tâm của Tuần 13

Tuần cuối cùng xoay quanh các nhiệm vụ hậu go-live (Day-2 Operations): trực chiến theo dõi tình trạng server, siết lại hiệu năng, vá lỗ hổng nhỏ và lắng nghe tiếng nói của những tập khách hàng đầu tiên.

- **Trực chiến Giám sát**:
  - Để mắt liên tục tới các chỉ số sức khỏe và thời gian uptime.
  - Đọc log hệ thống hàng ngày để phát hiện mầm mống lỗi.
  - Cam kết hệ thống không sập tải khi User thật tràn vào.

- **Siết mượt Hiệu năng**:
  - Tút tát lại mớ câu lệnh query và giảm tải cho API.
  - Tối ưu hóa thời gian load trang bên phía Frontend.
  - Kéo độ phản hồi tĩnh/động xuống mức lý tưởng nhất.

- **Vá Bug và Cải tiến Nhỏ**:
  - Tiếp nhận và xử lý nóng những vấn đề do User phản ánh.
  - Xoay trục thiết kế UX/UI cho thuận với thói quen người dùng thực tế.
  - Gọn gàng hóa các đoạn code cũ (Refactor) để dễ bề bảo trì.

- **Lắng nghe Phản hồi (Feedback)**:
  - Gom nhặt những review từ những người dùng trung thành đầu tiên.
  - Diễn dịch mô hình luồng thao tác của User.
  - Phác mâm cỗ tính năng ưu tiên để nạp vào Sprint sắp tới.

---

### Chi tiết nhiệm vụ

| Ngày | Chi tiết công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
|:----:|--------------------|:-------:|:----------:|----------------|
|  2   | **Khám sức khỏe App**:<br>- Lọc Log truy cập<br>- Check độ ổn định Live | 06/04/2026 | 06/04/2026 | CloudWatch |
|  3   | **Ép xung Ứng dụng**:<br>- Rút ngắn tốc độ Query<br>- Thông nòng API | 07/04/2026 | 08/04/2026 | Nội bộ |
|  4   | **Dọn Bug**:<br>- Sửa lỗi khẩn cấp<br>- Gọt lại dăm ba màn hình | 09/04/2026 | 10/04/2026 | Nội bộ |
|  5   | **Nghiên cứu Thị hiếu**:<br>- Lấy Feedback<br>- Đo lường Data thực | 11/04/2026 | 11/04/2026 | Nội bộ |
|  6   | **Lên Bản đồ V-Next**:<br>- Gọi tên loạt nâng cấp mới<br>- Ghi Roadmap cho App | 12/04/2026 | 12/04/2026 | Nội bộ |

---

### Thành quả Tuần 13

#### Cột mốc đạt được

- Chăm sóc tốt cơ sở hạ tầng sau sự kiện **bấm nút Go-live**.
- Săn và tiêu diệt loạt bug "cỏ" bị phát hiện bởi người dùng.
- Trả về kết quả vượt trội ở khoản chịu tải và bức tốc truy vấn.
- Giao diện được o bế trở nên mượt mà, chiều lòng người xài hơn.
- Thu thập một rổ dữ liệu đáng giá phục vụ cho các bản vá sau này.
- Hình thành bộ quy chuẩn vận hành (Ops Workflow) vững vàng.

#### Định hướng Kiến trúc

- **Trạng thái (Phase)**: Duy trì Sự sống (Maintenance) / Hậu Go-Live.
- **Canh gác (Monitoring)**: Trực hệ thống 24/7 (Log, Mốc metric, Báo động).
- **Trùng tu (Optimization)**: Bảo dưỡng sức mạnh cốt lõi.
- **Trọng lực Phát triển**: User trải nghiệm → Góp ý hòm thư → Product nâng cấp → Ra mắt tính năng mới.
- **Tổng Kết**: Chạy êm, ổn định, tiềm năng phình to vô cực.