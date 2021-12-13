# Group22_Lightsail
Project Final Cloud Class 06 (AWS)

+ Trần Lưu Thế Anh - 19110324

+ Nguyễn Thái Hải - 19110356

+ Nguyễn Hữu Hiếu - 19110364

Giảng viên hướng dẫn: TS. Huỳnh Xuân Phụng

Mã môn học: CLCO332779

# Cấu hình WordPress với Amazon Lightsail

- Amazon Web Services là nền tảng dịch vụ điện toán đám mây an toàn, mang đến khả năng tính toán, lưu trữ cơ sở dữ liệu, phân phối nội dung và các chức năng khác nhằm giúp các doanh nghiệp mở rộng và phát triển.

- Vậy Amazon Lightsail là gì? Amazon Lightsail là một dịch vụ đám mây của Amazon, không chỉ là môi trường điện toán (Computing environment), nó còn có thể lưu trữ dữ liệu (Storage - Amazon S3 ), khả năng khôi phục dữ liệu (Snapshots - Amazon RDS). Ngoài ra, nó cung cấp các dịch vụ khác như cân bằng tải (Elastic Load Balancing), tưởng lửa (Firewall), DNS (Route 53) kèm theo một số chức năng có sẵn khác.

- Đầu tiên giới thiệu về cách cài đặt và cấu hình WordPress trên Amazon Lightsail

![myimage-alt-tag](https://github.com/theanh176/Group22_Lightsail/blob/main/image/logo.jpg)

# Các bước thực hiện

## 1. Cài đặt WordPress với Lightsail

- Truy cập vào tab Lightsail chọn **Create instance**.

![myimage-alt-tag](https://github.com/theanh176/Group22_Lightsail/blob/main/image/1Create_instance.PNG)

- Chọn vị trí AWS

![myimage-alt-tag](https://github.com/theanh176/Group22_Lightsail/blob/main/image/2Singapore.PNG)

- Chọn hệ điều hành sẽ sử dụng.

- Linux/Unix.

- WordPress.

![myimage-alt-tag](https://github.com/theanh176/Group22_Lightsail/blob/main/image/3hdh.PNG)

- Chọn gói dịch vụ Amazon Lightsail chọn gói dịch vụ phù hợp với trang web của bạn ở đây thì mình sẽ chọn gói ít tiền nhất 3.5$

![myimage-alt-tag](https://github.com/theanh176/Group22_Lightsail/blob/main/image/4price_per_month.PNG)

- Cuối cùng thì nhập tên ứng dụng và khởi tạo.

- Với Amazon Lightsail cài đặt rất dễ dàng, chỉ cần vài cú click chuột, thì chúng ta đã có một server hoàn chỉnh.

## 2. Kết nối với máy tính thông qua SSH và lấy mật khẩu WordPress website

### Lấy mật khẩu để đăng nhập vào màn hình quản trị của WordPress

- Trên tab Lightsail click vào icon SSH

![myimage-alt-tag](https://github.com/theanh176/Group22_Lightsail/blob/main/image/5ssh.PNG)

- Sau đó dùng lệnh

`cat $HOME/bitnami_application_password` để lấy mật khẩu mặc định

![myimage-alt-tag](https://github.com/theanh176/Group22_Lightsail/blob/main/image/6password.PNG)

## 3. Đăng nhập vào trang quản trị WordPress

- Sau khi đăng nhập chúng ta có thể thay đổi mật khẩu cài đặt plugin và tùy biến giao diện cũng như các chức năng trên website của mình

- truy cập http://52.76.18.66/wp-login.php

![myimage-alt-tag](https://github.com/theanh176/Group22_Lightsail/blob/main/image/7ip.PNG)

- Đăng nhập và cấu hình, plugin

![myimage-alt-tag](https://github.com/theanh176/Group22_Lightsail/blob/main/image/8wordpress.PNG)

## 4. Tạo địa chỉ IP

- Truy cấp vào ứng dụng bạn vừa tạo và chọn tab Networking, sau đó tạo địa chỉ IP.

![myimage-alt-tag](https://github.com/theanh176/Group22_Lightsail/blob/main/image/9createIp.PNG)

- Sau khi đặt tên cho StaticIP nhấn Create.

![myimage-alt-tag](https://github.com/theanh176/Group22_Lightsail/blob/main/image/91Staticip.PNG)

## 5. Trỏ tên miền cho ứng dụng

- Vẫn ở tab Networking thì ta chọn Create DNS zone.

- Sau đó nhập tên miền và click Create DNS zone.

![myimage-alt-tag](https://github.com/theanh176/Group22_Lightsail/blob/main/image/9createIp.PNG)

- Nhập tên miền vào DNS records.

![myimage-alt-tag](https://github.com/theanh176/Group22_Lightsail/blob/main/image/92domain.PNG)

- Trỏ các Name servers qua bên quản lý domain.

![myimage-alt-tag](https://github.com/theanh176/Group22_Lightsail/blob/main/image/93domain_add_recore.PNG)

# Kết luận

- Với Amazon Lightsail thì chúng ta có thể cài đặt một website khá chi đơn giản và dễ sử dụng như các bước ở trên (Chỉ cần click và nhập thông tin đơn giản). Tuy nhiên nhược điểm khi dùng Amazon Lightsail thì khá cứng nhắc chúng ta sẽ bị hạn chế đội với một cài đặt nhất định khó có thể tùy biến theo ý muốn. Khó bảo trì nâng cấp.

- Với những ưu nhược điểm ở trên thì Amazon Lightsail khá chi phù hợp với các website đơn giản.

# Tài liệu tham khảo

https://aws.amazon.com

