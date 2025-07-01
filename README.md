<div class="content">
    <h1>BÁO CÁO KIỂM THỬ HIỆU SUẤT JMETER</h1>
    <ol>
        <p><strong>Tên Dự Án:</strong> Load Testing trang CTSV Phenikaa</p>
        <p><strong>Ngày Kiểm Thử:</strong> 01/07/2025</p>
        <p><strong>Người Kiểm Thử:</strong> Vũ Minh Hiếu </p>
        <p><strong>1. Mục Tiêu Kiểm Thử:</strong> Sử dụng JMeter để kiểm tra hiệu năng trang web CTSV Phenikaa</p>
        <p><strong>2. Môi Trường Kiểm Thử:</strong> Phần mềm Apache JMeter 5.6.3</p>
        <p><strong>3. Phương Pháp Kiểm Thử:</strong> Kiểm thử tự động với các kịch bản mô phỏng nhiều người dùng truy cập đồng thời.</p>

        <p><strong>4. Kịch Bản Kiểm Thử lần 1:</strong></p>
        <ul>
            <li><p><strong>Tên Kịch Bản:</strong> Kiểm thử tải trang chủ CTSV</p></li>
            <li><p><strong>Mục Đích:</strong> Đánh giá khả năng phản hồi của trang chủ khi có ít người truy cập</p></li>
            <li><p><strong>HTTP request:</strong> https://ctsv.phenikaa-uni.edu.vn/</p></li>
            <li><p><strong>Số lượng người dùng (Threads):</strong> 10</p></li>
            <li><p><strong>Ramp-up period (giây):</strong> 5</p></li>
            <li><p><strong>Loop-count:</strong> 5</p></li>
            <li><p><strong>Kết Quả Mong Đợi:</strong> Trang chủ phản hồi đầy đủ, không lỗi</p></li>
            <li><p><strong>Kết Quả Thực Tế:</strong> Đã gửi yêu cầu thành công, không phát sinh lỗi</p></li>
            <li><p><strong>Trạng Thái:</strong> Thành công</p></li>
            <li><p><strong>Kết quả sau khi test:</strong></p></li>
            <img width="800" src="https://github.com/gtaAsian/Jmeter/assets/170786444/e9529079-f7f6-43e0-818d-535dc613f8c2">
            <li><p><strong>Thời gian phản hồi trung bình:</strong> 3.5 giây</p></li>
            <li><p><strong>Tỷ lệ yêu cầu thành công:</strong> 100%</p></li>
        </ul>

        <p><strong>Kịch Bản Kiểm Thử lần 2:</strong></p>
        <ul>
            <li><p><strong>Tên Kịch Bản:</strong> Kiểm thử chịu tải nhiều trang</p></li>
            <li><p><strong>Mục Đích:</strong> Kiểm tra khả năng chịu tải với nhiều người truy cập đồng thời vào các trang chức năng phổ biến</p></li>
            <li><p><strong>HTTP request:</strong></p>
                <ul>
                    <li><p>Trang chủ: https://ctsv.phenikaa-uni.edu.vn/</p></li>
                    <li><p>Trang đăng nhập: https://ctsv.phenikaa-uni.edu.vn/sinhvien/login</p></li>
                    <li><p>Trang thông báo: https://ctsv.phenikaa-uni.edu.vn/thongbao</p></li>
                </ul>
            </li>
            <li><p><strong>Số lượng người dùng (Threads):</strong> 50</p></li>
            <li><p><strong>Ramp-up period (giây):</strong> 15</p></li>
            <li><p><strong>Loop-count:</strong> 10</p></li>
            <li><p><strong>Kết Quả Mong Đợi:</strong> Các trang phản hồi đúng nội dung, hệ thống không bị treo hoặc sập</p></li>
            <li><p><strong>Kết Quả Thực Tế:</strong> Hệ thống xử lý ổn định, có một số yêu cầu thất bại khi tải cao</p></li>
            <li><p><strong>Trạng Thái:</strong> Đạt yêu cầu</p></li>
            <li><p><strong>Kết quả sau khi test:</strong></p></li>
            <img width="800" src="https://github.com/gtaAsian/Jmeter/assets/170786444/27faca0c-1cec-49be-82cc-068c472e6a80">
            <li><p><strong>Thời gian phản hồi trung bình:</strong> 6.2 giây</p></li>
            <li><p><strong>Tỷ lệ yêu cầu thành công:</strong> 92%</p></li>
        </ul>

        <p><strong>5. Kết Luận:</strong></p>
        <p>Trang CTSV của Phenikaa hoạt động ổn định trong điều kiện truy cập thông thường và chịu được tải cao ở mức trung bình. 
            Tuy nhiên, khi số lượng người dùng vượt ngưỡng 50 đồng thời, cần theo dõi thêm để tối ưu hệ thống.</p>
</div>
