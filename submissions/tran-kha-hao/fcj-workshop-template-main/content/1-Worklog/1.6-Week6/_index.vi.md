---
title: "Tuần 6"
date: 2026-05-25
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

**Mốc thời gian:** 25/5 → 31/5 (5 ngày làm việc)

## Ngày 1 - 25/5: Nghiên cứu Amazon API Gateway

**Công việc đã thực hiện:** Tôi bắt đầu nghiên cứu Amazon API Gateway để xây dựng các REST API cho hệ thống Incident Response Management System (IRMS). Tôi tìm hiểu các thành phần của API Gateway như API, Resource, Method, Stage và Deployment. Đồng thời, tôi thực hành tạo API đầu tiên và gửi yêu cầu kiểm thử bằng Postman.

**Kiến thức đã học:** Tôi hiểu API Gateway là dịch vụ tiếp nhận yêu cầu từ phía Client, thực hiện xác thực, định tuyến yêu cầu đến AWS Lambda và trả kết quả về cho ứng dụng. Dịch vụ này giúp quản lý API tập trung, dễ mở rộng và tăng cường bảo mật.

**Kết quả đạt được:** Tôi tạo thành công REST API đầu tiên trên API Gateway và thực hiện kiểm thử thông qua Postman.

**Khó khăn và bài học:** Ban đầu tôi chưa hiểu mối quan hệ giữa Resource và Method trong API Gateway. Sau khi thực hành nhiều lần, tôi đã nắm được cách tổ chức API theo từng chức năng.

## Ngày 2 - 26/5: Xây dựng REST API cho hệ thống IRMS

**Công việc đã thực hiện:** Tôi tiến hành xây dựng các API phục vụ hệ thống IRMS như lấy danh sách Incident, tạo Incident mới, cập nhật thông tin và xóa dữ liệu. Tôi thiết kế các Endpoint theo chuẩn RESTful để đảm bảo dễ bảo trì và mở rộng trong tương lai.

**Kiến thức đã học:** Tôi hiểu nguyên tắc thiết kế REST API, cách sử dụng các phương thức HTTP như GET, POST, PUT và DELETE, cũng như quy ước đặt URL cho từng tài nguyên trong hệ thống.

**Kết quả đạt được:** Hoàn thành các Endpoint cơ bản phục vụ việc quản lý Incident và chuẩn bị tích hợp với Lambda.

**Khó khăn và bài học:** Việc thiết kế API cần thống nhất ngay từ đầu để tránh phải sửa đổi nhiều khi phát triển hệ thống. Tôi học được cách đặt tên Endpoint rõ ràng và nhất quán.

## Ngày 3 - 27/5: Cấu hình Route, Method và tích hợp với AWS Lambda

**Công việc đã thực hiện:** Tôi cấu hình Route và Method trên API Gateway, sau đó tích hợp từng API với các Lambda Function đã xây dựng ở tuần trước. Tôi kiểm tra việc truyền dữ liệu giữa Client, API Gateway và Lambda bằng Postman để đảm bảo luồng xử lý hoạt động chính xác.

**Kiến thức đã học:** Tôi hiểu quy trình xử lý yêu cầu trong kiến trúc Serverless gồm Client → API Gateway → Lambda → DynamoDB → Response. Đồng thời tôi hiểu cách truyền dữ liệu thông qua Event Object của Lambda.

**Kết quả đạt được:** Các API có thể gọi thành công Lambda Function và trả về dữ liệu đúng định dạng JSON.

**Khó khăn và bài học:** Trong quá trình tích hợp, tôi gặp lỗi do Lambda chưa được cấp quyền Invoke từ API Gateway. Sau khi bổ sung quyền và triển khai lại API, hệ thống hoạt động bình thường.

## Ngày 4 - 28/5: Tìm hiểu Amazon S3

**Công việc đã thực hiện:** Tôi nghiên cứu Amazon Simple Storage Service (S3) để chuẩn bị cho việc lưu trữ file của hệ thống. Tôi thực hành tạo Bucket, cấu hình quyền truy cập, tải lên và tải xuống các tệp mẫu, đồng thời tìm hiểu cách quản lý đối tượng trong S3.

**Kiến thức đã học:** Tôi hiểu Amazon S3 là dịch vụ lưu trữ đối tượng của AWS với độ bền và khả năng mở rộng rất cao. Tôi cũng biết cách tổ chức dữ liệu theo Bucket và Object, cũng như các nguyên tắc bảo mật khi quản lý tệp trên Cloud.

**Kết quả đạt được:** Tôi tạo thành công S3 Bucket và thực hiện các thao tác Upload, Download và Delete đối với các tệp thử nghiệm.

**Khó khăn và bài học:** Ban đầu tôi gặp lỗi truy cập do cấu hình quyền Bucket chưa phù hợp. Tôi rút ra kinh nghiệm cần kiểm tra IAM Policy và Bucket Policy trước khi triển khai.

## Ngày 5 - 29/5: Tham gia hội thảo AWS và tổng kết tuần

**Công việc đã thực hiện:** Tôi tham gia buổi hội thảo do AWS tổ chức để tìm hiểu thêm về các dịch vụ Cloud và xu hướng phát triển Serverless. Các chuyên gia chia sẻ kinh nghiệm triển khai hệ thống thực tế trên AWS, cách tối ưu chi phí và nâng cao bảo mật. Sau buổi hội thảo, tôi tổng hợp lại kiến thức đã học trong tuần và cập nhật tài liệu kỹ thuật của dự án.

**Kiến thức đã học:** Tôi hiểu rõ hơn về các mô hình triển khai Serverless, các nguyên tắc thiết kế kiến trúc Cloud hiện đại và cách lựa chọn dịch vụ AWS phù hợp với từng bài toán thực tế. Ngoài ra, tôi cũng học được nhiều kinh nghiệm triển khai từ các chuyên gia AWS.

**Kết quả đạt được:** Tôi mở rộng kiến thức về hệ sinh thái AWS, hoàn thiện các REST API cơ bản của hệ thống và chuẩn bị nền tảng để phát triển các chức năng nghiệp vụ ở tuần tiếp theo.

**Khó khăn và bài học:** Khối lượng kiến thức trong hội thảo khá lớn nên tôi cần ghi chú lại những nội dung quan trọng để nghiên cứu thêm. Tôi nhận thấy việc tham gia các sự kiện chuyên môn giúp cập nhật công nghệ mới và nâng cao tư duy thiết kế hệ thống trên nền tảng Cloud.