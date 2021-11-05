> Anh bưu tá này là một người mà Gà rất tin tưởng. Gà ủy quyền cho anh ấy lên bưu điện, nói chuyện với anh kiểm thư để lấy thư về.

> Nếu giấy ủy quyền hợp lệ, anh kiểm thư sẽ giữ lại bản gốc rồi photocopy ra một bản khác để anh bưu tá đem về cho Gà. Để nhỡ trong trường hợp Gà có tức quá xé thư đi thì vẫn có thể lên đây lấy lại.

> Đố bạn anh bưu tá sử dụng giao thức email nào để nói chuyện với anh kiểm thư?
>  network.letspentest.org 9002


* Sử dụng `nmap` để scan cổng `9002`: `nmap  network.letspentest.org -p 9002`



![image](https://user-images.githubusercontent.com/68783065/140474061-ef6e42b0-f808-4ea1-947d-1d2f7b0226f9.png)



* `Port 9002` sử dụng giao thức `TCP`


* Dùng `telnet` connect: `telnet network.letspentest.org 9002` 


![image](https://user-images.githubusercontent.com/68783065/140474311-146c9a64-0676-4816-9446-394c6ff64a9c.png)


* Sau một hồi dùng tool `brute force` bằng "cơm". Login được với `USER` là `cookiehanhoan`; `PASS` là `password`:


![image](https://user-images.githubusercontent.com/68783065/140474860-57b20961-bc9c-43b6-96a8-1fc235f5c88b.png)

* Dùng `LIST` để hiện thị những `message`:


![image](https://user-images.githubusercontent.com/68783065/140475018-caa02ef8-f79a-4cbb-88e2-d89ffa298d68.png)

* Dùng `RETR` mở từng `message` một. Đến message 8 thì thấy flag:


![image](https://user-images.githubusercontent.com/68783065/140475340-ccf6edad-f191-419f-8027-151e9df92874.png)


* Flag is: `Flag{1-Ha\/3-1o0o-UnS33n-3Ma1L}`

