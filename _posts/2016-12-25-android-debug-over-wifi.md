---
layout: post
title:  "[Android] Debug ứng dụng android qua Wifi"
date:   2016-12-25 09:09:09
categories: Android
---
# Debug ứng dụng android qua Wifi

Nhiều khi việc debug ứng dụng android mà phải cắm thông qua dây cáp USB có đôi chút bât tiện không hề nhẹ. Do đó việc không dùng cáp mà vẫn debug được trông thật là pro và giảm bớt đi nhiều phiền phức không đáng có.

## Cách thực hiện

* Kết nối điện thoại và máy tính vào chung 1 mạng wifi, từ điện thoại lấy ra địa chỉ IP, ví dụ của mình là **10.0.0.9**
* Disconnect tất cả các devices nếu đã kết nối trước đó:

```
adb disconect
```

* Tạo port lắng nghe cổng 5555

```
adb tcpip 5555
```

* Connect đến thiết bị thông qua IP

```
adb connect 10.0.0.9
```

Nếu kết nối thành công sẽ báo

```
Connected to 10.0.0.9:5555
```

* Cuối cùng trong eclipse hoặc android studio, bạn phải chọn lại devices để test.

Demo:

<img src="https://luyentm.github.io/assets/connectdemo/connectdemo.png">

## Tạo file script/bat

Dĩ nhiên để cho việc connect được nhanh chóng chúng ta nên tạo ra 1 file script. Trên windows các bạn nhớ thay đường dẫn của bạn cho chính xác. Trên linux nhớ cài adb hoặc trỏ đúng đường dẫn.

* Windows

Tạo 1 file: connect.bat

```
C:\Users\luyentm\android-sdks\platform-tools\adb.exe tcpip 5555
C:\Users\luyentm\android-sdks\platform-tools\adb.exe connect 10.0.0.9
```

* Linux

Tạo 1 file: connect.sh

```
adb tcpip 5555
adb connect 10.0.0.9
```


**Chúc các bạn thành công và giáng sinh vui vẻ ^^**
