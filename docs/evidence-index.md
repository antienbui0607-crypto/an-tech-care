| Em thử gì | Kết quả | Ảnh/link (nếu có) |
|---|---|---|
| Cấu trúc HTML5 và nhãn biểu mẫu | Đã kiểm tra tĩnh: cả hai trang có `header`, `nav`, `main`, `section`, `footer`; các `label for` trỏ tới ID có thật. | [index.html](../index.html), [ket-qua.html](../ket-qua.html) |
| Thuộc tính bốn trường form | Chưa đạt đủ: `ho-ten`, `dong-may-dich-vu`, `mo-ta` có `required`, `minlength`, `maxlength`, `aria-describedby`. `email` có `required` và `aria-describedby` nhưng thiếu `minlength`/`maxlength`. | [index.html](../index.html) |
| Đường dẫn tuyệt đối và đường dẫn cục bộ | Không tìm thấy `C:\`, `file:///`, `href="/"` hoặc `src="/"` trong các tệp văn bản được quét. Liên kết menu/trang đích và stylesheet cục bộ có đích tồn tại. | [index.html](../index.html), [ket-qua.html](../ket-qua.html), [style.css](../css/style.css) |
| Đối chiếu ảnh trong HTML với `assets/images/` | Đã kiểm tra đủ 5 ảnh: `avatar-an.jpg`, `banner-laptop.jpg`, `cai-win-phan-mem.jpg`, `nang-cap-ssd.jpg`, `ve-sinh-laptop.jpg`; khớp chính xác, không thiếu/không dư. Cả 5 ảnh tải được ở trang cục bộ. | [Thư mục ảnh](../assets/images/) |
| Class HTML, trạng thái và responsive CSS | Tất cả class dùng trong HTML đều có quy tắc CSS; có `:hover` và `:focus-visible`. Hai trang được xem ở viewport 375px; `scrollWidth` bằng `clientWidth`, không thấy tràn ngang. | [style.css](../css/style.css) |
| Bấm menu Giới thiệu, Dịch vụ, Bảng giá, Liên hệ | Đã bấm từng mục ở trang cục bộ; mỗi mục chuyển tới đúng fragment tương ứng. | [index.html](../index.html) |
| Gửi biểu mẫu hợp lệ | Đã nhập dữ liệu thử và bấm **Gửi yêu cầu đặt lịch**; trình duyệt mở `ket-qua.html` với trang xác nhận mô phỏng. Form dùng `GET`, dữ liệu nằm trong query URL; không có máy chủ nhận/lưu dữ liệu. Không nhập dữ liệu nhạy cảm. | [index.html](../index.html), [ket-qua.html](../ket-qua.html) |
| Quét mẫu token/mật khẩu | Không phát hiện mẫu credential phổ biến trong các tệp văn bản đọc được. Đây không phải kiểm toán bảo mật toàn diện; tên, MSSV, lớp và trường của sinh viên có trong HTML theo nội dung trang. | Tệp HTML trong workspace |
| Mở URL GitHub Pages trong cửa sổ ẩn danh | Chưa kiểm tra. | Không có ảnh; URL giữ trong [README.md](../README.md) |
| Kiểm tra website công khai trên GitHub Pages | Chưa kiểm tra trực tiếp; chưa xác nhận Pages đã bật. | Không có ảnh |
| Kiểm tra trên iPhone thật | Chưa kiểm tra. | Không có ảnh |
| Ảnh chụp màn hình làm bằng chứng | Chưa lưu ảnh kiểm thử trong workspace. | Không có |
