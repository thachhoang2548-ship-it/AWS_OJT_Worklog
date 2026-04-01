---
title: "Worklog Tuần 10"
date: 2026-03-16
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Trọng tâm của Tuần 10

Giai đoạn này được dành riêng để rèn giũa các nghiệp vụ khó, chẳng hạn như bộ máy tính điểm thưởng, cơ chế bắt vi phạm, và chốt chặn bảo mật phân quyền nhằm thắt chặt khâu vận hành.

- **Bộ máy Điểm thưởng**:
  - Thuật toán hóa các quy tắc cộng/trừ điểm.
  - Gài cắm event thưởng điểm vào các tương tác của khách hàng.
  - Đối soát chặt chẽ để dữ liệu ví điểm không bị sai lệch.

- **Cơ chế Bắt lỗi & Phạt**:
  - Viết logic tự động phát hiện hành vi sai chuẩn.
  - Ban hành chế tài xử lý tương ứng với từng mức độ vi phạm.
  - Dựng trang quản trị trực quan để admin vào gõ búa.

- **Kiểm soát Truy cập (RBAC)**:
  - Thiết lập hàng rào bảo vệ người dùng theo chức danh (Role-Based).
  - Khoanh vùng quyền hạn của từng nhóm đối tượng cụ thể.
  - Chặn đứng các hành vi vượt rào vào những tính năng nhạy cảm.

- **Đánh bóng Mã nguồn**:
  - Luân chuyển logic nghiệp vụ sao cho hợp lý nhất.
  - Đảm bảo app chạy bền và dễ mở rộng về sau.

---

### Chi tiết nhiệm vụ

| Ngày | Chi tiết công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
|:----:|--------------------|:-------:|:----------:|----------------|
|  2   | **Engine Điểm thưởng**:<br>- Viết logic ví điểm<br>- Gắn bảng vào DB | 16/03/2026 | 17/03/2026 | Nội bộ |
|  3   | **Bắt Vi phạm**:<br>- Tạo log theo dõi sai phạm<br>- Setup luật xử phạt | 18/03/2026 | 19/03/2026 | Nội bộ |
|  4   | **Dựng rào Phân quyền (RBAC)**:<br>- Phân bậc user<br>- Gắn quyền vào API | 20/03/2026 | 21/03/2026 | Security Docs |
|  5   | **Nhúng Tính năng & Test**:<br>- Gom module vào app<br>- Chạy kịch bản test luồng | 22/03/2026 | 23/03/2026 | Nội bộ |
|  6   | **Sửa đổi nội thất**:<br>- Tune lại performance<br>- Refactor mã dư thừa | 24/03/2026 | 25/03/2026 | Nội bộ |

---

### Thành quả Tuần 10

#### Cột mốc đạt được

- Chạy đà thành công module **Ví điểm thưởng**.
- Cất nóc cỗ máy **Quản lý hành vi sai phạm** kèm khả năng tự động truy vết.
- Cài cắm lớp khiên **Phân quyền dựa trên vai trò (RBAC)** vào tận lõi ứng dụng.
- Bịt kín các kẽ hở phân quyền vào những tính năng Admin.
- Nâng bật sự mạch lạc trong luồng chạy của App.
- Chắp nối thành công các chức năng mới tinh này vào phiên bản chính thống.

#### Định hướng Kiến trúc

- **Nghiệp vụ cốt lõi**: Cơ chế Thưởng điểm & Bắt phạt.
- **Tường lửa Nội bộ**: Chốt chặn bằng phân quyền người dùng (RBAC).
- **Kho dữ liệu (Database)**: Thiết kế thêm các entity chứa điểm và biên bản vi phạm.
- **Luồng dữ liệu (Flow)**: Thao tác của User → Bộ lọc Backend → Ghi Database → Hiển thị cho Admin.
- **Giai đoạn (Phase)**: Chốt hạ Tính năng nâng cao.