---
title: "Tuần 7"
date: 2026-06-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

**Mốc thời gian:** 1/6 → 7/6 (5 ngày làm việc)

## Ngày 1 - 1/6: Xây dựng chức năng Evidence Management

**Công việc đã thực hiện:** Tôi bắt đầu phát triển chức năng quản lý bằng chứng điều tra (Evidence Management) cho hệ thống IRMS. Tôi phân tích yêu cầu nghiệp vụ, xác định các loại dữ liệu cần lưu trữ như file log, hình ảnh, tài liệu PDF và thông tin mô tả bằng chứng. Sau đó, tôi thiết kế cấu trúc dữ liệu và luồng xử lý cho chức năng này.

**Kiến thức đã học:** Tôi hiểu vai trò của Evidence Management trong hệ thống Incident Response. Việc lưu trữ và quản lý bằng chứng giúp phục vụ quá trình điều tra, truy vết sự cố và hỗ trợ kiểm toán sau này. Tôi cũng hiểu cần tách dữ liệu metadata và dữ liệu tệp để tối ưu hiệu suất hệ thống.

**Kết quả đạt được:** Hoàn thành thiết kế chức năng Evidence Management và xác định được các trường dữ liệu cần quản lý trong hệ thống.

**Khó khăn và bài học:** Việc xác định đầy đủ thông tin của một bằng chứng cần tham khảo nhiều tài liệu và trao đổi với các thành viên trong nhóm. Tôi nhận thấy việc phân tích yêu cầu kỹ lưỡng sẽ giúp giảm thời gian chỉnh sửa khi lập trình.

## Ngày 2 - 2/6: Tích hợp Amazon S3 để lưu trữ bằng chứng

**Công việc đã thực hiện:** Tôi tiến hành tích hợp Amazon S3 vào hệ thống để lưu trữ các tệp bằng chứng. Tôi tạo Bucket riêng cho dự án, xây dựng cấu trúc thư mục lưu trữ và cấu hình IAM Role để Lambda có thể truy cập S3 một cách an toàn.

**Kiến thức đã học:** Tôi hiểu Amazon S3 phù hợp để lưu trữ các tệp dung lượng lớn thay vì lưu trực tiếp trong cơ sở dữ liệu. Việc lưu đường dẫn tệp trong DynamoDB giúp hệ thống hoạt động hiệu quả và giảm chi phí lưu trữ.

**Kết quả đạt được:** Hệ thống có thể tải tệp lên Amazon S3 và lưu thông tin đường dẫn của tệp trong cơ sở dữ liệu.

**Khó khăn và bài học:** Ban đầu Lambda chưa thể ghi dữ liệu lên S3 do thiếu quyền truy cập. Sau khi cập nhật IAM Policy và kiểm tra Bucket Policy, việc tải tệp đã hoạt động bình thường.

## Ngày 3 - 3/6: Upload và quản lý nhiều loại tệp

**Công việc đã thực hiện:** Tôi mở rộng chức năng Upload để hỗ trợ nhiều định dạng như hình ảnh, file log và tài liệu PDF. Đồng thời xây dựng quy tắc đặt tên tệp theo Incident ID nhằm tránh trùng lặp và thuận tiện cho việc tìm kiếm sau này.

**Kiến thức đã học:** Tôi hiểu việc tổ chức dữ liệu trên S3 theo thư mục và quy tắc đặt tên sẽ giúp việc quản lý hàng nghìn tệp trở nên dễ dàng hơn. Tôi cũng tìm hiểu cách xác thực định dạng tệp trước khi cho phép tải lên.

**Kết quả đạt được:** Chức năng Upload hoạt động ổn định với nhiều loại tệp khác nhau và dữ liệu được lưu đúng vị trí trên S3.

**Khó khăn và bài học:** Trong quá trình kiểm thử, một số tệp có kích thước lớn khiến thời gian tải lên lâu hơn dự kiến. Tôi học được cách xử lý ngoại lệ và hiển thị thông báo tiến trình để cải thiện trải nghiệm người dùng.

## Ngày 4 - 4/6: Kiểm thử chức năng Evidence Management

**Công việc đã thực hiện:** Tôi thực hiện kiểm thử toàn bộ chức năng Evidence Management, bao gồm tạo mới bằng chứng, tải tệp lên S3, xem danh sách bằng chứng và xóa dữ liệu không còn sử dụng. Tôi cũng phối hợp với các thành viên trong nhóm để kiểm tra tính ổn định của hệ thống.

**Kiến thức đã học:** Tôi hiểu tầm quan trọng của việc kiểm thử sau khi hoàn thành từng chức năng. Việc kiểm thử sớm giúp phát hiện lỗi về quyền truy cập, dữ liệu và luồng xử lý trước khi tích hợp với các thành phần khác.

**Kết quả đạt được:** Chức năng quản lý bằng chứng hoạt động đúng yêu cầu, dữ liệu được lưu trữ và truy xuất thành công từ Amazon S3.

**Khó khăn và bài học:** Một số lỗi phát sinh do dữ liệu đầu vào chưa được kiểm tra đầy đủ. Tôi bổ sung bước kiểm tra dữ liệu trước khi Upload nhằm hạn chế lỗi trong quá trình sử dụng.

## Ngày 5 - 05/06: Nghiên cứu thêm các dịch vụ AWS và tổng kết tuần

**Công việc đã thực hiện:** Tôi dành thời gian tìm hiểu thêm các dịch vụ hỗ trợ cho hệ thống như Amazon CloudWatch để theo dõi log, AWS CloudTrail để ghi nhận hoạt động và AWS Secrets Manager để quản lý thông tin nhạy cảm. Cuối ngày, tôi tổng hợp lại toàn bộ kiến thức đã học trong tuần và cập nhật tài liệu kỹ thuật của dự án.

**Kiến thức đã học:** Tôi hiểu vai trò của các dịch vụ giám sát và bảo mật trong việc vận hành hệ thống trên AWS. CloudWatch hỗ trợ theo dõi log và hiệu năng, CloudTrail ghi nhận lịch sử thao tác trên tài khoản AWS, còn Secrets Manager giúp lưu trữ an toàn các thông tin như API Key và mật khẩu.

**Kết quả đạt được:** Tôi mở rộng kiến thức về hệ sinh thái AWS, hoàn thiện chức năng Evidence Management và chuẩn bị nền tảng cho việc phát triển giao diện người dùng ở tuần tiếp theo.

**Khó khăn và bài học:** AWS có rất nhiều dịch vụ liên quan nên việc lựa chọn dịch vụ phù hợp với từng bài toán là điều quan trọng. Tôi nhận thấy cần đọc tài liệu chính thức và thực hành thường xuyên để hiểu rõ chức năng của từng dịch vụ.