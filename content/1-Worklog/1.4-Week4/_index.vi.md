---
title: "Worklog Tuần 4"
date: 2026-01-26
weight: 4 
chapter: false
pre: " <b> 1.4. </b> "
---

### Trọng tâm của Tuần 4

Tuần này hướng đến việc thiết lập và vận hành một hệ thống đạt tiêu chuẩn môi trường sản xuất (production-ready). Phạm vi bao trùm các khía cạnh về tự động hóa, an toàn thông tin, tính sẵn sàng cao, hiệu suất xử lý và tiết kiệm chi phí thuận theo triết lý của AWS Well-Architected Framework.

- **Tối ưu Vận hành (Operational Excellence)**:
  - Dùng AWS Lambda để thiết lập các tác vụ tự động (ví dụ: tự ngắt EC2, đẩy cảnh báo sang nền tảng Slack).
  - Phác họa hệ thống đo lường, giám sát thông qua CloudWatch kết hợp Grafana.
  - Phân loại tài nguyên máy ảo EC2 thông qua hệ thống Tags.
  - Đẩy mạnh tự động hóa quy trình quản trị qua AWS Systems Manager.

- **An toàn thông tin (Security)**:
  - Thiếp lập rào cản phân quyền bằng IAM Permission Boundary.
  - Dò phòng hổng và kiểm soát rủi ro thông qua AWS Security Hub.
  - Tích hợp lớp tường lửa bảo vệ các ứng dụng web với AWS WAF.

- **Độ ổn định, sẵn sàng (Reliability)**:
  - Lên chiến lược phòng chống mất mát dữ liệu nhờ AWS Backup.
  - Giao tiếp xuyên mạng VPC qua cơ chế VPC Peering.
  - Quy hoạch kết nối liên mạng đồng bộ sử dụng Transit Gateway.

- **Năng suất hoạt động (Performance Efficiency)**:
  - Đóng gói phần mềm theo cấu trúc Docker và đưa lên nền tảng ECS.
  - Kiến tạo quy trình triển khai liên tục (CI/CD) với CodePipeline.
  - Mở rộng năng lực dữ liệu với giải pháp File Storage Gateway.

- **Quản lý tài chính (Cost Optimization)**:
  - Mua trước dung lượng/dịch vụ qua Savings Plans và Reserved Instances để giảm phí.
  - Đánh giá và điều chỉnh lại cấu hình EC2 cho vừa vặn (Right-sizing).
  - Vẽ biểu đồ theo dõi các khoản chi tiêu Cloud sát sao.

---

### Chi tiết nhiệm vụ

| Ngày | Chi tiết công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
|:----:|--------------------|:-------:|:----------:|----------------|
|  2   | **Tự động & Giám sát**:<br>- Lập trình Lambda<br>- Tích hợp CloudWatch và Grafana<br>- Quản lý bằng Tags<br>- Công cụ Systems Manager | 26/01/2026 | 26/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  3   | **Hàng rào bảo mật**:<br>- Giới hạn quyền theo Boundary<br>- Đánh giá từ Security Hub<br>- Áp dụng luật WAF | 27/01/2026 | 27/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  4   | **Dự phòng & Mạng**:<br>- Lên lịch AWS Backup<br>- Định tuyến VPC Peering<br>- Thiết lập Transit Gateway | 28/01/2026 | 28/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  5   | **Hiệu suất hệ thống**:<br>- Container hóa vs Docker/ECS<br>- Dựng luồng CodePipeline<br>- Kết nối File Storage Gateway | 29/01/2026 | 29/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |
|  6   | **Cân đối thu chi**:<br>- Tham gia Savings Plans<br>- Đăng ký Reserved Instances<br>- Dashboard báo cáo chi phí | 30/01/2026 | 30/01/2026 | [AWS Docs](https://cloudjourney.awsstudygroup.com/) |

---

### Thành quả Tuần 4

#### Cột mốc đạt được

- Đưa tự động hóa vào đời sống vận hành:
  - Script Lambda giúp tự động tắt EC2 lúc ngoài giờ làm và báo cáo lỗi qua Slack.
  - Xây lên các bảng điều khiển số liệu trực quan cùng CloudWatch cộng hưởng Grafana.
  - Áp dụng Tags và dùng Systems Manager để thao tác dễ dàng trên lô lượng lớn tài nguyên.

- Nâng trần phòng ngự cho hệ thống:
  - Gắn chặt giới hạn hạn quyền với **IAM Permission Boundary**.
  - Đứng vững trước lưu lượng web có dấu hiệu lừa đảo thông qua **AWS WAF**.
  - Thường xuyên khám sức khỏe an ninh bằng **Security Hub**.

- Tăng cường sức chịu đựng của dịch vụ:
  - Tạo luồng sao lưu định kỳ liền mạch cùng **AWS Backup**.
  - Thông hành trơn tru giữa các khu vực mạng thông qua **VPC Peering** và trạm trung chuyển **Transit Gateway**.

- Đáp ứng năng lực xử lý vượt trội:
  - Chạy ứng dụng dưới định dạng container qua công cụ **Docker + ECS**.
  - Dựng thành công tuyến đường băng chuyền CI/CD.

- Tối giản hóa hóa đơn hàng tháng:
  - Đăng ký lộ trình chiết khấu **Savings Plans / Reserved Instances**.
  - Điều hướng và thu hẹp bớt tài nguyên máy ảo bị dư thừa năng lực (**Right-sizing EC2**).
  - Hiển thị trực quan bức tranh chi tiêu AWS.

#### Kiến thức cốt lõi

- **Trục tự động (Automation)**: Cặp bài trùng Lambda và Systems Manager.
- **Trục giám sát (Monitoring)**: Số liệu CloudWatch được visualize bằng Grafana.
- **Trục an ninh (Security)**: Chốt chặn IAM Boundary + Bộ lọc truy cập WAF + Trung tâm soát lỗi Security Hub.
- **Trục điều hướng (Networking)**: Mạng nối tiếp VPC Peering + Nút mạng trung tâm Transit Gateway.
- **Trục xử lý (Compute)**: Dàn Container vận hành trên hệ thống ECS (Docker).
- **Trục đóng gói (CI/CD)**: Trình quản lý luồng CodePipeline.
- **Trục mở rộng (Storage)**: Kỹ thuật nhúng lưu trữ File Storage Gateway.
- **Trục kế toán (Cost)**: Áp dụng Savings Plans đi kèm hệ thống kiểm soát tiền tệ.
