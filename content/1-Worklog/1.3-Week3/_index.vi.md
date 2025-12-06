---
title: "Worklog Tuần 3"
date: "2025-09-22"
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---


### Mục tiêu tuần 3:

* Học cách hosting website tĩnh sử dụng S3.
* Làm quen với EC2 và các tính năng cơ bản.
* Tìm hiểu cách triển khai và quản lý cơ sở dữ liệu quan hệ trên AWS.
* Cài đặt và sử dụng AWS CLI để tương tác với dịch vụ AWS.
* Giám sát, quản lí hiệu suất hệ thống với CloudWatch

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Học tổng quan về S3 <br> - **Thực hành:**<br>&emsp; + Tạo S3 bucket và tải lên dữ liệu<br>&emsp; + Cấu hình truy cập vào bucket và đối tượng<br>&emsp; + Tăng tốc và bảo mật website tĩnh với Cloudront + Sao chép, di chuyển đối tượng trong S3 bucket<br>&emsp;                                                                                         | 22/09/2025   | 22/09/2025      | [AWS Study Group](https://cloudjourney.awsstudygroup.com/)
| 3   | - Tìm hiểu các tính năng cơ bản của Amazon EC2 <br> - **Thực hành:**<br>&emsp; + Tạo Windows, linux instance<br>&emsp; + Thay đổi cấu hình EC2<br>&emsp; + Xây dựng AMI tùy chọn<br>&emsp;                                           | 23/09/2025   | 23/09/2025      | [AWS Study Group](https://cloudjourney.awsstudygroup.com/) |
| 4   | - Tìm hiểu kiến thức cơ bản về cơ sở dữ liệu với Amazon RDS<br> - **Thực hành:**<br>&emsp; + Tạo RDS database instance<br>&emsp; + Thử triển khai ứng dụng mẫu<br>&emsp;  | 24/09/2025   | 24/09/2025      | [AWS Study Group](https://cloudjourney.awsstudygroup.com/) |
| 5   | - Tìm hiểu về AWS CLI và sử dụng để tương tác với dịch vụ AWS:<br>&emsp; + S3<br>&emsp; + SNS<br>&emsp; + IAM<br>&emsp; + VPC<br>&emsp; + EC2<br>&emsp;                | 25/09/2025   | 25/09/2025      | [AWS Study Group](https://cloudjourney.awsstudygroup.com/) |
| 6   | - **Thực hành:**<br>&emsp; + Sử dụng Metric của CLoudWatch để quan sát thông qua các biểu đồ và bảng dữ liệu<br>&emsp; + Thu thập, phân tích và lưu trữ logs từ các ứng dụng, hệ thống và dịch vụ AWS thông qua CloudWatch Logs<br>&emsp; + Tự động giám sát metrics và logs qua CloudWatch Alarm <br>&emsp; + Quản lí tập trung các metrics, logs và alarm thông qua Dashboard                                                                                       | 26/09/2025   | 26/09/2025      | [AWS Study Group](https://cloudjourney.awsstudygroup.com/) |


### Kết quả đạt được tuần 3:

* Học được cách hosting và cấu hình website tĩnh sử dụng S3

* Tìm hiểu về Amazon EC2 - dịch vụ máy chủ ảo cốt lõi của AWS, cách thức hoạt động và các thành phần quan trọng của dịch vụ này.
  * AMI
  * Keypair
  * Instance

* Nắm được cơ bản về cơ sở dữ liệu với RDS
  * Tạo RDS database instance
  * Cách triển khai, sao lưu và khôi phục ứng dụng trên RDS

* Biết cách cấu hình, kiểm tra tài nguyên với CLI và tương tác với các dịch vụ cơ bản của AWS

* Nắm được cách CloudWatch hoạt động như một dịch vụ giám sát và quản lý hiệu suất toàn diện trong hệ sinh thái AWS.
  * Biết cách thu thập và phân tích các chỉ số từ ứng dụng đang chạy trên EC2 Instances.
  * Làm quen với việc xử lý và lọc dữ liệu từ CloudWatch Logs.
  * Tạo cảnh báo dựa trên ngưỡng Metrics để phát hiện sớm các vấn đề và nhận thông báo kịp thời.
  * Tạo bảng điều khiển trực quan tích hợp các Metrics và Alarms để có cái nhìn tổng quan về hệ thống.

