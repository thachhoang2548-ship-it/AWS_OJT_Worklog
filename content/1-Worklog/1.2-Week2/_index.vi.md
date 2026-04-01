---
title: "Worklog Tuần 2"
date: 2026-01-12
weight: 2 
chapter: false
pre: " <b> 1.2. </b> "
---

### Trọng tâm của Tuần 2

Tuần này xoay quanh việc thiết lập hạ tầng mạng vững chắc và quản lý quyền truy cập danh tính trên AWS, từ các khái niệm căn bản đến mô hình phức tạp. Các trọng tâm cụ thể gồm:

- **Kiểm soát IAM**:
  - Khởi tạo các Users và Groups.
  - Liên kết các Policies cấp quyền.
  - Định nghĩa và áp dụng IAM Roles.
  - Trải nghiệm tính năng **Switch Role**.

- **Lý thuyết & Thực hành VPC**:
  - Nắm bắt mô hình kiến trúc mạng VPC.
  - Phân tích điểm khác biệt giữa **Network ACLs và Security Groups**.
  - Thiết kế sẵn sàng môi trường mạng để chạy EC2.

- **Khởi chạy máy chủ EC2**:
  - Đưa EC2 instance vào hoạt động trong các subnet.
  - Tùy chỉnh tường lửa Security Group.
  - Thiết lập kết nối từ xa (SSH) qua Key Pair.

- **Thiết lập Hybrid DNS bằng Route 53 Resolver**:
  - Khởi tạo Key Pair.
  - Cấu hình các rule cho Security Group.
  - Quản lý DNS:
    - Cấu hình Outbound Endpoint.
    - Lên bộ quy tắc Resolver Rules.
    - Cấu hình Inbound Endpoint.
  - Xóa bỏ tài nguyên rác.

- **Kết nối mạng qua VPC Peering**:
  - Nắm vững khái niệm Peering.
  - Triển khai tự động hạ tầng qua CloudFormation.
  - Chuẩn bị EC2 và Security Group tương ứng.
  - Chỉnh sửa quy tắc Network ACLs.
  - Khởi tạo Peering Connection giữa hai mạng.
  - Cập nhật định tuyến (Route Tables).
  - Cho phép phân giải DNS chéo (Cross-Peer).

- **Ứng dụng AWS Transit Gateway**:
  - Khởi tạo thành phần Transit Gateway.
  - Kết nối (Attach) các VPC đích vào Gateway.
  - Quy định Route Tables ngay trên Transit Gateway.
  - Điều chỉnh lại Route Tables tại các VPC.

---

### Chi tiết nhiệm vụ

| Ngày | Chi tiết công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
|:----:|--------------------|:-------:|:----------:|----------------|
|  2   | **IAM & EC2 cốt lõi**:<br>- Quản trị User, Group<br>- Cấp phát Policy<br>- Switch Role & Assume Role<br>- Khởi tạo EC2 và SSH vào máy | 12/01/2026 | 12/01/2026 | [AWS Study Group](https://www.facebook.com/groups/awsstudygroupfcj/) |
|  3   | **Mạng VPC**:<br>- Kiến trúc VPC<br>- Đối chiếu SG và NACL<br>- Quy hoạch subnet cho EC2 | 13/01/2026 | 13/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  4   | **Kiến trúc Hybrid DNS**:<br>- Sinh Key Pair<br>- Tinh chỉnh SG<br>- Xây dựng In/Out Endpoint<br>- Khai báo quy tắc Resolver | 14/01/2026 | 14/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  5   | **Kết nối VPC Peering**:<br>- Setup bằng CloudFormation<br>- Khởi tạo EC2 và SG<br>- Mở kết nối Peering<br>- Sửa đổi Route Table<br>- Bật tính năng DNS tĩnh | 15/01/2026 | 15/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  6   | **Sử dụng Transit Gateway**:<br>- Khởi động TGW<br>- Gắn VPC (Attachment)<br>- Tùy chỉnh định tuyến liên mạng | 16/01/2026 | 16/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |

---

### Thành quả Tuần 2

#### Cột mốc đạt được

- Nắm chắc phương pháp phân quyền với **IAM** cũng như thao tác **Switch Role**.
- Nắm bắt luồng mạng **VPC**, hiểu cách Security Group bảo vệ tài nguyên.
- Tạo máy ảo **EC2** và thao tác thành công qua giao thức SSH.
- Cấu hình liền mạch **Hybrid DNS** nhờ Route 53 Resolver.
- Thành công thiết lập **VPC Peering**, nối liền hai môi trường Dev và Staging.
- Sử dụng **AWS Transit Gateway** như bộ xử lý mạng trung tâm đa VPC.
- Làm quen khái niệm **Infrastructure as Code** khi triển khai CloudFormation.
- Luôn đảm bảo hoàn tất khâu **dọn dẹp tài nguyên** (clean up).

#### Kiến thức cốt lõi

- **Mô hình IAM**: Đi từ Users → Groups → Policies → Roles (linh hoạt quyền).
- **Mô hình bảo vệ VPC**:
  - Security Group: Áp dụng trên mức instance.
  - NACL: Áp dụng trên mức subnet.
- **Hoạt động Hybrid DNS**:
  - Phân giải giữa On-premise và mạng AWS thông qua các điểm dò Route 53 Resolver.
- **Mô hình kết nối mạng**:
  - VPC Peering: Kết nối ngang hàng (point-to-point).
  - Transit Gateway: Cấu trúc trung tâm (hub-and-spoke).
