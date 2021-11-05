> Hazy ngồi cân những viên bi mình đang có, loay hoay vẫn không biết phải cân bao nhiêu lần để tìm được viên bi nhẹ nhất.

> Bạn giúp Hazy một tay với nhé.



> programming.letspentest.org 8333 


* `import` thêm modul `re`:

```python
import re
```

* Thêm hàm `count` và viết lại hàm `slover`:

```python
def count(n):
  i=0
  while n>1:
    n//=3
    i+=1
  return i
# Ham nay giai bai toan
# |||||||||||||||||||||||||||||||||||||||||||||||||
# |||Người chơi điền code giải và return kết quả|||
# |||||||||||||||||||||||||||||||||||||||||||||||||
# vvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvv
def solver(received):
    # solver lets goo
    # Kiểu dữ liệu trả về là INT
    # nên dùng try-except để tránh xảy ra những tai nạn
    stringnumber = re.findall(r"\d+",received)
    intnum = int(stringnumber[0])
    return count(intnum)
```


![image](https://user-images.githubusercontent.com/68783065/140482070-6105162f-d973-450c-83d4-63cac50d1d33.png)



* Flag is: `Flag{n0_pr0b_w1th_cub3_r00t_RIGHT?}`
