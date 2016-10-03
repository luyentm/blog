---
layout: post
title:  "Sử dụng git tạo patch file"
date:   2016-09-10 18:00:00
categories: git patch 
---
# Sử dụng git tạo patch file

Trong quá trình làm việc chung trên một source code chúng ta phải thường xuyên trao đổi với nhau về những thay đổi của source code. Đối với git chúng ta hay sử dụng việc đóng gói những thay đổi vào các commit và share cho các thành viên khác trong team. Tuy nhiên đôi khi chúng ta vì lý do nào đó mà không thể push lên repo chung. Khi đó việc dùng patch file là cực kì quan trọng và thuận lợi, chúng ta có thể trao đổi thông qua việc gửi email, share file. Thậm chí có thể quan sát các thay đổi trong từng file.

Trong bài này chúng ta cùng học cách tạo patch file nhanh chóng với git, đồng thời tìm hiểu cách áp dụng patch file vô source code.

## Tạo patch file

b1. Commit những thay đổi của bạn muốn đưa vào patch file. Bạn có thể chia ra làm nhiều commit, khi đó mỗi commit sẽ là một patch file.

b2. Command

```
git format-patch HEAD~n
```

* trong đó n là số commit kể từ commit hiện tại mà bạn muốn tạo patch. Ví dụ: n=7, git sẽ tạo ra 7 file patch, mỗi file tương ứng với một commit kể từ commit hiện tại (HEAD). Đồng thời các file cũng được đánh số 0001-commit-message*.patch

## Apply patch

b1. Kiểm tra xem patch sẽ thực hiện những thay đổi gì

```
git apply --stat file.patch
```

b2. Kiểm tra xem file có apply được vô source code hay không

```
git apply --check file.patch
```

b3. Thực hiện apply

```
git am --signoff < file.patch
```

* Chú ý bạn có thể bỏ tham số --signoff, nếu muốn apply nhiều file dùng *.patch thay cho tên file.


