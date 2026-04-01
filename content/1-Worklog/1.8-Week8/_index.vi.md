---
title: "Worklog Tuần 8"
date: 2026-03-02
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Trọng tâm của Tuần 8

Tuần này đánh dấu bước chuyển mình quan trọng từ việc thiết kế trên giấy sang giai đoạn gõ code thực tế. Nhóm tiến hành lập trình các dòng code đầu tiên và kết nối trực tiếp những dịch vụ trọng tâm của AWS vào nền tảng.

- **Bắt tay Lập trình**:
  - Khởi tạo mã nguồn cho các tính năng xương sống.
  - Đấu nối mượt mà giữa lớp màn hình (frontend), xử lý logic (backend) và CSDL.
  - Đúc kết bộ khung kỹ thuật để làm bệ phóng cho các vòng lặp sau.

- **Nhúng Dịch vụ Đám mây AWS**:
  - Dùng **Amazon EC2** làm máy chủ chứa tài nguyên web.
  - Nối **Amazon RDS** làm trung tâm quản trị dữ liệu quan hệ lõi.
  - Biến **Amazon S3** thành kho chứa ảnh, file tĩnh và tài liệu upload.
  - Tích hợp **AWS Map** để phủ sóng tính năng bản đồ và định vị.

- **Kiểm định & Tối ưu**:
  - Xác thực đường đi của dữ liệu xuyên qua các lớp kiến trúc.
  - Sửa lỗi (debug) các tình huống bất đồng bộ trong khâu tích hợp.
  - Sàng lọc cấu trúc code nhằm tạo đà cho lộ trình các tuần tới.

---

### Chi tiết nhiệm vụ

| Ngày | Chi tiết công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
|:----:|--------------------|:-------:|:----------:|----------------|
|  2   | **Khởi động Source Code**:<br>- Khởi ráp khung thư mục project<br>- Viết tính năng cơ bản | 02/03/2026 | 02/03/2026 | Internal |
|  3   | **Ghép nối DB & Backend**:<br>- Thông mạch từ API xuống RDS<br>- Trích xuất dữ liệu mồi | 03/03/2026 | 03/03/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  4   | **Xử lý Tệp tĩnh (S3)**:<br>- Setup bucket S3<br>- Điều phối file asset | 04/03/2026 | 04/03/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  5   | **Xử lý Bản đồ (Maps)**:<br>- Gắn API AWS Map<br>- Đẩy tọa độ lên frontend | 05/03/2026 | 05/03/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  6   | **Deploy & Test**:<br>- Đưa mã nguồn lên EC2<br>- Chạy thử luồng (end-to-end) | 06/03/2026 | 06/03/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |

---

### Thành quả Tuần 8

#### Cột mốc đạt được

- Phát pháo những chuỗi **code logic đầu tiên** vào thực tế.
- Thiết lập tuyến giao thông thông suốt giữa block **Frontend, Backend và Database**.
- Chỉ định đích đến dữ liệu chuẩn xác vào **Amazon RDS**.
- Khai thác thành công kho lưu trữ object **Amazon S3**.
- Sử dụng trơn tru **AWS Map** phục vụ mục đích không gian địa lý.
- Đẩy thành công bản ứng dụng thử nghiệm (staging) lên cổng **Amazon EC2**.
- Đảm bảo luồng chạy thao tác cơ bản (end-to-end flow) hoạt động ổn định.

#### Định hướng Kiến trúc

- **Đầu não xử lý (Compute)**: EC2 đảm trách việc nhận lệnh và phản hồi.
- **Kho dữ liệu (Database)**: RDS bảo quản dữ liệu nghiệp vụ chặt chẽ.
- **Kho tập tin (Storage)**: S3 quán xuyến toàn bộ media và file tĩnh.
- **Hệ Định vị (Map Service)**: AWS Map lo khâu vẽ bản đồ trực quan.
- **Luồng dữ liệu (Flow)**: Vận hành trơn tru cấu trúc Frontend ↔ Backend ↔ AWS.
