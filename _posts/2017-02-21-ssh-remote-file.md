---
layout: post
title:  "[SSH] Mount remote directory using SSH"
date:   2016-02-21 09:09:09
categories: SSH Linux
---

# Sử dụng SSh để mount thư mục từ máy remote
Đôi khi chúng ta cần chỉnh sửa những file cấu hình, source code từ máy remote, server. Nếu chỉnh sửa nhỏ thì không sao, nhưng nếu như máy remote không có graphic và phải chỉnh sửa nhiều thì thật là ác mộng khi chỉ dùng công cụ vi/vim. Các đơn giản nhất là copy file đó về máy -> chỉnh sửa -> copy lại lên server. Tuy nhiên đôi khi chỉnh sửa chưa đúng, chưa đủ thì ta lại phải làm lại các bước trên. Thật may, chúng ta có thể mount trực tiếp file đó về máy local và chỉnh sửa. Một thứ sẽ thật nhẹ nhàng và nhanh chóng.

## Các bước thực hiện 

* Cài đặt sshfs
```
sudo apt-get install sshfs
```

* Đặt quyền 
```
sudo adduser $USER fuse

sudo chown root:fuse /dev/fuse

sudo chmod +x /dev/fusermount
```

* Tạo thư mục chứa thông tin mount về 
```
mkdir remoteDir
```

* Mount thư mục từ file remote v
```
sshfs remoteHostName@192.168.xx.xx:/pathToRemoteDir ~/remoteDir
```

**Ok, bây giờ chúng ta có thể chỉnh sửa mọi thứ trong thư mục remoteDir như chỉnh sửa trực tiếp trên server.**
