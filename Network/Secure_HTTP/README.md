> HTTP và HTTPS đều là hai giao thức giúp trình duyệt của bạn truy cập, tương tác với các trang Web. Tuy nhiên khi sử dụng giao thức HTTP để truy cập Web ở một quán cà phê hay trong cùng một khu trọ thì tất cả các nội dung trao đổi nhạy cảm, cũng như mật khẩu của bạn trên Web đều có thể nghe lén.

> Còn HTTPS (chữ S có nghĩa là Secure - Bảo mật) sinh ra để mã hóa dữ liệu trong quá trình trao đổi giữa trình duyệt và máy chủ bằng một chiếc Chứng chỉ (Certificate)
> network-insecure.letspentest.org 9004


* Truy cập http://network-insecure.letspentest.org:9004. Không hỗ trợ giao thức `HTTP`.

![image](https://user-images.githubusercontent.com/68783065/140476602-18ef1060-7458-4422-8afd-3245c1098895.png)

* Đổi lại thành https://network-insecure.letspentest.org:9004

![image](https://user-images.githubusercontent.com/68783065/140476845-76b54568-7f09-444b-a115-0869c2fcd391.png)

* Chọn `Advanced`, đi đến `view certificate`:

![image](https://user-images.githubusercontent.com/68783065/140477246-fe7b7478-ddbd-46e6-b682-254932d631e3.png)


![image](https://user-images.githubusercontent.com/68783065/140477109-e4e51db1-8a90-4d72-a28a-648d8aea4ee5.png)



* Flag is: `Flag{This-Is-A-Trusted-One}`


