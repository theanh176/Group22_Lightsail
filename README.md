# Group22_Lightsail
Project Final Cloud Class 06 (AWS)

+ Trần Lưu Thế Anh - 19110324

+ Nguyễn Thái Hải - 19110356

+ Nguyễn Hữu Hiếu - 19110364

Giảng viên hướng dẫn: TS. Huỳnh Xuân Phụng

Mã môn học: CLCO332779

# I. Cấu hình WordPress với Amazon Lightsail

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

# II. Mean
Ngăn xếp dành cho nhà phát triển Mean: Mean Stack là sự kết hợp giữa của MongoDB, ExpressJS, AngularJS, NodeJS và khiến cho việc xây dựng những ứng dụng web trở nên mạnh mẽ và đơn giản hơn bao giờ hết.

<img src="https://github.com/ThaiHaiDev/Mean/blob/main/Images/bandicam%202021-12-03%2017-01-26-743.jpg?raw=true">

# Các bước thực hiện
  ## 1. Tiến hành Create Instance trong Lightsail AWS
  • Chọn Stack Mean và đặt tên instance lại nếu cần. Sau đó chọn Create Instance. Đợi 1 vài phút để AWS có thể tạo và running.
  <img src="https://github.com/ThaiHaiDev/Mean/blob/main/Images/bandicam%202021-12-13%2010-25-33-075.jpg?raw=true" >
  
  ## 2. Lấy Password Mean
  • Mở connect bitnami trong Stack Mean vừa tạo, gõ lệnh ls để xem các thành phần, sẽ có mục bitnami_application_password để chúng ta lấy password. Để lấy password của Mean, gõ lệnh `cat bitnami_application_password` 
  
  <img src="https://github.com/ThaiHaiDev/Mean/blob/main/Images/bandicam%202021-12-13%2010-29-38-872.jpg?raw=true">
  
  ## 3. Clone các project github
  • Clone 2 project từ github về gồm Front-End và Back-End để thực hiện cài đặt app React. Sau khi clone xong, sử dụng lệnh `ls` để xem đã có mục phần đó hay chưa.
  
  <img src="https://github.com/ThaiHaiDev/Mean/blob/main/Images/bandicam%202021-12-13%2010-42-52-360.jpg?raw=true">
  
  ## 4. Tạo Database Mongodb
  • Thực hiện tạo Database với Mongodb với các lệnh:
  
  `mongo admin --username root --password + Password Mean ở trên vừa lấy`
  
  Sau khi kết nối với Mongodb sẽ có dạng như sau:
  
  <img src="https://github.com/ThaiHaiDev/Mean/blob/main/Images/bandicam%202021-12-13%2010-50-16-927.jpg?raw=true">
  
  • Tiến hành tạo Database 
  
  `db = db.getSiblingDB('GROUP22')`
  
  • Thêm User vào Database
  
  `db.createUser( { user : "mean", pwd : "admin", roles : [ "readWrite", "dbAdmin" ]} )`
  
  <img src="https://github.com/ThaiHaiDev/Mean/blob/main/Images/bandicam%202021-12-13%2011-00-59-303.jpg?raw=true">
  
  Sau khi thêm thành công sẽ có hiện Successfull.
  
  ## 5. Chỉnh sửa cấu hình Folder customerManagement_MERN
  
  • Truy cập Folder customerManagement_MERN và mở file index.js để chỉnh sửa bằng lệnh:
  
  `cd customerManagement_MERN`
  
  `vim index.js`
  
  <img src="https://github.com/ThaiHaiDev/Mean/blob/main/Images/bandicam%202021-12-13%2011-06-00-597.jpg?raw=true">
  
  • Thực hiện chỉnh sửa file index.js theo như trong hình bằng cách nhấn phím `s` rồi thực hiện.
  
  <img src="https://github.com/ThaiHaiDev/Mean/blob/main/Images/bandicam%202021-12-13%2020-29-38-346.jpg?raw=true">
  
  Sau đó lưu lại bằng cách nhấn tổ hợp phím `Ctrl + C` và gõ lệnh `wq!` để lưu.
  
  • Lấy địa chỉ localhost bằng cách cd .. ra mục ban đầu và gõ lệnh `sudo ifconfig` để lấy địa chỉ localhost.
  
  <img src="https://github.com/ThaiHaiDev/Mean/blob/main/Images/bandicam%202021-12-13%2020-43-57-476.jpg?raw=true">
  
  • Mở .env để chỉnh sửa đường dẫn Path Database đã được tạo ở trên bằng các lệnh:
  
  `touch .env`
  
  `vim .env`
  
  <img src="https://github.com/ThaiHaiDev/Mean/blob/main/Images/bandicam%202021-12-13%2011-57-39-851.jpg?raw=true">
  
  Sau đó cũng nhấn phím `s để bắt đầu chỉnh sửa và gõ 2 lệnh ở dưới vào:
  
  `DATABASE_PATH=mongodb://mean:admin@172.26.8.161/GROUP22`
  
  `SECRET_KEY=thisissecret`
  
  Với mean là tên User, admin là Password, GROUP22 là tên Database, 172.26.8.161 là địa chỉ localhost.
  
  <img src="https://github.com/ThaiHaiDev/Mean/blob/main/Images/bandicam%202021-12-13%2020-43-06-800.jpg?raw=true">
  
  • Truy cập Folder cm_frontend và kiểm tra yêu cầu:
  
  Trong cm_frontend có src, chúng ta sẽ xem code bằng lệnh `cat src/index.js` và `cat src/backend` sẽ thấy yêu cầu đường dẫn REACT_APP_BACKEND. Sẽ thêm vào ở .env như ở trên.
  
  <img src="https://github.com/ThaiHaiDev/Mean/blob/main/Images/bandicam%202021-12-13%2012-00-36-211.jpg?raw=true">
  
  Thêm dòng code vào .env ở cm_frontend
  
  <img src="https://github.com/ThaiHaiDev/Mean/blob/main/Images/bandicam%202021-12-13%2021-06-04-795.jpg?raw=true">
  
  • Với địa chỉ ip được lấy ở Network ở AWS Lightsail của Stack Mean. Và đồng thời add rule ở Netword 2 Port 3000 và 8000
  
  <img src="https://github.com/ThaiHaiDev/Mean/blob/main/Images/bandicam%202021-12-13%2021-09-15-801.jpg?raw=true">
  
  <img src="https://github.com/ThaiHaiDev/Mean/blob/main/Images/bandicam%202021-12-13%2021-07-13-707.jpg?raw=true">
  
  • Quay về vị trí ban đầu, cài đặt forever: `npm install -g forever` 
  
  Chạy `forever start index.js`
  
  • Truy cập lại customerManagement_MERN và cài npm `npm install`
  
  Sau khi cài xong npm, chạy `npm start` kiểm tra xem đã kết nối Database hay chưa. Nếu kết nối thành công sẽ hiện DB is Connected.
  
  <img src="https://github.com/ThaiHaiDev/Mean/blob/main/Images/bandicam%202021-12-13%2021-48-01-367.jpg?raw=true">
  
  • Truy cập cm_frontend và cài npm `npm install`. Sau đó chạy lệnh `forever start "npm start" ./` và chạy `npm install`. App React đã được Starting với Server.
  
  • Chạy trên trình duyện địa chỉ: `54.251.142.63:3000` . Bây giờ đã start App thành công với giao diện:
  
  <img src="https://github.com/ThaiHaiDev/Mean/blob/main/Images/bandicam%202021-12-13%2021-23-18-528.jpg?raw=true">
  
  <img src="https://github.com/ThaiHaiDev/Mean/blob/main/Images/bandicam%202021-12-13%2021-23-34-427.jpg?raw=true">
  

# Tài liệu tham khảo

https://aws.amazon.com

