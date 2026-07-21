---
title: "Tuần 10"
date: 2026-06-22
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

**Mốc thời gian:** 22/6 → 28/6 (5 ngày làm việc)

## Ngày 1 - 22/06: Nghiên cứu hệ thống giám sát bảo mật trên AWS

**Công việc đã thực hiện:** Tôi bắt đầu tìm hiểu các dịch vụ giám sát và cảnh báo bảo mật trên nền tảng AWS. Tôi nghiên cứu vai trò của Amazon GuardDuty, Amazon EventBridge và Amazon SNS trong việc xây dựng hệ thống phát hiện và phản ứng tự động đối với các sự kiện bảo mật. Đồng thời, tôi tìm hiểu luồng xử lý của một Security Finding từ khi được phát hiện cho đến khi tạo Incident trong hệ thống.

**Kiến thức đã học:** Tôi hiểu GuardDuty là dịch vụ phát hiện mối đe dọa bằng cách phân tích log từ AWS CloudTrail, VPC Flow Logs và DNS Logs. Khi phát hiện hành vi bất thường, GuardDuty sẽ tạo Security Finding để các dịch vụ khác tiếp tục xử lý.

**Kết quả đạt được:** Tôi nắm được kiến trúc tổng thể của hệ thống giám sát bảo mật và hiểu cách các dịch vụ AWS phối hợp với nhau để tự động hóa quá trình phản ứng sự cố.

**Khó khăn và bài học:** Đây là lần đầu tôi tiếp cận một hệ thống giám sát bảo mật hoàn chỉnh nên cần đọc nhiều tài liệu chính thức của AWS. Tôi nhận thấy việc hiểu luồng dữ liệu giúp việc triển khai trở nên dễ dàng hơn.

## Ngày 2 - 23/6: Cấu hình Amazon GuardDuty

**Công việc đã thực hiện:** Tôi tiến hành kích hoạt Amazon GuardDuty trên tài khoản AWS và tìm hiểu các loại Security Finding mà dịch vụ có thể phát hiện. Tôi thực hiện một số bài thực hành mô phỏng để quan sát cách GuardDuty ghi nhận các sự kiện bất thường và hiển thị mức độ nghiêm trọng của từng Finding.

**Kiến thức đã học:** Tôi hiểu GuardDuty sử dụng Machine Learning và Threat Intelligence để phát hiện các hành vi bất thường mà không cần triển khai thêm Agent trên máy chủ. Các Finding được phân loại theo nhiều mức độ để hỗ trợ quá trình xử lý.

**Kết quả đạt được:** GuardDuty được kích hoạt thành công và có thể tạo Security Finding phục vụ cho việc kiểm thử hệ thống.

**Khó khăn và bài học:** Ban đầu tôi gặp khó khăn khi đọc nội dung của các Finding do có nhiều trường dữ liệu. Sau khi tham khảo tài liệu AWS, tôi đã hiểu ý nghĩa của từng thông tin và cách đánh giá mức độ rủi ro.

## Ngày 3 - 24/6: Tích hợp EventBridge với Lambda

**Công việc đã thực hiện:** Tôi cấu hình Amazon EventBridge để lắng nghe các Security Finding do GuardDuty tạo ra. Sau đó, tôi xây dựng Rule để tự động kích hoạt AWS Lambda khi có sự kiện mới. Lambda sẽ xử lý dữ liệu Finding và tạo Incident tương ứng trong hệ thống IRMS.

**Kiến thức đã học:** Tôi hiểu EventBridge là dịch vụ xử lý sự kiện theo mô hình Event-Driven. Khi có sự kiện phù hợp với Rule đã cấu hình, EventBridge sẽ tự động chuyển dữ liệu đến Lambda để xử lý mà không cần sự can thiệp của người dùng.

**Kết quả đạt được:** EventBridge có thể kích hoạt Lambda thành công khi xuất hiện Security Finding và dữ liệu được chuyển đến hệ thống đúng định dạng.

**Khó khăn và bài học:** Trong quá trình cấu hình Rule, tôi gặp lỗi do điều kiện lọc sự kiện chưa chính xác. Sau khi điều chỉnh Event Pattern, Lambda đã nhận đúng các sự kiện từ GuardDuty.

## Ngày 4 - 25/6: Gửi cảnh báo qua Amazon SNS

**Công việc đã thực hiện:** Tôi nghiên cứu Amazon Simple Notification Service (SNS) để gửi thông báo khi hệ thống phát hiện Incident mới. Tôi tạo SNS Topic, đăng ký Email Subscription và tích hợp Lambda để tự động gửi thông báo sau khi Incident được tạo thành công.

**Kiến thức đã học:** Tôi hiểu SNS là dịch vụ gửi thông báo theo mô hình Publish/Subscribe. Một thông điệp có thể được gửi đồng thời đến nhiều Subscriber thông qua Email hoặc các giao thức khác, giúp việc cảnh báo được thực hiện nhanh chóng.

**Kết quả đạt được:** Hệ thống có thể gửi Email thông báo mỗi khi GuardDuty phát hiện một sự kiện bảo mật và Lambda tạo Incident thành công.

**Khó khăn và bài học:** Việc xác nhận Email Subscription là bước bắt buộc trước khi nhận thông báo. Tôi học được cách kiểm tra toàn bộ luồng gửi thông báo để đảm bảo cảnh báo được gửi đến đúng người nhận.

## Ngày 5 - 26/6: Kiểm thử luồng giám sát và tổng kết tuần

**Công việc đã thực hiện:** Tôi tiến hành kiểm thử toàn bộ quy trình từ khi GuardDuty phát hiện mối đe dọa, EventBridge nhận sự kiện, Lambda tạo Incident đến khi SNS gửi Email cảnh báo. Tôi phối hợp cùng các thành viên trong nhóm rà soát kết quả, kiểm tra log trên CloudWatch và ghi nhận các lỗi phát sinh để điều chỉnh.

**Kiến thức đã học:** Tôi hiểu rõ hơn về kiến trúc Event-Driven trên AWS và cách kết hợp nhiều dịch vụ để xây dựng hệ thống phản ứng sự cố tự động. Tôi cũng nhận thấy việc theo dõi log trên CloudWatch rất quan trọng trong quá trình kiểm thử và xử lý lỗi.

**Kết quả đạt được:** Hoàn thiện chức năng tự động tạo Incident và gửi cảnh báo khi phát hiện sự kiện bảo mật. Hệ thống hoạt động ổn định và đáp ứng đúng yêu cầu của dự án.

**Khó khăn và bài học:** Trong quá trình kiểm thử, một số sự kiện chưa được kích hoạt do cấu hình Rule chưa đầy đủ. Sau khi kiểm tra Event Pattern và quyền truy cập của Lambda, toàn bộ quy trình hoạt động chính xác. Tôi rút ra kinh nghiệm rằng khi làm việc với kiến trúc Serverless, cần kiểm tra kỹ từng bước trong chuỗi xử lý để dễ dàng xác định nguyên nhân khi xảy ra lỗi.