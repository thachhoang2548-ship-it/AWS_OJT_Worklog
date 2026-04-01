---
title: "Worklog Tuần 3"
date: 2026-01-19
weight: 3 
chapter: false
pre: " <b> 1.3. </b> "
---

### Trọng tâm của Tuần 3

Mục đích chính của tuần này là lên khung ý tưởng cho dự án chốt khóa (capstone) đi đôi với việc cọ xát thực tế các dịch vụ xương sống của AWS như EC2, S3, IAM và RDS. Các tiêu điểm chính gồm:

- **Định hình dự án chốt khóa**:
  - Tổ chức brainstorm các ý tưởng khả thi.
  - Sàng lọc và chọn lựa dịch vụ AWS tương ứng.
  - Phác họa sơ đồ kiến trúc hệ thống ban đầu.

- **Kinh nghiệm thực chiến EC2**:
  - Trải nghiệm sâu hơn mô hình dịch vụ EC2.
  - Khởi tạo và vận hành các máy ảo (virtual machines).
  - Tùy biến thông số cấu hình của instance.
  - Đóng gói và sử dụng các bản image (AMI) cá nhân hóa.

- **Cơ chế Phân quyền & Không gian Code (IDE)**:
  - Ứng dụng thực tiễn của IAM Role.
  - Khám phá môi trường lập trình đám mây AWS Cloud9.

- **Giải pháp Lưu trữ S3**:
  - Xây dựng và thiết lập các bucket lưu trữ.
  - Quản trị object và tinh chỉnh quyền truy cập dữ liệu.

- **Hệ quản trị CSDL RDS**:
  - Triển khai cụm cơ sở dữ liệu quan hệ.
  - Nắm bắt quy trình vận hành và bảo trì RDS.

- **Củng cố nền tảng kiến thức**:
  - Nhìn lại hệ sinh thái IAM, EC2, S3, RDS.
  - Hệ thống lại lượng kiến thức từ Tuần 1 và Tuần 2.

---

### Chi tiết nhiệm vụ

| Ngày | Chi tiết công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
|:----:|--------------------|:-------:|:----------:|----------------|
|  2   | **Kế hoạch dự án**:<br>- Brainstorm ý tưởng<br>- Chốt danh sách dịch vụ<br>- Vẽ nháp kiến trúc | 19/01/2026 | 19/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  3   | **Máy chủ & Bản sao (AMI)**:<br>- Bật EC2<br>- Cấu hình máy chủ<br>- Xuất AMI tự tạo | 20/01/2026 | 20/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  4   | **Phân quyền & IDE**:<br>- Cấu hình IAM Role<br>- Thao tác trên Cloud9 | 21/01/2026 | 21/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  5   | **Kho lưu trữ S3**:<br>- Tạo lập bucket<br>- Cấp quyền Public<br>- Quản lý phiên bản (Versioning) | 22/01/2026 | 22/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  6   | **Cơ sở dữ liệu & Ôn tập**:<br>- Khởi động RDS<br>- Thao tác với DB<br>- Tổng hợp kiến thức | 23/01/2026 | 23/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |

---

### Thành quả Tuần 3

#### Cột mốc đạt được

- Chốt hạ được bản thiết kế kiến trúc chuẩn chỉnh cho **dự án cuối khóa**.
- Khởi chạy và kiểm soát trơn tru hệ thống các máy ảo **EC2 instances**.
- Thành thạo việc tạo bản sao lưu và tái triển khai qua **AMI tùy chỉnh**.
- Triển khai **IAM Roles** đáp ứng đúng bài toán phân quyền thực tế.
- Khởi tạo và sử dụng thành thạo môi trường IDE **AWS Cloud9**.
- Hoàn thành **trang web tĩnh lưu trữ trên Amazon S3** với các tính năng:
  - Cho phép truy cập từ internet (Public access).
  - Lưu vết các bản cập nhật (Versioning).
  - Đồng bộ chép vác dữ liệu liên region (Cross-region replication).
- Vận hành trơn tru một cụm database qua dịch vụ **Amazon RDS**.
- Nắm vững hơn những mảng kiến thức đã được học ở các tuần đầu.

#### Kiến thức cốt lõi

- **Lớp tính toán (Compute)**: Dùng máy chủ ảo EC2 kết hợp các bản AMI được tùy biến.
- **Lớp lưu trữ (Storage)**: Khai thác kho chứa S3 (hỗ trợ Web tĩnh + Versioning + Replication).
- **Lớp dữ liệu (Database)**: Dịch vụ cơ sở dữ liệu tích hợp sẵn RDS.
- **Lớp bảo mật (Access Control)**: Quản lý quyền theo vai trò qua IAM Role.
- **Không gian phát triển (Dev Environment)**: Công cụ lập trình dựa trên web Cloud9.
