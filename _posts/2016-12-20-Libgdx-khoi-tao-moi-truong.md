---
layout: post
title:  "[LIBGDX] Thiết lập môi trường làm việc Libgdx"
date:   2016-12-20 17:00:07
categories: LIBGDX
---
# Chapter 1: Thiết lập môi trường làm việc Libgdx
Thật may mắn vì libgdx là open source và đa nền tảng. Do đó, chúng ta có thể code một cách thoải mái với bất kỳ IDE hay hệ điều hành nào chúng ta cảm thấy thân thiết nhất.

Tuy nhiên 1 tutorial thì không thể hướng dẫn một lúc trên nhiều IDE hay nhiều hệ điều hành được. Vì vậy, tôi sẽ đưa ra những cài đặt, tùy chỉnh mà bản thân tôi thấy là phù hợp, dễ tiếp cận cũng như phổ biến nhất hiện nay. Nếu bạn cảm thấy không quen thuộc với những cài đặt mà tôi đứng ra, đừng lo, hãy thử theo cách của bạn, mọi thứ đều khá dễ dàng và tương tự nhau.

## IDE
Mình chọn **eclipse** cho tutorial này. Tuy vậy, bạn có thể chọn bất cứ IDE nào có hỗ trợ **Gradle** mà bạn cảm thấy ưa thích. Gradle là một công cụ hỗ trợ phát triển code mới. Bạn sẽ không phí phạm nếu dành ra 1 chút thời gian để đọc qua về nó. Hiện tại, bạn có thể chọn intellij, netbean, eclipse hoặc android studio ...

## Java
Cài đặt JDK, tốt nhất nên cài từ bản 7 trở lên. Ở đây thì mình cứ bản mới nhất (JDK 8) là chiến thôi
[link](http://www.oracle.com/technetwork/java/javase/downloads/index.html)

```
http://www.oracle.com/technetwork/java/javase/downloads/index.html
```

## Eclipse
Bạn có thể cài bất kì bản nào của eclipse. Ở đây mình dùng Neon mới nhất 
[link](http://www.eclipse.org/neon/)

```
http://www.eclipse.org/neon/
```

## Android SDK

* Linux
[link](https://dl.google.com/android/repository/tools_r25.2.3-linux.zip)

```
https://dl.google.com/android/repository/tools_r25.2.3-linux.zip
```

* Windows
[link](https://dl.google.com/android/repository/tools_r25.2.3-windows.zip)

```
https://dl.google.com/android/repository/tools_r25.2.3-windows.zip
```
* Mac
[link](https://dl.google.com/android/repository/tools_r25.2.3-macosx.zip)

```
https://dl.google.com/android/repository/tools_r25.2.3-macosx.zip
```

## ADT plugin - dùng cho project android trong eclipse

* Bật eclipse

* Help/Install New Software

* Chọn đường link: **https://dl-ssl.google.com/android/eclipse/**

* Cài đặt tất cả những gói được list ra

## Gradle
Đối với eclipse neon thì gradle mặc định đã cài sẵn, nếu bạn đang dùng 1 version khác thì bạn làm theo hướng dẫn sau:

* Bật eclipse

* Help/Install New Software

* Chọn đường link: **http://dist.springsource.com/release/TOOLS/gradle**

* Cài đặt tất cả những gói được list ra 

