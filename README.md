# BÁO CÁO KIỂM THỬ HIỆU SUẤT JMETER

**Ngày Kiểm Thử:** 01/07/2025  
**Người Kiểm Thử:** Vũ Minh Hiếu  

## 1. Mục Tiêu Kiểm Thử
Sử dụng JMeter để kiểm tra hiệu năng trang web CTSV Phenikaa.

## 2. Môi Trường Kiểm Thử
Phần mềm Apache JMeter 5.6.3

## 3. Phương Pháp Kiểm Thử
Kiểm thử tự động với các kịch bản mô phỏng nhiều người dùng truy cập đồng thời.

---

## 4. Kịch Bản Kiểm Thử lần 1

- **Tên Kịch Bản:** Kiểm thử tải trang chủ CTSV
- **Mục Đích:** Đánh giá khả năng phản hồi của trang chủ khi có ít người truy cập
- **HTTP Request:** [https://ctsv.phenikaa-uni.edu.vn](https://ctsv.phenikaa-uni.edu.vn)
- **Số lượng người dùng (Threads):** 10
- **Ramp-up period (giây):** 5
- **Loop-count:** 5
- **Kết Quả Mong Đợi:** Trang chủ phản hồi đầy đủ, không lỗi
- **Kết Quả Thực Tế:** Đã gửi yêu cầu thành công, không phát sinh lỗi
- **Kết quả sau khi test:**  
![Kết quả test](https://github.com/gtaAsian/Jmeter/assets/170786444/e9529079-f7f6-43e0-818d-535dc613f8c2)
- **Thời gian phản hồi trung bình:** 3.5 giây
- **Tỷ lệ yêu cầu thành công:** 100%

---

## 5. Kịch Bản Kiểm Thử lần 2

- **Tên Kịch Bản:** Kiểm thử chịu tải nhiều trang
- **Mục Đích:** Kiểm tra khả năng chịu tải với nhiều người truy cập đồng thời vào các trang chức năng khác nhau
- **HTTP Request:** https://ctsv.phenikaa-uni.edu.vn + Các trang chức năng phụ
- **Số lượng người dùng (Threads):** 50
- **Ramp-up period (giây):** 10
- **Loop-count:** 10
- **Kết Quả Mong Đợi:** Tất cả trang phản hồi đầy đủ, tốc độ chấp nhận được
- **Kết Quả Thực Tế:** Có 1 số trang phản hồi chậm, tỷ lệ lỗi 2%
- **Kết quả sau khi test:**  
![Kết quả test](https://github.com/gtaAsian/Jmeter/assets/170786444/f8ef453a-c512-40f7-a294-049710fc8436)
- **Thời gian phản hồi trung bình:** 6.2 giây
- **Tỷ lệ yêu cầu thành công:** 98%

---

## 6. Kết luận
Trang web hoạt động tương đối ổn định, tuy nhiên cần tối ưu hiệu năng cho các trang chức năng khi lượng người dùng cao.

---


