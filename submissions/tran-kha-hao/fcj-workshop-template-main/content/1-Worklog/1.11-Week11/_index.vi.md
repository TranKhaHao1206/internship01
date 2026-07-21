---
title: "Tuần 11"
date: 2026-06-29
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

**Mốc thời gian:** 29/6 → 5/7 (5 ngày làm việc)

## Ngày 1 - 29/6: Thiết kế Test Case và lập kế hoạch kiểm thử

**Công việc đã thực hiện:** Tôi bắt đầu giai đoạn kiểm thử hệ thống bằng cách phân tích các chức năng đã hoàn thành và xây dựng bộ Test Case. Tôi xác định các kịch bản kiểm thử cho từng chức năng như đăng nhập, quản lý Incident, quản lý Evidence, phân quyền người dùng, báo cáo và AI Assistant. Đồng thời tôi lập kế hoạch kiểm thử để đảm bảo tất cả các chức năng đều được đánh giá đầy đủ.

**Kiến thức đã học:** Tôi hiểu Test Case là tài liệu mô tả các bước thực hiện, dữ liệu đầu vào, kết quả mong đợi và kết quả thực tế của từng chức năng. Một bộ Test Case đầy đủ giúp quá trình kiểm thử có hệ thống và dễ dàng theo dõi lỗi phát sinh.

**Kết quả đạt được:** Hoàn thành bộ Test Case cho các chức năng chính của hệ thống và thống nhất kế hoạch kiểm thử cùng các thành viên trong nhóm.

**Khó khăn và bài học:** Việc xây dựng Test Case cần bao quát cả trường hợp hợp lệ và không hợp lệ. Tôi học được cách suy nghĩ theo góc nhìn của người dùng để xây dựng các tình huống kiểm thử thực tế hơn.

## Ngày 2 - 30/6: Kiểm thử Authentication và CRUD

**Công việc đã thực hiện:** Tôi tiến hành kiểm thử chức năng Authentication sử dụng Amazon Cognito, bao gồm đăng nhập, đăng xuất, xác thực JWT Token và kiểm tra quyền truy cập của từng vai trò. Sau đó, tôi kiểm thử các chức năng CRUD đối với Incident và Evidence để đảm bảo dữ liệu được xử lý chính xác.

**Kiến thức đã học:** Tôi hiểu việc kiểm thử không chỉ kiểm tra chức năng hoạt động mà còn phải xác minh tính bảo mật và tính toàn vẹn của dữ liệu. Tôi cũng hiểu cách sử dụng Postman để kiểm thử API độc lập với giao diện.

**Kết quả đạt được:** Các chức năng Authentication và CRUD hoạt động ổn định, dữ liệu được lưu trữ và truy xuất chính xác theo yêu cầu.

**Khó khăn và bài học:** Một số API trả về thông báo lỗi chưa rõ ràng khi Token hết hạn. Tôi bổ sung cơ chế xử lý lỗi và hiển thị thông báo phù hợp để người dùng dễ nhận biết.

## Ngày 3 - 1/7: Kiểm thử Upload Evidence, Reports và AI Assistant

**Công việc đã thực hiện:** Tôi tiếp tục kiểm thử chức năng Upload Evidence bằng nhiều loại tệp khác nhau như hình ảnh, PDF và file log. Đồng thời kiểm tra chức năng tạo Report và AI Assistant nhằm đánh giá khả năng hoạt động của toàn bộ hệ thống trong các tình huống thực tế.

**Kiến thức đã học:** Tôi hiểu việc kiểm thử nhiều loại dữ liệu đầu vào sẽ giúp phát hiện các lỗi liên quan đến định dạng, kích thước tệp và xử lý ngoại lệ. Tôi cũng nhận thấy AI Assistant cần được kiểm tra với nhiều câu hỏi khác nhau để đánh giá chất lượng phản hồi.

**Kết quả đạt được:** Chức năng Upload Evidence và Reports hoạt động ổn định. AI Assistant có thể phản hồi đúng với các câu hỏi thuộc phạm vi dữ liệu của hệ thống.

**Khó khăn và bài học:** Một số tệp có dung lượng lớn làm thời gian Upload tăng lên. Tôi học được cách kiểm tra giới hạn kích thước tệp và tối ưu quá trình tải dữ liệu lên Amazon S3.

## Ngày 4 - 2/7: Ghi nhận và xử lý lỗi

**Công việc đã thực hiện:** Sau khi hoàn thành kiểm thử, tôi tổng hợp toàn bộ lỗi phát hiện được và phân loại theo mức độ ưu tiên. Tôi phối hợp với các thành viên trong nhóm để xác định nguyên nhân, chỉnh sửa mã nguồn và kiểm thử lại sau khi khắc phục nhằm đảm bảo lỗi không còn xuất hiện.

**Kiến thức đã học:** Tôi hiểu quy trình xử lý lỗi trong dự án phần mềm gồm phát hiện, ghi nhận, phân tích nguyên nhân, sửa lỗi và kiểm thử lại. Việc lưu lại thông tin chi tiết của từng lỗi giúp nhóm dễ dàng theo dõi tiến độ và tránh lặp lại lỗi tương tự.

**Kết quả đạt được:** Phần lớn các lỗi được khắc phục thành công và hệ thống hoạt động ổn định hơn sau khi kiểm thử lại.

**Khó khăn và bài học:** Một số lỗi chỉ xuất hiện trong những điều kiện đặc biệt nên mất nhiều thời gian để tái hiện. Tôi nhận thấy cần xây dựng các kịch bản kiểm thử đa dạng để phát hiện lỗi sớm hơn.

## Ngày 5 - 3/7: Xây dựng tài liệu kỹ thuật

**Công việc đã thực hiện:** Tôi hoàn thiện bộ tài liệu kỹ thuật của dự án, bao gồm API Documentation, Architecture Diagram, Sequence Diagram và Use Case Diagram. Tôi mô tả chi tiết các API, phương thức HTTP, tham số đầu vào, dữ liệu trả về và luồng xử lý của hệ thống. Đồng thời cập nhật các sơ đồ để phản ánh đúng kiến trúc sau khi hoàn thành quá trình phát triển.

**Kiến thức đã học:** Tôi hiểu tài liệu kỹ thuật là thành phần không thể thiếu trong một dự án phần mềm, giúp các thành viên mới dễ dàng tiếp cận hệ thống và hỗ trợ công tác bảo trì sau này. Việc chuẩn hóa tài liệu cũng giúp quá trình bàn giao dự án trở nên thuận lợi hơn.

**Kết quả đạt được:** Hoàn thiện bộ tài liệu kỹ thuật phục vụ quá trình kiểm thử, nghiệm thu và chuẩn bị cho buổi Demo dự án.

**Khó khăn và bài học:** Việc cập nhật tài liệu cần được thực hiện song song với quá trình phát triển để tránh thiếu sót. Tôi nhận thấy tài liệu càng rõ ràng thì việc trao đổi giữa các thành viên và giảng viên hướng dẫn càng hiệu quả.
