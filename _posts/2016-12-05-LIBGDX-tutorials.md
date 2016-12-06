---
layout: post
title:  "[LIBGDX] Lập trình game với LIBGDX"
date:   2016-12-05 09:09:09
categories: LIBGDX
---
# Học lập trình game đa nền tảng với LibGDX platform

## Giới thiệu

Tôi tên là Luyện (Trần Minh). Sở thích của tôi là làm những cái mình thích. Do đó tôi hay voọc vạch linh tinh, cũng vì làm linh tinh nên chẳng có cái gì ra hồn cả. Những thứ tôi đã làm thường dở dang và thường không có đầu có cuối. Chính vì vậy tôi dự định sẽ viết 1 blog, trước là để hệ thống lại kiến thức của mình một cách chỉn chu, ngăn nắp. Sau đó là share kiến thức có ích cho người khác. Tôi cũng phân vân nên viết bằng tiếng Việt hay tiếng Anh. Bời vì tiếng Anh của tôi khá kém nên đây có thể là một cơ hội để nâng trình. Có lẽ sẽ có thêm 1 bài song song bằng tiếng Anh chăng? ^^

## Mục đích

Bên cạnh những kiến thức rời rạc sẽ được post khi mà tôi học được cái mới, tôi dự định viết 1 tutorial dài hơi về làm game. Trong loạt bài này, tôi sẽ viết về lập trình game với LibGDX. Với xu thế hiện nay là game trên mobile thì tôi hy vọng loạt bài này sẽ hữu dụng không chỉ cho bây giờ mà ngay cả trong tương lai 5-7 năm nữa. Giúp các bạn đang tìm hiểu về làm game có được một bộ tutorial rõ ràng, đầy đủ và dễ hiểu. 
Và cuối cùng là mong muốn làm một cái gì có ích cho đời :D.

## Tại sao lại chọn Libgdx ???

Để trả lời cho câu hỏi này, tôi sẽ không đưa ra so sánh giữa Libgdx với các engine khác như Unity, Andengine, v.v. Bởi vì thực ra tôi chưa từng làm qua những engine này nên không thể đưa ra nhận định khách quan được. Thay vào đó tôi sẽ nêu ra những điểm mạnh của Libgdx.

- Ngôn ngữ lập trình: Java. Một ngôn ngữ cực phổ biến, trong sáng và dễ học. Có lẽ bất kể ai học trong ngành IT thì việc học lập trình hướng đối tượng nói chung hay học Java nói riêng gần như là bắt buộc. Ngay cả khi bạn chưa bao giờ lập trình java, nếu bạn nắm được kiến thức hướng đối tượng thì việc học ngôn ngữ này trong vòng 1 tuần là khả thi.

- Đa nền tảng: Android, iOS, Desktop(Windows,Mac,Linux), HTML5. Cho đến hiện nay Libgdx vẫn build ngôn nghẻ cho hiều hệ điều hành. Các ứng dụng khá nhẹ (game tối thiểu libgdx trên android chỉ khoảng 300Kb), chạy mượt mà, hiệu năng cao. Về phần iOS gần đây có một chút trục trặc khi robovm chuyển sang close source. Tuy nhiên Libgdx đã nhanh chóng có những cập nhật nhanh chóng. Libgx đã fork lại robovm để tự support tiếp, đồng thời đưa thêm 1 tùy chọn nữa là mobile intel engine. Hiện tại, bạn vữa build cho iOS dễ dàng. Tính đa nền tảng này giúp cho chúng ta tiếp kiệm thời gian rất nhiều. Đặc biệt là với những bạn muốn phát triển game 1 cách độc lập.

- Open source: Tôi là một người yêu thích open source. Ban đầu chỉ vì những ứng dụng open source đa số là free (Tôi dùng hệ điều hành debian, tất cả các tool đều sủ dụng của linux). Nhưng giờ đây với tôi vẻ đẹp của opensource chính là source code. Cái mà tôi hoàn toàn có thể khám phá vào bên trong. Đọc source code người khác như là một sở thích của tôi vậy :D. Cụ thể là chúng ta có thể hiểu được cách mà người ta làm được ở tầng dưới hơn, thậm chí chúng ta sửa đổi được theo ý mình.

- Ứng dụng hỗ trợ: Cộng đồng libgdx khá phát triển, cùng với đó là các công cụ đi kèm, giúp làm tăng đáng kể hiệu xuất cũng như tốc độ làm việc. Đa số chúng là các công cụ opensource, free và cập nhật liên tục. Do đó chúng ta có được một bộ công cụ hữu ích, đồ sộ mà không tốn 1 xu.

- Other: còn rất nhiều điều nữa, có lẽ chúng ta sẽ khám phá tiếp :D 

## Học những gì?
- Libgdx: học các api cơ bản của Libgdx, chúng chủ yếu là java thuần.
- Xây dụng một thư viện của riêng chúng ta, giúp bạn tăng tốc khi làm các game tiếp theo.
- Học sử dụng các tool hỗ trợ: Hiero-tạo font, Skineditor-customize giao diện, Texturepacker-đóng gói resource.
- Làm một vài game: flappy bird, braindots, v.v.
- Tích hợp quảng cáo: google admob
- Làm một game multiplayer: trong mạng LAN và Online.
- Học đồ họa: sử dụng inkscape, gimp để clone,tạo đồ họa. Phần này có lẽ mình sẽ làm video.
- Dùng Spine để tạo animation.
- Up game lên store. Dự định là google play. Hy vọng đến lúc viết tới phần này sẽ có tiền làm up lên Apple store :D

**Hy vọng rằng tôi có đủ thời gian, công sức và nhiệt huyết để đi hết được loạt bài này**

*Mọi ý kiến đóng góp, thắc mắc, rất mong các bạn gửi mail vào địa chỉ tranminhluyen.1993ATgmailDOTcom*
