---
title: "Tuần 2"
date: 2026-04-27
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

**Mốc thời gian:** 27/4 → 3/5 (5 ngày làm việc)

## Ngày 1 - 27/4: AWS IAM Fundamentals

**Công việc đã thực hiện:** Tôi bắt đầu tuần thứ hai bằng việc tìm hiểu dịch vụ AWS Identity and Access Management (IAM). Tôi nghiên cứu các thành phần cơ bản gồm IAM User, IAM Group, IAM Role và IAM Policy. Đồng thời, tôi tạo một số IAM User thử nghiệm để quan sát sự khác biệt giữa tài khoản Root và tài khoản IAM, từ đó hiểu cách AWS quản lý danh tính và quyền truy cập.

**Kiến thức đã học:** Tôi hiểu IAM là dịch vụ quản lý danh tính và phân quyền trung tâm của AWS. Root Account có toàn quyền đối với tài khoản AWS nên chỉ nên sử dụng khi thực sự cần thiết. Trong khi đó, IAM User được tạo để phục vụ cho người dùng hoặc quản trị viên trong quá trình làm việc hằng ngày.

**Kết quả đạt được:** Tôi phân biệt được vai trò của Root Account và IAM User, đồng thời tạo thành công các IAM User phục vụ cho việc thực hành.

**Khó khăn và bài học:** Ban đầu tôi còn nhầm lẫn giữa Root Account và IAM User. Sau khi thực hành trực tiếp trên AWS Console, tôi nhận thấy việc sử dụng IAM User giúp tăng tính bảo mật và dễ quản lý hơn.

## Ngày 2 - 28/4: Quản lý Group và Policy

**Công việc đã thực hiện:** Tôi tiếp tục tìm hiểu về IAM Group và IAM Policy. Tôi thực hành tạo nhiều Group với các quyền khác nhau, sau đó gán User vào từng Group để quan sát cách quyền được kế thừa. Đồng thời, tôi nghiên cứu cấu trúc của Policy dạng JSON và đọc ý nghĩa của các trường như Version, Effect, Action, Resource và Condition.

**Kiến thức đã học:** Tôi hiểu Policy là tập hợp các quyền được mô tả dưới dạng JSON. Group giúp quản lý quyền cho nhiều User cùng lúc thay vì phải cấu hình từng User riêng lẻ, giúp việc quản trị hệ thống trở nên thuận tiện hơn.

**Kết quả đạt được:** Tôi tạo thành công các Group và gán Policy phù hợp cho từng Group. Đồng thời đọc và hiểu được cấu trúc cơ bản của một IAM Policy.

**Khó khăn và bài học:** Policy JSON có khá nhiều thành phần nên ban đầu hơi khó đọc. Tôi rút ra kinh nghiệm nên đọc từng trường và kết hợp với tài liệu AWS để hiểu rõ chức năng của từng quyền.

## Ngày 3 - 29/4: IAM Role và nguyên tắc Least Privilege

**Công việc đã thực hiện:** Tôi tìm hiểu IAM Role và sự khác biệt giữa Role với User. Tôi thực hành tạo Role cho dịch vụ AWS và tìm hiểu các trường hợp sử dụng Role trong EC2, Lambda và các dịch vụ khác. Đồng thời nghiên cứu nguyên tắc Least Privilege nhằm chỉ cấp đúng quyền cần thiết cho từng đối tượng sử dụng.

**Kiến thức đã học:** Tôi hiểu IAM Role không đại diện cho một người dùng cụ thể mà được sử dụng để cấp quyền tạm thời cho người dùng hoặc dịch vụ AWS. Nguyên tắc Least Privilege giúp giảm thiểu rủi ro bảo mật bằng cách chỉ cấp các quyền cần thiết để hoàn thành công việc.

**Kết quả đạt được:** Tôi tạo được IAM Role cơ bản và hiểu khi nào nên sử dụng User, Group hoặc Role trong từng tình huống.

**Khó khăn và bài học:** Việc xác định quyền tối thiểu phù hợp cho từng Role không đơn giản. Tôi học được rằng nên cấp quyền từ mức nhỏ nhất rồi mở rộng khi thực sự cần thiết.

## Ngày 4 - 30/4: Region, Availability Zone và Edge Location

**Công việc đã thực hiện:** Tôi nghiên cứu kiến trúc hạ tầng toàn cầu của AWS, bao gồm Region, Availability Zone (AZ) và Edge Location. Tôi tìm hiểu cách lựa chọn Region phù hợp với vị trí địa lý, độ trễ mạng và yêu cầu triển khai hệ thống.

**Kiến thức đã học:** Tôi hiểu Region là khu vực triển khai dịch vụ AWS, mỗi Region gồm nhiều Availability Zone độc lập nhằm đảm bảo tính sẵn sàng cao. Edge Location được sử dụng để tăng tốc độ phân phối nội dung thông qua mạng CDN của AWS.

**Kết quả đạt được:** Tôi nắm được cách lựa chọn Region phù hợp và hiểu vai trò của Availability Zone trong việc xây dựng hệ thống có khả năng chịu lỗi cao.

**Khó khăn và bài học:** Ban đầu tôi chưa phân biệt rõ Region và Availability Zone. Sau khi xem sơ đồ kiến trúc AWS, tôi hiểu được mối quan hệ giữa hai thành phần này.

## Ngày 5 - 1/5: Ôn tập và thực hành IAM

**Công việc đã thực hiện:** Tôi dành thời gian tổng hợp lại toàn bộ kiến thức đã học trong tuần, thực hành tạo User, Group, Role và Policy trên AWS Console. Đồng thời kiểm tra lại các quyền đã cấp và thử nghiệm một số trường hợp truy cập khác nhau để hiểu rõ cơ chế kiểm soát quyền của AWS.

**Kiến thức đã học:** Tôi củng cố kiến thức về IAM và hiểu được quy trình quản lý quyền truy cập trong môi trường Cloud. Tôi cũng nhận thức rõ tầm quan trọng của việc áp dụng nguyên tắc Least Privilege trong các hệ thống thực tế.

**Kết quả đạt được:** Hoàn thành các bài thực hành IAM cơ bản và có thể tự tạo, quản lý User, Group, Role và Policy trên AWS.

**Khó khăn và bài học:** Tôi nhận thấy việc đặt tên tài nguyên và tổ chức Policy theo quy tắc rõ ràng sẽ giúp việc quản trị hệ thống dễ dàng hơn khi số lượng người dùng và tài nguyên tăng lên.
