## V1 – 23/11/2026

- Đã rà soát `index.html`, `ket-qua.html`, `css/style.css` và tài liệu bàn giao; không thấy mẫu đường dẫn tuyệt đối hoặc root-relative thuộc các dạng được yêu cầu kiểm tra.
- Đối chiếu 5 tệp ảnh trong `assets/images/` với các thẻ `<img>`: tên khớp chính xác, không thiếu/không dư; cả 5 ảnh tải được khi mở trang cục bộ.
- Kiểm tra cấu trúc ngữ nghĩa, nhãn form, liên kết menu, các class CSS, `:hover`/`:focus-visible`; thử menu, gửi biểu mẫu hợp lệ và mở trang kết quả trong trình duyệt cục bộ.
- Thử hai trang ở viewport 375px: không thấy tràn ngang. Quét mẫu thông tin đăng nhập phổ biến trên các tệp văn bản đọc được, không phát hiện token/mật khẩu; thông tin tên, MSSV, lớp và trường vẫn hiện trong HTML theo nội dung trang.
- Cập nhật README, evidence index và nhật ký AI để ghi lại kết quả thực tế, kể cả giới hạn và hạng mục chưa kiểm tra.
- Phát hiện chưa đáp ứng đủ yêu cầu thuộc tính form: trường `email` thiếu `minlength` và `maxlength`; chưa sửa HTML/CSS trong đợt cập nhật tài liệu này.
- Xác nhận biểu mẫu dùng `GET`: dữ liệu mẫu chuyển thành query trên URL trang kết quả; không có máy chủ nhận/lưu dữ liệu. Không nên nhập dữ liệu nhạy cảm vào luồng mô phỏng.

### Chưa kiểm tra

- Chưa mở URL GitHub Pages trực tiếp, nên chưa xác nhận website công khai/Pages đã bật; chưa chạy trong cửa sổ ẩn danh.
- Chưa kiểm tra trên thiết bị iPhone thật; chưa chạy kiểm thử bảo mật chuyên sâu. Quét credential chỉ là dò mẫu phổ biến, không phải bảo đảm an toàn tuyệt đối.
- Chưa lưu ảnh chụp màn hình kiểm thử. Chưa kiểm tra các trường hợp nhập sai/biên của biểu mẫu ngoài việc gửi một bộ dữ liệu hợp lệ.
