---
layout: post
title:  "[LIBGDX][Chapter 2] Hello Libgdx's World"
date:   2017-02-22 17:00:07
categories: LIBGDX
---

# Viết chương trình Hello world

Chúng ta sẽ bắt đầu loạt bài Libgdx với bài mở đầu về chương trình Hello world kinh điển. Chương trình mà khi chúng ra bắt đầu làm quen với bất kỳ ngôn ngữ hay framework nào cũng đều trải qua. Trong phạm vị bài viết này tôi sẽ cung cấp cho các bạn 

* Cách khởi tạo một project libgdx

* Build và chạy chương trình libgdx trên các nền tảng khác nhau 

* Mô tả về cấu trúc thư mục, file, resource,...

* Một số bug có thể gặp trong quá trình thực hiện

Nào chúng ra cùng bắt đầu.

## Khởi tạo project 

Đầu tiên chúng ta cần download tool tạo project tạo đây:

[Gdx-setup.jar](https://libgdx.badlogicgames.com/nightlies/dist/gdx-setup.jar)

Đây là công cụ tạo project chính thức cho libgdx, nó bao gồm một số tùy chọn nhanh khi khởi tạo như thêm các thư viện, đặt đường dẫn android SDK, ...

Khi khởi chạy có giao diện như hình dưới đây:

<img src="https://luyentm.github.io/blog/assets/libgdx/chapter2/helloworld1.png">

- Name: Tên project bạn muốn tạo
- Package: package nam
- Game class: Tên main class, sẽ được đặt trong project core
- Destination: đường dẫn lưu trữ pr
- Android SDK: đường dẫn mà bạn đặt android sdk. Lưu ý, nếu không tìm tồn tại thì bạn sẽ không tạo ra được project Android
- Sub project: đâu là tên các project sẽ được tạo ra. Nên chọn Desktop, Android, Ios và HTML
- Extension: một project bình thường ta nên chọn Freetype (dành cho font chữ). Các thành phần còn lại chúng ra sẽ tìm hiểu trong 1 bài viết cụ thể khác.
