---
title: "Worklog Tuần 1"
date: 2026-01-05
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

### Trọng tâm của Tuần 1

Mục đích chính của tuần này là xây dựng kiến thức nền tảng về AWS, chuẩn bị môi trường thực hành và nắm bắt các khái niệm cơ bản về bảo mật tài khoản cũng như theo dõi chi phí. Các trọng tâm cụ thể gồm:

- **Nắm bắt nền tảng AWS**:
  - Khám phá cơ chế hoạt động và các mô hình điện toán đám mây.
  - Điểm qua một số dịch vụ trọng yếu (EC2, S3, IAM, VPC, v.v.).

- **Khám phá cấu trúc Lab**:
  - Phác họa bức tranh tổng thể về cách bố trí các bài lab.
  - Làm quen luồng thao tác thực hành (hands-on).

- **Phát triển nhóm**:
  - Tổ chức và hình thành một nhóm làm việc.
  - Tương tác với các thành viên khác để tăng cường sự gắn kết.

- **Khởi tạo tài khoản AWS**:
  - Đăng ký một tài khoản AWS mới thuộc gói Free Tier.
  - Kích hoạt **MFA cho Root User** để đảm bảo an toàn.
  - Thiết lập một người dùng IAM có quyền quản trị (Admin).
  - Tạo nhóm Admin với các policy tương ứng.
  - Trải nghiệm giao diện hệ thống AWS Management Console.

- **Giám sát ngân sách & Chi phí**:
  - Xây dựng Cost Budget.
  - Thiết lập Usage Budget.
  - Xác định các Reservation và Savings Plans Budget.
  - Cài đặt hệ thống cảnh báo (alert).
  - Loại bỏ các tài nguyên không dùng đến.

---

### Chi tiết nhiệm vụ

| Ngày | Chi tiết công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
|:----:|--------------------|:-------:|:----------:|----------------|
|  2   | **Khái niệm AWS cốt lõi**:<br>- Giới thiệu AWS<br>- Các mô hình triển khai Cloud<br>- Dịch vụ cơ sở | 05/01/2026 | 05/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  3   | **Định hướng Lab**:<br>- Cấu trúc hệ thống lab<br>- Phương pháp tiếp cận thực hành | 06/01/2026 | 06/01/2026 | [AWS Study Group](https://www.facebook.com/groups/awsstudygroupfcj/) |
|  4   | **Gắn kết đội nhóm**:<br>- Xây dựng đội ngũ<br>- Giao lưu thành viên<br>- Đề ra phương hướng chung | 07/01/2026 | 07/01/2026 | Nội bộ |
|  5   | **Quản lý danh tính (IAM)**:<br>- Khởi tạo tài khoản<br>- Bật xác thực hai bước (MFA)<br>- Tạo User/Group quản trị<br>- Làm quen giao diện điều khiển | 08/01/2026 | 08/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  6   | **Kiểm soát chi phí**:<br>- Định nghĩa các ngân sách (Budgets)<br>- Lên kịch bản cảnh báo<br>- Dọn dẹp tài nguyên rác | 09/01/2026 | 09/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |

---

### Thành quả Tuần 1

#### Cột mốc đạt được

- Đạt được hiểu biết vững chắc về **các khái niệm cốt lõi của AWS**.
- Tích lũy đủ kỹ năng cần thiết để tiếp cận và xử lý **các bài thực hành lab**.
- Chính thức thành lập **đội nhóm học tập** và đi vào hoạt động chung.
- Đăng ký tài khoản AWS thành công với **quyền lợi Free Tier (khoảng $100)**.
- Thắt chặt an ninh bằng việc kích hoạt **MFA cho Root Account**.
- Khởi tạo xong **người dùng IAM quản trị** chuyên biệt.
- Sử dụng thành thạo điều hướng cơ bản trên **AWS Management Console**.
- Áp dụng **AWS Budgets** để giám sát mức chi tiêu trên nền tảng.
- Bật **cảnh báo chi phí** đồng thời thực hiện thao tác xóa tài nguyên thừa.

#### Bài học kinh nghiệm

- **Tiêu chuẩn Bảo mật**:
  - Hạn chế tối đa sử dụng Root Account cho tác vụ hàng ngày.
  - Đảm bảo MFA luôn được áp dụng cho các tài khoản có đặc quyền.

- **Quản lý mức sử dụng**:
  - Thường xuyên theo dõi resource tiêu thụ thông qua AWS Budgets.
  - Thiết lập ngưỡng alert để tránh các khoản phí phát sinh ngoài ý muốn.

- **Định hướng học hỏi**:
  - Tích cực thực hành thao tác (hands-on).
  - Giữ kết nối và trao đổi thường xuyên trong nhóm.
