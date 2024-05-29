#switcher

![image](https://github.com/NamDT5125/ctfs/assets/69895129/afcf9b0a-d180-4797-b7b3-b1c9da9dd467)

Check thì thấy là ELF64 và không có gì đặc biệt, chạy thử trên linux xem ra cái gì:

![image](https://github.com/NamDT5125/ctfs/assets/69895129/a2f87770-c2f6-40ca-bd05-5a32adf770df)

Chương trình check password, đưa vào IDA để dịch ngược:

![image](https://github.com/NamDT5125/ctfs/assets/69895129/592f5627-6a28-4832-b72b-0087f24f27b3)

s là input và hàm `sub_5540` để check flag, vào đó xem thì ta thấy có if else liên tục:

![image](https://github.com/NamDT5125/ctfs/assets/69895129/d4e099ad-3376-4b84-94b6-c76c88338ef2)

Chép mấy số này lại và chuyển từ decimal ra text ta có flag: `jumping_my_way_to_the_flag_one_by_one`
