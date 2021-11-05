> Ôi không, Hazy lỡ xoá đi một mảnh ghép trong quá trình mã hoá AES mất rồi :)


* `Brute Force` với `Python`:


```python
from Crypto.Cipher import AES
from Crypto.Util.Padding import unpad
f = open('cipher1.txt','rb')
ciphertext = f.read()
key = b'supersecretkey!?'
iv0 = b"0xcafedeadbeef"
for i in range(32,127):
    for j in range(32,127):
        iv = iv0+bytes([i])+bytes([j])
        cipher = AES.new(key, AES.MODE_CBC, iv)
        plaintext = unpad(cipher.decrypt(ciphertext),16).decode()
        if all([char in 'abcdef0123456789' for char in plaintext[5:-1] ]):
            print(iv,plaintext)
```
