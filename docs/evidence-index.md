| Em thử gì | Kết quả | Ảnh/link (nếu có) |
|---|---|---|
| Cấu trúc HTML5 và nhãn biểu mẫu | Đã kiểm tra tĩnh: cả hai trang có `header`, `nav`, `main`, `section`, `footer`; các `label for` trỏ tới ID có thật. | [index.html](../index.html), [ket-qua.html](../ket-qua.html) |
| Thuộc tính bốn trường form | Chưa đạt đủ: `ho-ten`, `dong-may-dich-vu`, `mo-ta` có `required`, `minlength`, `maxlength`, `aria-describedby`. `email` có `required` và `aria-describedby` nhưng thiếu `minlength`/`maxlength`. | [index.html](../index.html) |
| Đường dẫn tuyệt đối và đường dẫn cục bộ | Không tìm thấy `C:\`, `file:///`, `href="/"` hoặc `src="/"` trong các tệp văn bản được quét. Liên kết menu/trang đích và stylesheet cục bộ có đích tồn tại. | [index.html](../index.html), [ket-qua.html](../ket-qua.html), [style.css](../css/style.css) |
| Đối chiếu ảnh trong HTML với `assets/images/` | Đã kiểm tra đủ 5 ảnh: `avatar-an.jpg`, `banner-laptop.jpg`, `cai-win-phan-mem.jpg`, `nang-cap-ssd.jpg`, `ve-sinh-laptop.jpg`; khớp chính xác, không thiếu/không dư. Cả 5 ảnh tải được ở trang cục bộ. | [Thư mục ảnh](../assets/images/) |
| Class HTML, trạng thái và responsive CSS | Tất cả class dùng trong HTML đều có quy tắc CSS; có `:hover` và `:focus-visible`. Hai trang được xem ở viewport 375px; `scrollWidth` bằng `clientWidth`, không thấy tràn ngang. | [style.css](../css/style.css) |
| Bấm menu Giới thiệu, Dịch vụ, Bảng giá, Liên hệ | Đã bấm từng mục ở trang cục bộ; mỗi mục chuyển tới đúng fragment tương ứng. | [index.html](../index.html) |
| Gửi biểu mẫu hợp lệ | Đã gửi bộ dữ liệu mẫu trên GitHub Pages bằng `requestSubmit()`; trình duyệt mở `ket-qua.html` với trang xác nhận mô phỏng. Form dùng `GET`, dữ liệu nằm trong query URL; không có máy chủ nhận/lưu dữ liệu. | [index.html](../index.html), [ket-qua.html](../ket-qua.html), [form-submit-ket-qua.png](../evidence/form-submit-ket-qua.png) |
| Quét mẫu token/mật khẩu | Không phát hiện mẫu credential phổ biến trong các tệp văn bản đọc được. Đây không phải kiểm toán bảo mật toàn diện; tên, MSSV, lớp và trường của sinh viên có trong HTML theo nội dung trang. | Tệp HTML trong workspace |
| Mở URL GitHub Pages trong cửa sổ ẩn danh | Chưa kiểm tra. | Không có ảnh; URL giữ trong [README.md](../README.md) |
| Kiểm tra website công khai trên GitHub Pages | Đã mở được URL công khai và chụp toàn trang ở viewport 1440 × 900; ảnh xác nhận bố cục ba cột dịch vụ. | [pages-live-1440px.png](../evidence/pages-live-1440px.png) |
| Kiểm tra trên iPhone thật | Chưa kiểm tra. | Không có ảnh |
| Ảnh chụp màn hình làm bằng chứng | Đã lưu 5 ảnh PNG trong `evidence/`; các tệp đều có nội dung và kích thước khác 0. Chi tiết kích thước và điều kiện chụp bên dưới. | [Thư mục evidence](../evidence/) |

### Ảnh chụp đã lưu

| Tệp | Nội dung / kết quả kiểm tra |
|---|---|
| [mobile-320px.png](../evidence/mobile-320px.png) | Toàn trang `index.html`, viewport 320 × 800. Bố cục dịch vụ một cột; menu xuống dòng; bảng rộng 608 CSS px nằm trong wrapper cuộn ngang; `scrollWidth` và `clientWidth` của tài liệu đều 305 CSS px, không tràn ngang. Chụp từ workspace qua `file:///` vì không khởi động được HTTP server trong môi trường này. |
| [desktop-1440px.png](../evidence/desktop-1440px.png) | Toàn trang `index.html`, viewport 1440 × 900. Grid dịch vụ có 3 cột; `.container` rộng 1152 CSS px. Chụp từ workspace qua `file:///`. |
| [form-validation-error.png](../evidence/form-validation-error.png) | Trang live ở viewport 1440 × 900 sau khi gửi form với email `not-an-email`; `:user-invalid` đúng và trường email hiển thị viền lỗi cùng thông báo định dạng HTML5. |
| [form-submit-ket-qua.png](../evidence/form-submit-ket-qua.png) | Trang xác nhận live sau khi gửi form hợp lệ với dữ liệu mẫu; URL nhận GET là `https://antienbui0607-crypto.github.io/an-tech-care/ket-qua.html?ho-ten=Nguyen+Van+A&email=test%40example.com&dong-may-dich-vu=Ve+sinh+laptop&mo-ta=May+nong+va+quat+keu+to+can+ve+sinh`. Ảnh chụp nội dung trang bằng Playwright không bao gồm thanh địa chỉ trình duyệt. |
| [pages-live-1440px.png](../evidence/pages-live-1440px.png) | Toàn trang GitHub Pages tại viewport 1440 × 900; xác nhận 3 cột dịch vụ, container rộng 1152 CSS px và không tràn ngang. |

Đã xác nhận cả 5 PNG tồn tại và có kích thước tệp lớn hơn 0; ảnh được chụp ở device scale factor 1.25. Ảnh chụp trang không chứa thanh trình duyệt/URL bar; URL GET đầy đủ được ghi tại dòng tương ứng để đối chiếu. Ảnh local dùng `file:///` vì HTTP server không khởi động được trong môi trường này.
