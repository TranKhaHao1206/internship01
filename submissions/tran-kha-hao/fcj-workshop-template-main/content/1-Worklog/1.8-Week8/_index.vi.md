---
title: "Tuần 8"
date: 2026-06-08
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

**Mốc thời gian:** 8/6 → 14/6 (5 ngày làm việc)

## Ngày 1 - 8/6: Khởi tạo dự án ReactJS

**Công việc đã thực hiện:** Tôi bắt đầu phát triển giao diện người dùng (Frontend) cho hệ thống Incident Response Management System (IRMS) bằng ReactJS. Tôi khởi tạo dự án, tổ chức cấu trúc thư mục theo từng module như Components, Pages, Services và Assets. Đồng thời cài đặt các thư viện cần thiết như React Router, Axios và Material UI để phục vụ quá trình phát triển.

**Kiến thức đã học:** Tôi hiểu ReactJS là thư viện JavaScript được sử dụng để xây dựng giao diện theo mô hình Component-Based. Việc chia nhỏ giao diện thành các Component giúp mã nguồn dễ bảo trì, tái sử dụng và mở rộng khi hệ thống phát triển.

**Kết quả đạt được:** Hoàn thành việc khởi tạo dự án ReactJS và xây dựng cấu trúc thư mục phù hợp với quy mô của hệ thống.

**Khó khăn và bài học:** Ban đầu tôi còn bối rối trong việc tổ chức thư mục dự án. Sau khi tham khảo các mô hình React phổ biến, tôi lựa chọn cấu trúc rõ ràng để thuận tiện cho việc phát triển lâu dài.

## Ngày 2 - 9/6: Thiết kế giao diện Dashboard

**Công việc đã thực hiện:** Tôi tiến hành xây dựng giao diện Dashboard hiển thị tổng quan về các Incident trong hệ thống. Dashboard bao gồm số lượng Incident, trạng thái xử lý, mức độ nghiêm trọng và các thông tin thống kê cơ bản. Tôi sử dụng Material UI để xây dựng giao diện đồng nhất và dễ sử dụng.

**Kiến thức đã học:** Tôi hiểu Dashboard là màn hình tổng quan giúp người dùng nhanh chóng theo dõi tình trạng của hệ thống. Việc trình bày dữ liệu trực quan sẽ giúp người quản trị đưa ra quyết định nhanh hơn khi xảy ra sự cố.

**Kết quả đạt được:** Hoàn thành giao diện Dashboard với các thành phần thống kê cơ bản và bố cục rõ ràng.

**Khó khăn và bài học:** Việc sắp xếp bố cục giao diện cần đảm bảo tính trực quan và dễ quan sát. Tôi học được cách ưu tiên hiển thị những thông tin quan trọng nhất ở vị trí nổi bật.

## Ngày 3 - 10/6: Xây dựng Incident List và Incident Detail

**Công việc đã thực hiện:** Tôi phát triển giao diện danh sách Incident và trang chi tiết Incident. Màn hình Incident List hiển thị danh sách các sự cố theo dạng bảng với các thông tin như tiêu đề, mức độ nghiêm trọng, trạng thái và thời gian tạo. Khi chọn một Incident, người dùng sẽ được chuyển đến màn hình Incident Detail để xem thông tin chi tiết.

**Kiến thức đã học:** Tôi hiểu cách quản lý dữ liệu trong React bằng State và Props, đồng thời sử dụng React Router để điều hướng giữa các trang. Tôi cũng tìm hiểu cách hiển thị dữ liệu động từ API lên giao diện.

**Kết quả đạt được:** Hoàn thành hai màn hình chính của hệ thống và xây dựng thành công luồng điều hướng giữa các trang.

**Khó khăn và bài học:** Việc quản lý State giữa nhiều Component khá phức tạp. Tôi học được cách chia nhỏ Component và truyền dữ liệu hợp lý để giảm sự phụ thuộc giữa các thành phần.

## Ngày 4 - 11/6: Thiết kế Timeline và Evidence Upload

**Công việc đã thực hiện:** Tôi tiếp tục phát triển giao diện Timeline để hiển thị lịch sử xử lý Incident theo trình tự thời gian. Đồng thời xây dựng giao diện Evidence Upload cho phép người dùng tải lên các file log, hình ảnh và tài liệu PDF liên quan đến sự cố.

**Kiến thức đã học:** Tôi hiểu việc trình bày Timeline giúp người quản trị dễ dàng theo dõi toàn bộ quá trình xử lý sự cố. Tôi cũng tìm hiểu cách sử dụng FormData trong React để gửi tệp lên API.

**Kết quả đạt được:** Hoàn thiện giao diện Timeline và màn hình Upload Evidence với đầy đủ các trường thông tin cần thiết.

**Khó khăn và bài học:** Việc xử lý Upload File cần kiểm tra định dạng và kích thước tệp trước khi gửi lên máy chủ. Tôi bổ sung các thông báo lỗi để người dùng dễ dàng nhận biết khi thao tác không hợp lệ.

## Ngày 5 - 12/6: Kết nối Frontend với API Gateway và Cognito

**Công việc đã thực hiện:** Tôi tiến hành kết nối giao diện ReactJS với các REST API đã xây dựng thông qua Amazon API Gateway. Đồng thời tích hợp Amazon Cognito để thực hiện xác thực người dùng bằng JWT Token trước khi gọi các API. Tôi kiểm thử toàn bộ luồng đăng nhập và truy xuất dữ liệu từ giao diện.

**Kiến thức đã học:** Tôi hiểu cách sử dụng Axios để gửi HTTP Request đến API Gateway và cách đính kèm JWT Token vào Header Authorization nhằm xác thực người dùng. Tôi cũng hiểu quy trình Frontend giao tiếp với Backend trong kiến trúc Serverless.

**Kết quả đạt được:** Giao diện ReactJS có thể đăng nhập bằng Cognito, gọi API thành công và hiển thị dữ liệu Incident từ hệ thống.

**Khó khăn và bài học:** Trong quá trình kết nối API, tôi gặp lỗi CORS và Token hết hạn. Sau khi kiểm tra cấu hình API Gateway và bổ sung cơ chế xử lý Token, hệ thống hoạt động ổn định hơn. Tôi nhận thấy việc kiểm thử toàn bộ luồng Frontend - Backend rất quan trọng để đảm bảo trải nghiệm người dùng.