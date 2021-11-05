> Nếu coi mỗi máy chủ là một ngôi nhà, trước khi xâm nhập vào bên trong, các Hacker phải thực hiện việc thăm dò. Họ xem xét đâu là điểm yếu nhất của ngôi nhà, chỗ nào là điểm mù camera? Chủ nhà hoặc bảo vệ sẽ phản ứng thế nào khi có xuất hiện các dấu hiệu bất thường?

> Trong quá trình tìm kiếm lỗ hổng, Hazy thường xem xét ngôi nhà này có bao nhiêu cánh cửa đang mở (Port). Hãy sử dụng công cụ thân quen để "ném đá" vào tất cả các cánh cửa của ngôi nhà.

> Biết rằng, cửa sổ được đánh số từ 8100 tới 9100

> Dựa vào sự phản hồi bạn sẽ biết được những điều thú vị!
> network-insecure.letspentest.org


* Use `nmap` scan từ port `8100`-`9100`: `nmap  network-insecure.letspentest.org -p 8100-9100`


![image](https://user-images.githubusercontent.com/68783065/140476136-e1c45841-378d-48d8-ac01-3b4d6f538a24.png)


* `telnet` vào port `9003`:

![image](https://user-images.githubusercontent.com/68783065/140476357-31d4a962-bb81-4080-a1a5-5b1c10b0c073.png)


* Flag is: `Flag{Every-Header-Have-It-Own-Meaning}`





