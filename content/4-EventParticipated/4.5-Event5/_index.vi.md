---
title: "Event 5"
date: "2025-11-29"
weight: 5
chapter: false
pre: " <b> 4.5. </b> "
---

# Báo cáo tóm tắt: “AWS Well-Architected Security Pillar”

### Mục tiêu sự kiện

- **Quản lý danh tính và truy cập (IAM)**: Khám phá kiến trúc IAM hiện đại, nhấn mạnh tầm quan trọng của việc tránh sử dụng thông tin xác thực dài hạn và tận dụng AWS Identity Center để có thông tin xác thực ngắn hạn.
- **Phát hiện và giám sát liên tục**: Làm nổi bật tầm quan trọng của khả năng hiển thị bảo mật đa tầng và các cơ chế phát hiện tự động.
- **Bảo vệ cơ sở hạ tầng**: Thảo luận về các chiến lược bảo mật mạng và khối lượng công việc, bao gồm phân đoạn và bảo vệ khối lượng công việc.
- **Bảo vệ dữ liệu**: Hiểu các phương pháp mã hóa, quản lý khóa và luân chuyển bí mật.
- **Phản hồi sự cố**: Tìm hiểu về vòng đời IR và các kỹ thuật tự động hóa để xử lý sự cố hiệu quả.

### Điểm nổi bật chính

#### Trụ cột 1 — Quản lý danh tính và truy cập
- **Kiến trúc IAM hiện đại**: Được trình bày bởi Huỳnh Hoàng Long và Aiden, phiên họp này đề cập đến người dùng IAM, vai trò và chính sách, nhấn mạnh việc tránh sử dụng thông tin xác thực dài hạn. AWS Identity Center đã được giới thiệu để đăng nhập một lần (SSO) và tập hợp quyền.
- **SCP & Ranh giới quyền**: Giải thích vai trò của Chính sách Kiểm soát Dịch vụ (SCP) trong việc quản lý môi trường nhiều tài khoản. SCP lọc quyền nhưng không cấp quyền.
- **MFA & Luân chuyển thông tin xác thực**: So sánh TOTP và FIDO2 cho xác thực đa yếu tố. Các khuyến nghị bao gồm tránh người dùng IAM với khóa dài hạn và sử dụng AWS Identity Center để có thông tin xác thực ngắn hạn.
- **Access Analyzer**: Trình bày cách xác thực chính sách IAM và mô phỏng quyền truy cập.
- **Mini Demo**: Xác thực chính sách IAM và mô phỏng các kịch bản truy cập.

#### Trụ cột 2 — Phát hiện
- **Phát hiện và giám sát liên tục**: Được trình bày bởi Trần Đức Anh, Nguyễn Tuấn Thịnh và Nguyễn Đỗ Thành Đạt, phiên họp này nhấn mạnh khả năng hiển thị bảo mật đa tầng, bao gồm các sự kiện quản lý, sự kiện dữ liệu và sự kiện hoạt động mạng.
- **CloudTrail & GuardDuty**: Thảo luận về ghi nhật ký cấp tổ chức với CloudTrail và sử dụng GuardDuty để phát hiện mối đe dọa. Các phương pháp phát hiện dưới dạng mã đã được trình bày, bao gồm các truy vấn CloudTrail Lake và triển khai tự động.
- **Kế hoạch bảo vệ nâng cao**: Đề cập đến các tính năng bảo vệ mối đe dọa mở rộng của GuardDuty, bao gồm bảo vệ S3, bảo vệ EKS và phát hiện phần mềm độc hại.
- **Security Hub**: Làm nổi bật cảnh báo tập trung và chuẩn hóa bằng cách sử dụng AWS Security Hub, giúp đơn giản hóa phân tích và lọc dữ liệu.
- **Cảnh báo & Tự động hóa**: Làm nổi bật việc sử dụng EventBridge để cảnh báo và tự động hóa, cùng với ghi nhật ký ở tất cả các lớp (ví dụ: VPC Flow Logs, nhật ký ALB/S3).

#### Trụ cột 3 — Bảo vệ cơ sở hạ tầng
- **Bảo mật mạng và khối lượng công việc**: Đề cập đến phân đoạn VPC, vị trí riêng tư so với công khai và áp dụng Nhóm bảo mật so với NACL. Các chủ đề bổ sung bao gồm WAF, Shield và Tường lửa Mạng để tăng cường bảo vệ.
- **Các vectơ tấn công mạng phổ biến**: Thảo luận về các kịch bản tấn công đi ra ngoài, đông-tây và đi vào, cùng với các trường hợp sử dụng bảo vệ.
- **Bảo mật phân lớp**: Giới thiệu các phương pháp tiếp cận bảo mật phân lớp của AWS, bao gồm trình phân giải DNS VPC Route53 và các tính năng Tường lửa DNS.
- **Bảo vệ khối lượng công việc**: Thảo luận về các nguyên tắc cơ bản để bảo mật khối lượng công việc EC2, ECS và EKS.

#### Trụ cột 4 — Bảo vệ dữ liệu
- **Mã hóa & Quản lý khóa**: Khám phá các chính sách khóa KMS, cấp quyền và luân chuyển. Các phương pháp mã hóa cho dữ liệu khi lưu trữ và khi truyền đã được trình bày cho S3, EBS, RDS và DynamoDB.
- **Quản lý bí mật**: Thảo luận về các mẫu luân chuyển bí mật bằng cách sử dụng Secrets Manager và Parameter Store. Phân loại dữ liệu và các rào cản bảo vệ quyền truy cập cũng được làm nổi bật.

#### Trụ cột 5 — Phản hồi sự cố
- **IR Playbook & Tự động hóa**: Trình bày vòng đời IR theo AWS. Các playbook cho các kịch bản phổ biến, chẳng hạn như khóa IAM bị xâm phạm, phơi bày công khai S3 và phát hiện phần mềm độc hại EC2, đã được chia sẻ. Các kỹ thuật tự động hóa sử dụng Lambda và Step Functions đã được trình bày để tự động phản hồi.
- **Chiến lược phòng ngừa**: Nhấn mạnh tầm quan trọng của việc loại bỏ thông tin xác thực dài hạn, tránh phơi bày trực tiếp các nhóm S3 và thực thi cơ sở hạ tầng dưới dạng mã (IaC) để ngăn chặn cấu hình sai.
- **Quy trình phản hồi sự cố**: Chi tiết quy trình năm bước:
  1. **Chuẩn bị**: Phát triển playbook, đào tạo nhóm và triển khai công cụ phù hợp.
  2. **Phát hiện và phân tích**: Sử dụng các phát hiện của GuardDuty, các bất thường của CloudTrail và cảnh báo của Security Hub.
  3. **Kiềm chế**: Cô lập tài nguyên, thu hồi thông tin xác thực và bảo toàn bằng chứng.
  4. **Loại bỏ và khôi phục**: Loại bỏ các mối đe dọa, vá các lỗ hổng và khôi phục từ các bản sao lưu sạch.
  5. **Đánh giá sau sự cố**: Rút ra bài học, cập nhật playbook và cải thiện cơ chế phát hiện.

### Trải nghiệm sự kiện

Sự kiện rất hấp dẫn, với một chương trình được cấu trúc tốt cho phép người tham gia có được kiến thức sâu sắc về các thực hành bảo mật của AWS. Các diễn giả đã truyền đạt hiệu quả các khái niệm phức tạp, giúp chúng trở nên dễ tiếp cận với những người tham dự có trình độ chuyên môn khác nhau. Các buổi trình diễn trực tiếp và các nghiên cứu điển hình thực tế đã cung cấp những hiểu biết thực tiễn, nâng cao trải nghiệm học tập tổng thể.

### Bài học rút ra

1. **Các biện pháp bảo mật chủ động**: Tầm quan trọng của việc áp dụng cách tiếp cận chủ động đối với bảo mật đám mây, bao gồm việc sử dụng tự động hóa và giám sát liên tục, là một bài học chính.
2. **Mô hình trách nhiệm chia sẻ**: Hiểu mô hình trách nhiệm chia sẻ là rất quan trọng để đảm bảo an ninh trong môi trường đám mây.
3. **Chuẩn bị cho sự cố**: Phát triển và duy trì các playbook phản hồi sự cố và tự động hóa các phản hồi có thể giảm đáng kể tác động của các sự cố bảo mật.
4. **Cải tiến liên tục**: Thường xuyên cập nhật các thực hành và công cụ bảo mật là điều cần thiết để giải quyết các mối đe dọa đang phát triển.

### Điểm chính cần lưu ý

- **Quản lý danh tính và truy cập**: Tránh thông tin xác thực dài hạn và tận dụng AWS Identity Center để tăng cường bảo mật.
- **Phát hiện và giám sát**: Triển khai khả năng hiển thị bảo mật đa tầng bằng cách sử dụng các công cụ như CloudTrail, GuardDuty và Security Hub.
- **Bảo vệ cơ sở hạ tầng**: Sử dụng các công cụ bảo vệ nâng cao như WAF, Shield và Tường lửa Mạng để bảo vệ khối lượng công việc.
- **Bảo vệ dữ liệu**: Mã hóa dữ liệu khi lưu trữ và khi truyền, và quản lý bí mật một cách an toàn với AWS KMS và Secrets Manager.
- **Phản hồi sự cố**: Tự động hóa các quy trình phản hồi sự cố và đảm bảo các nhóm được chuẩn bị tốt với các playbook và đào tạo được cập nhật.

### Một số hình ảnh sự kiện

![pic1](/images/event5_1.jpg)
![pic2](/images/event5_2.jpg)
![pic3](/images/event5_3.jpg)

> Tổng quan, sự kiện đã cung cấp cái nhìn toàn diện về Trụ cột Bảo mật AWS Well-Architected, nhấn mạnh các phương pháp hay nhất và kỹ thuật tự động hóa để nâng cao tư thế bảo mật. Người tham gia đã có được những hiểu biết có giá trị về việc bảo mật môi trường đám mây một cách hiệu quả. Các phiên họp đã làm nổi bật tầm quan trọng của các biện pháp chủ động, giám sát liên tục và tận dụng các công cụ AWS để xây dựng cơ sở hạ tầng an toàn và linh hoạt.