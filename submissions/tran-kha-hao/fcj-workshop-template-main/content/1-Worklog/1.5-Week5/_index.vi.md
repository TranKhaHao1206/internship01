---
title: "Tuần 5"
date: 2026-05-18
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

**Mốc thời gian:** 18/5 → 24/5 (5 ngày làm việc)

## Ngày 1 - 18/5: Tìm hiểu AWS Lambda và mô hình Function as a Service (FaaS)

**Công việc đã thực hiện:** Tôi bắt đầu tìm hiểu AWS Lambda - dịch vụ điện toán không máy chủ (Serverless Computing) của AWS. Tôi nghiên cứu cách Lambda hoạt động, tạo một Lambda Function đầu tiên bằng Node.js và thực hành viết các đoạn mã đơn giản để xử lý yêu cầu từ người dùng. Đồng thời tôi tìm hiểu quy trình triển khai và kiểm thử hàm trực tiếp trên AWS Console.

**Kiến thức đã học:** Tôi hiểu AWS Lambda là dịch vụ cho phép thực thi mã nguồn mà không cần quản lý máy chủ. Người phát triển chỉ cần tập trung vào việc viết mã, AWS sẽ tự động cấp phát tài nguyên, mở rộng và quản lý hạ tầng khi có yêu cầu thực thi.

**Kết quả đạt được:** Tôi tạo thành công Lambda Function đầu tiên và thực hiện kiểm thử bằng các sự kiện (Event) mẫu do AWS cung cấp.

**Khó khăn và bài học:** Ban đầu tôi chưa quen với mô hình Serverless vì không còn phải cấu hình máy chủ như EC2. Sau khi thực hành nhiều lần, tôi hiểu rõ quy trình hoạt động dựa trên sự kiện (Event-Driven) của Lambda.

## Ngày 2 - 19/5: Tích hợp Lambda với DynamoDB

**Công việc đã thực hiện:** Tôi tiếp tục xây dựng Lambda Function để thao tác với bảng dữ liệu trên Amazon DynamoDB. Tôi thực hiện các chức năng thêm mới, cập nhật, truy vấn và xóa dữ liệu nhằm chuẩn bị cho việc phát triển các API của hệ thống.

**Kiến thức đã học:** Tôi hiểu cách AWS SDK hỗ trợ Lambda kết nối với DynamoDB và thực hiện các thao tác CRUD. Tôi cũng tìm hiểu cơ chế phân quyền IAM Role để Lambda có thể truy cập cơ sở dữ liệu một cách an toàn.

**Kết quả đạt được:** Lambda có thể đọc và ghi dữ liệu vào DynamoDB thành công, giúp tôi hiểu rõ quy trình xử lý dữ liệu trong kiến trúc Serverless.

**Khó khăn và bài học:** Trong quá trình thực hiện, Lambda gặp lỗi thiếu quyền truy cập vào DynamoDB. Tôi đã kiểm tra và bổ sung IAM Policy phù hợp để khắc phục vấn đề.

## Ngày 3 - 20/5: Tìm hiểu API Gateway và Cognito

**Công việc đã thực hiện:** Tôi nghiên cứu Amazon API Gateway và vai trò của dịch vụ này trong việc xây dựng REST API. Đồng thời tôi tìm hiểu cách kết hợp API Gateway với Amazon Cognito để xác thực người dùng trước khi cho phép truy cập các API của hệ thống.

**Kiến thức đã học:** Tôi hiểu API Gateway là dịch vụ trung gian tiếp nhận yêu cầu từ phía Client, chuyển tiếp đến Lambda để xử lý và trả kết quả về cho người dùng. Cognito được sử dụng để xác thực và cấp JWT Token nhằm bảo vệ các API khỏi truy cập trái phép.

**Kết quả đạt được:** Tôi nắm được luồng xử lý từ Client → API Gateway → Lambda → DynamoDB và ngược lại, đồng thời hiểu cách Cognito tham gia vào quy trình xác thực.

**Khó khăn và bài học:** Ban đầu tôi chưa hình dung rõ mối liên kết giữa API Gateway, Lambda và Cognito. Sau khi vẽ sơ đồ luồng dữ liệu, tôi đã hiểu được cách các dịch vụ phối hợp với nhau trong hệ thống.

## Ngày 4 - 21/5: Thiết kế kiến trúc hệ thống

**Công việc đã thực hiện:** Tôi cùng các thành viên trong nhóm phân tích yêu cầu của dự án và thiết kế sơ đồ kiến trúc tổng thể. Chúng tôi xác định các thành phần chính của hệ thống gồm Frontend, API Gateway, Lambda, Cognito, DynamoDB và Amazon S3, đồng thời mô tả luồng xử lý dữ liệu giữa các dịch vụ.

**Kiến thức đã học:** Tôi hiểu tầm quan trọng của việc thiết kế kiến trúc trước khi bắt đầu phát triển hệ thống. Một kiến trúc hợp lý sẽ giúp hệ thống dễ mở rộng, dễ bảo trì và đảm bảo hiệu năng trong quá trình vận hành.

**Kết quả đạt được:** Nhóm hoàn thành sơ đồ kiến trúc ban đầu của hệ thống và thống nhất phương án triển khai cho các tuần tiếp theo.

**Khó khăn và bài học:** Việc lựa chọn dịch vụ phù hợp cho từng chức năng cần nhiều thời gian phân tích. Tôi học được rằng nên ưu tiên các dịch vụ Serverless để giảm chi phí quản lý hạ tầng và tăng khả năng mở rộng.

## Ngày 5 - 22/5: Tổng hợp kiến thức và chuẩn bị triển khai

**Công việc đã thực hiện:** Tôi rà soát lại toàn bộ kiến thức đã học trong tuần, kiểm tra hoạt động của Lambda Function, API Gateway và DynamoDB. Đồng thời cập nhật tài liệu kỹ thuật, chỉnh sửa sơ đồ kiến trúc theo góp ý của nhóm và chuẩn bị môi trường để triển khai các chức năng chính của hệ thống ở tuần tiếp theo.

**Kiến thức đã học:** Tôi củng cố kiến thức về kiến trúc Serverless trên AWS và hiểu cách các dịch vụ Lambda, API Gateway, Cognito và DynamoDB phối hợp với nhau để xây dựng một ứng dụng Web hiện đại.

**Kết quả đạt được:** Tôi hoàn thiện môi trường phát triển, nắm rõ kiến trúc của dự án và sẵn sàng bước vào giai đoạn xây dựng các chức năng nghiệp vụ.

**Khó khăn và bài học:** Sau một tuần làm việc với nhiều dịch vụ AWS, tôi nhận thấy việc đọc tài liệu chính thức và thường xuyên thực hành trên AWS Console là cách hiệu quả nhất để hiểu rõ cơ chế hoạt động của từng dịch vụ. Tôi cũng học được cách làm việc nhóm và trao đổi thường xuyên để thống nhất phương án triển khai.