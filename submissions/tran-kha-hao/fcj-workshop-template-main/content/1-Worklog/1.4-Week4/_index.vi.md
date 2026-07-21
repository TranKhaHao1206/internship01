---
title: "Tuần 4"
date: 2026-05-11
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

**Mốc thời gian:** 11/5 → 17/5 (5 ngày làm việc)

## Ngày 1 - 11/5: Khởi tạo Amazon EC2

**Công việc đã thực hiện:** Tôi bắt đầu triển khai hạ tầng cho dự án bằng cách tìm hiểu và khởi tạo một máy chủ Amazon EC2. Tôi thực hành tạo EC2 Instance trên AWS Console, lựa chọn Amazon Machine Image (AMI), loại Instance phù hợp, cấu hình Security Group và tạo Key Pair để phục vụ việc kết nối từ máy tính cá nhân đến máy chủ.

**Kiến thức đã học:** Tôi hiểu Amazon EC2 là dịch vụ cung cấp máy chủ ảo trên nền tảng điện toán đám mây, cho phép triển khai ứng dụng với khả năng mở rộng linh hoạt. Tôi cũng nắm được vai trò của AMI, Instance Type, Key Pair và Security Group trong quá trình khởi tạo máy chủ.

**Kết quả đạt được:** Tôi tạo thành công một EC2 Instance, cấu hình các cổng cần thiết và kết nối thành công đến máy chủ thông qua SSH để chuẩn bị cho việc triển khai ứng dụng.

**Khó khăn và bài học:** Trong quá trình kết nối SSH, tôi gặp lỗi do quyền truy cập của tệp Key Pair chưa đúng. Sau khi điều chỉnh quyền và kiểm tra Security Group, tôi đã kết nối thành công. Tôi rút ra kinh nghiệm cần kiểm tra kỹ cấu hình bảo mật trước khi triển khai.

---

## Ngày 2 - 12/5: Cấu hình Amazon VPC

**Công việc đã thực hiện:** Sau khi khởi tạo EC2, tôi tiếp tục nghiên cứu Amazon Virtual Private Cloud (VPC). Tôi thực hành tạo VPC mới, cấu hình Subnet, Internet Gateway và Route Table để thiết lập môi trường mạng riêng cho hệ thống.

**Kiến thức đã học:** Tôi hiểu VPC là mạng riêng ảo trên AWS giúp kiểm soát địa chỉ IP, định tuyến và kết nối mạng của các tài nguyên. Tôi cũng hiểu mối quan hệ giữa VPC, Subnet, Internet Gateway và Route Table trong việc xây dựng hệ thống mạng an toàn.

**Kết quả đạt được:** Hoàn thành cấu hình VPC và kết nối EC2 với Internet thông qua Internet Gateway, đảm bảo máy chủ có thể truy cập các dịch vụ cần thiết.

**Khó khăn và bài học:** Ban đầu tôi nhầm lẫn giữa Public Subnet và Private Subnet dẫn đến việc EC2 không thể truy cập Internet. Sau khi kiểm tra lại Route Table và Gateway, tôi đã khắc phục được vấn đề.

---

## Ngày 3 - 13/5: Làm việc với Amazon DynamoDB

**Công việc đã thực hiện:** Tôi tìm hiểu Amazon DynamoDB và thực hành tạo bảng dữ liệu phục vụ dự án. Tôi thiết lập Partition Key phù hợp với dữ liệu quản lý Incident và thực hiện các thao tác CRUD (Create, Read, Update, Delete) để kiểm tra khả năng lưu trữ và truy xuất dữ liệu.

**Kiến thức đã học:** Tôi hiểu DynamoDB là cơ sở dữ liệu NoSQL được AWS quản lý hoàn toàn, có khả năng mở rộng tự động và tốc độ truy xuất rất cao. Tôi cũng hiểu tầm quan trọng của việc lựa chọn Partition Key phù hợp để tối ưu hiệu năng hệ thống.

**Kết quả đạt được:** Tôi tạo thành công bảng DynamoDB và thực hiện đầy đủ các thao tác thêm, sửa, xóa và truy vấn dữ liệu.

**Khó khăn và bài học:** Lúc đầu tôi chưa hiểu cách DynamoDB lưu trữ dữ liệu theo Partition Key nên việc thiết kế bảng còn chưa hợp lý. Sau khi tham khảo tài liệu AWS, tôi đã điều chỉnh cấu trúc dữ liệu phù hợp hơn.

---

## Ngày 4 - 14/5: Amazon Cognito và xác thực người dùng

**Công việc đã thực hiện:** Tôi nghiên cứu Amazon Cognito để xây dựng chức năng xác thực người dùng cho hệ thống. Tôi thực hành tạo User Pool, cấu hình chính sách mật khẩu, tạo tài khoản thử nghiệm và tìm hiểu quy trình đăng nhập bằng Authentication Flow.

**Kiến thức đã học:** Tôi hiểu Amazon Cognito là dịch vụ quản lý người dùng và xác thực của AWS, hỗ trợ đăng ký, đăng nhập và quản lý thông tin người dùng. Tôi cũng hiểu vai trò của User Pool trong việc lưu trữ thông tin tài khoản và xác thực người dùng.

**Kết quả đạt được:** Tôi tạo thành công User Pool và đăng nhập thử nghiệm bằng tài khoản đã tạo để kiểm tra quy trình xác thực.

**Khó khăn và bài học:** Việc cấu hình Authentication Flow có khá nhiều tùy chọn nên tôi mất thời gian tìm hiểu từng cơ chế hoạt động trước khi lựa chọn cấu hình phù hợp.

---

## Ngày 5 - 15/5: Tìm hiểu JWT Token và tổng kết tuần

**Công việc đã thực hiện:** Tôi tiếp tục nghiên cứu JSON Web Token (JWT) được Amazon Cognito sử dụng để xác thực người dùng. Tôi tìm hiểu cấu trúc của Access Token, ID Token và Refresh Token, đồng thời kiểm tra quá trình tạo và sử dụng Token sau khi đăng nhập. Cuối ngày, tôi tổng hợp toàn bộ kiến thức đã học trong tuần và chuẩn bị cho việc tích hợp các dịch vụ AWS vào dự án ở tuần tiếp theo.

**Kiến thức đã học:** Tôi hiểu JWT gồm ba thành phần là Header, Payload và Signature. Tôi biết cách Cognito cấp Token sau khi người dùng xác thực thành công và cách Token được sử dụng để truy cập các API được bảo vệ.

**Kết quả đạt được:** Tôi nắm được quy trình xác thực bằng Cognito và JWT, đồng thời hiểu cách kết hợp EC2, VPC, DynamoDB và Cognito trong kiến trúc của hệ thống.

**Khó khăn và bài học:** Tuần này có nhiều dịch vụ AWS mới nên lượng kiến thức khá lớn. Tôi nhận thấy việc ghi chép sơ đồ kiến trúc và mối liên hệ giữa các dịch vụ giúp việc học dễ dàng và hiệu quả hơn.