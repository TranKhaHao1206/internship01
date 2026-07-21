---
title: "Tuần 9"
date: 2026-06-15
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

**Mốc thời gian:** 15/6 → 21/6 (5 ngày làm việc)

## Ngày 1 - 15/6: Hoàn thiện Dashboard theo dõi Incident

**Công việc đã thực hiện:** Tôi tiếp tục hoàn thiện giao diện Dashboard của hệ thống Incident Response Management System (IRMS). Tôi bổ sung các thẻ thống kê (Summary Cards) hiển thị tổng số Incident, Incident đang xử lý, Incident đã hoàn thành và Incident quá hạn. Đồng thời tối ưu bố cục giao diện để người dùng có thể quan sát nhanh tình trạng của hệ thống.

**Kiến thức đã học:** Tôi hiểu Dashboard không chỉ hiển thị dữ liệu mà còn phải hỗ trợ người quản trị đưa ra quyết định nhanh chóng. Việc sắp xếp thông tin theo mức độ ưu tiên giúp tăng khả năng theo dõi và xử lý sự cố.

**Kết quả đạt được:** Dashboard hiển thị đầy đủ các thông tin tổng quan và cập nhật dữ liệu từ API theo thời gian thực.

**Khó khăn và bài học:** Việc sắp xếp nhiều thành phần trên cùng một màn hình dễ gây rối mắt. Tôi học được cách nhóm các thông tin liên quan và sử dụng bố cục hợp lý để tăng tính trực quan.

## Ngày 2 - 16/6: Xây dựng chức năng phân loại mức độ nghiêm trọng

**Công việc đã thực hiện:** Tôi phát triển chức năng phân loại mức độ nghiêm trọng của Incident theo ba mức: Critical, High và Medium. Tôi cập nhật cơ sở dữ liệu, bổ sung trường Severity và xây dựng giao diện để hiển thị mức độ của từng Incident bằng màu sắc khác nhau.

**Kiến thức đã học:** Tôi hiểu việc phân loại mức độ nghiêm trọng giúp đội ngũ bảo mật ưu tiên xử lý các sự cố có ảnh hưởng lớn trước, từ đó giảm thiểu rủi ro đối với hệ thống.

**Kết quả đạt được:** Người dùng có thể lựa chọn mức độ nghiêm trọng khi tạo Incident và hệ thống hiển thị thông tin rõ ràng trên Dashboard cũng như danh sách Incident.

**Khó khăn và bài học:** Ban đầu tôi chỉ lưu giá trị dạng chuỗi nên khó kiểm soát khi mở rộng hệ thống. Sau khi trao đổi với nhóm, tôi chuẩn hóa dữ liệu để thuận tiện cho việc xử lý sau này.

## Ngày 3 - 17/6: Cải thiện giao diện người dùng

**Công việc đã thực hiện:** Tôi rà soát toàn bộ giao diện của hệ thống, điều chỉnh khoảng cách giữa các thành phần, cải thiện màu sắc, biểu tượng và bố cục của các trang Dashboard, Incident List và Incident Detail. Tôi cũng bổ sung các thông báo khi tải dữ liệu và khi xảy ra lỗi để nâng cao trải nghiệm người dùng.

**Kiến thức đã học:** Tôi hiểu giao diện thân thiện sẽ giúp người dùng thao tác nhanh hơn và giảm sai sót trong quá trình sử dụng. Ngoài chức năng, tính trực quan cũng là yếu tố rất quan trọng đối với một ứng dụng Web.

**Kết quả đạt được:** Giao diện hệ thống đồng nhất hơn, dễ sử dụng và hiển thị tốt trên nhiều kích thước màn hình.

**Khó khăn và bài học:** Một số thành phần chưa tương thích khi hiển thị trên màn hình nhỏ. Tôi học được cách sử dụng Responsive Design để giao diện hoạt động ổn định trên nhiều thiết bị.

## Ngày 4 - 18/6: Kiểm thử luồng xử lý Incident

**Công việc đã thực hiện:** Tôi tiến hành kiểm thử toàn bộ quy trình xử lý Incident từ khi tạo mới, cập nhật thông tin, thay đổi trạng thái cho đến khi hoàn thành. Tôi sử dụng Postman và giao diện Web để kiểm tra dữ liệu giữa Frontend và Backend, đồng thời ghi nhận các lỗi phát sinh trong quá trình thao tác.

**Kiến thức đã học:** Tôi hiểu việc kiểm thử theo từng luồng nghiệp vụ giúp phát hiện lỗi sớm và đảm bảo các chức năng hoạt động đúng như yêu cầu thiết kế.

**Kết quả đạt được:** Hoàn thành kiểm thử các chức năng chính của hệ thống và khắc phục một số lỗi liên quan đến dữ liệu hiển thị và xử lý trạng thái.

**Khó khăn và bài học:** Một số lỗi chỉ xuất hiện khi thực hiện nhiều thao tác liên tiếp. Tôi học được cách xây dựng các kịch bản kiểm thử đầy đủ thay vì chỉ kiểm tra từng chức năng riêng lẻ.

## Ngày 5 - 19/6: Kiểm tra phân quyền người dùng và tổng kết tuần

**Công việc đã thực hiện:** Tôi kiểm tra cơ chế phân quyền người dùng dựa trên các vai trò đã thiết kế ở tuần trước như Admin, Security Manager, Security Analyst và Auditor. Tôi xác minh quyền truy cập của từng vai trò đối với các chức năng như tạo Incident, chỉnh sửa thông tin, tải bằng chứng và xem báo cáo. Cuối ngày, tôi tổng hợp kết quả làm việc và cập nhật tài liệu kỹ thuật của dự án.

**Kiến thức đã học:** Tôi hiểu việc kiểm soát quyền truy cập là yếu tố quan trọng để đảm bảo an toàn thông tin. Mỗi vai trò chỉ nên được phép thực hiện các thao tác phù hợp với nhiệm vụ của mình nhằm tuân thủ nguyên tắc Least Privilege.

**Kết quả đạt được:** Hệ thống phân quyền hoạt động đúng theo thiết kế, các API được bảo vệ bằng JWT Token của Amazon Cognito và giao diện hiển thị chức năng phù hợp với từng vai trò người dùng.

**Khó khăn và bài học:** Trong quá trình kiểm thử, tôi phát hiện một số chức năng vẫn hiển thị với người dùng không có quyền. Sau khi điều chỉnh điều kiện hiển thị trên Frontend và kiểm tra lại quyền ở Backend, hệ thống hoạt động ổn định hơn. Tôi nhận thấy việc kiểm tra đồng thời ở cả giao diện và API là rất cần thiết để đảm bảo tính bảo mật.