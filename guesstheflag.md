#guess_the_flag
![image](https://github.com/NamDT5125/ctfs/assets/69895129/cf9f85ad-9e54-4063-a8a3-2d61c2397fee)
Đây là file ELF64, ta chạy thử xem nó như nào
![image](https://github.com/NamDT5125/ctfs/assets/69895129/c6a84f6e-ba28-47cf-94bd-a73188df8b6b)
Chương trình yêu cầu ta nhập flag kiểm tra, dùng IDA dịch ngược:
![image](https://github.com/NamDT5125/ctfs/assets/69895129/d08bd8cf-8281-489b-9854-23dbbb08529c)
Nếu flag đúng thì in ra correct, flag nhập vào được xor với 1 và so sánh với `secretcode`, ta chỉ cần dùng `secretcode` xor lại với 1 là ra:
![image](https://github.com/NamDT5125/ctfs/assets/69895129/72c1c625-c2d7-4b99-8a07-a855fc3dd07e)
`ctf{committed_to_the_least_significant_bit}`
