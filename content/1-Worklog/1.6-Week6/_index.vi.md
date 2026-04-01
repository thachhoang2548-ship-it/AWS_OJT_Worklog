---
title: "Worklog Tuần 6"
date: 2026-02-09
weight: 6 
chapter: false
pre: " <b> 1.6. </b> "
---

### Trọng tâm của Tuần 6

Tuần này dồn toàn lực vào mảng cơ sở dữ liệu quan hệ, đi sâu vào nền tảng SQL Server. Các nội dung trải dài từ thiết kế cấu trúc bảng, thao tác truy xuất dữ liệu đến các kỹ thuật phân tích hiệu năng.

- **Cơ sở SQL Server**:
  - Giới thiệu thực thể: Cơ sở dữ liệu, Bảng dữ liệu, Hàng, Cột.
  - Khái niệm mỏ neo: Khóa chính (Primary Key) & Khóa ngoại (Foreign Key).
  - Xây dựng sơ đồ (Schema) chuẩn chỉnh.

- **Khởi tạo dữ liệu**:
  - Thao tác lập database và tạo lập các bảng.
  - Áp dụng các luật khống chế dữ liệu (constraints).

- **Chuỗi thao tác CRUD bằng mã SQL**:
  - Thêm mới (INSERT).
  - Truy vấn (SELECT).
  - Chỉnh sửa (UPDATE).
  - Xóa bỏ (DELETE).

- **Phần mềm Giao tiếp**:
  - Làm chủ SQL Server Management Studio (SSMS) và Azure Data Studio.
  - Thao tác trực tiếp trên AWS RDS (hệ quản trị SQL Server) hoặc máy local.

- **Đo lường năng lực (Performance)**:
  - Cân đo đếm thời gian chạy query.
  - Tập đọc và hiểu Execution Plan cơ bản.

---

### Chi tiết nhiệm vụ

| Ngày | Chi tiết công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
|:----:|--------------------|:-------:|:----------:|----------------|
|  2   | **Nền tảng SQL Server**:<br>- Database, cấu trúc bảng<br>- Ràng buộc khóa chính, khóa phụ | 09/02/2026 | 09/02/2026 | Microsoft Docs |
|  3   | **Xây dựng CSDL**:<br>- Tạo mới database<br>- Lập sơ đồ bảng và các luật | 10/02/2026 | 10/02/2026 | Microsoft Docs |
|  4   | **Xử lý CRUD**:<br>- Dùng lệnh INSERT / SELECT / UPDATE / DELETE | 11/02/2026 | 11/02/2026 | Microsoft Docs |
|  5   | **Công cụ & Tối ưu hóa**:<br>- SSMS / Azure Data Studio<br>- Chẩn đoán tốc độ và Execution plan | 12/02/2026 | 12/02/2026 | Microsoft Docs |

---

### Thành quả Tuần 6

#### Cột mốc đạt được

- Trực tiếp tạo dựng và tùy chỉnh một **CSDL SQL Server** hoàn chỉnh.
- Hiểu thấu đáo về **sơ đồ liên kết, Khóa chính (PK) ghép cùng Khóa phụ (FK)**.
- Xử lý mượt mà toàn bộ **lệnh CRUD bằng ngôn ngữ SQL**.
- Biết cách sử dụng **SSMS / Azure Data Studio** phục vụ công việc.
- Quản trị chéo giữa **AWS RDS (chạy SQL Server)** và môi trường cục bộ.
- Có khả năng **bắt bệnh truy vấn chậm thông qua execution plan**.

#### Kiến thức cốt lõi

- **Hệ thống lưu trữ (Database)**: Mô hình quản trị dữ liệu quan hệ (SQL Server).
- **Thiết kế cấu trúc (Schema)**:
  - Tổ chức bảng và thiết lập mối liên kết.
  - An toàn đối chiếu dữ liệu (PK/FK).
- **Phần mềm truy cập**:
  - Các GUI tools như SSMS hoặc Azure Data Studio.
- **Hiệu năng hệ thống**:
  - Các bước tối ưu hóa truy vấn sơ đẳng.
  - Khai thác dữ liệu từ Execution Plan.