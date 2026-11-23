# AnTech Care - Chăm sóc Laptop Sinh viên

## Sản phẩm này là gì?
AnTech Care là website tĩnh giới thiệu dịch vụ vệ sinh, nâng cấp và cài đặt laptop cho sinh viên. Trang giới thiệu Bùi Tiến An, sinh viên CNTT 20-04, Đại học Đại Nam.

## Demo
- GitHub Pages: https://antienbui0607-crypto.github.io/an-tech-care/  
  URL được giữ nguyên từ README trước; chưa xác minh trực tiếp trong lượt kiểm thử này.
- Repository: https://github.com/antienbui0607-crypto/an-tech-care

## Tính năng
- Menu **Giới thiệu**, **Dịch vụ**, **Bảng giá**, **Liên hệ** dẫn tới các mục tương ứng.
- Nút **Xem dịch vụ** chuyển tới phần dịch vụ.
- Giới thiệu ba nhóm dịch vụ, bảng giá tham khảo và quy trình nhận máy.
- Biểu mẫu gồm Họ và tên, Email, Dòng máy / dịch vụ cần hỗ trợ, Mô tả tình trạng máy; nút **Gửi yêu cầu đặt lịch** mở trang xác nhận mô phỏng `ket-qua.html`.
- Bố cục hỗ trợ màn hình hẹp, có trạng thái focus bàn phím.

## Cách mở
1. Mở `index.html` trực tiếp trong trình duyệt để xem bản cục bộ; `css/style.css` và ảnh được tham chiếu bằng đường dẫn tương đối.
2. Dùng các mục **Giới thiệu**, **Dịch vụ**, **Bảng giá**, **Liên hệ** hoặc nút **Xem dịch vụ** để điều hướng.
3. Điền biểu mẫu rồi bấm **Gửi yêu cầu đặt lịch** để mở `ket-qua.html`. Đây là luồng thử nghiệm tĩnh, không gửi/lưu dữ liệu trên máy chủ; do dùng `GET`, dữ liệu biểu mẫu xuất hiện trong URL.
4. Có thể mở URL GitHub Pages ở mục Demo, nhưng trạng thái triển khai công khai chưa được kiểm tra trong lượt này.

## Cấu trúc thư mục
```text
.
|-- index.html
|-- ket-qua.html
|-- css/
|   `-- style.css
|-- assets/
|   `-- images/
|       |-- avatar-an.jpg
|       |-- banner-laptop.jpg
|       |-- cai-win-phan-mem.jpg
|       |-- nang-cap-ssd.jpg
|       `-- ve-sinh-laptop.jpg
|-- docs/
|   |-- AI_LOG.md
|   `-- evidence-index.md
|-- CHANGELOG.md
`-- README.md
```

## Đã kiểm tra
- Hai trang có các thẻ `header`, `nav`, `main`, `section`, `footer`; nhãn biểu mẫu khớp với ID điều khiển.
- Không thấy đường dẫn tuyệt đối/root-relative theo các mẫu được rà soát; cả 5 ảnh có tên khớp và tải được khi mở trang cục bộ.
- Các class HTML đều có quy tắc CSS; có `:hover`/`:focus-visible`. Thử cục bộ ở viewport 375px không thấy tràn ngang.
- Menu đã được bấm qua các mục; biểu mẫu hợp lệ đã điều hướng tới `ket-qua.html`.
- Quét theo mẫu credential phổ biến không phát hiện token/mật khẩu. Mã nguồn vẫn có tên, MSSV, lớp và trường của sinh viên theo nội dung trang.
- Chi tiết từng bước và giới hạn kiểm tra: [docs/evidence-index.md](docs/evidence-index.md).

## Hạn chế / Chưa kiểm tra
- Trường Email hiện có `required` và `aria-describedby`, nhưng chưa có `minlength`/`maxlength`; ba trường còn lại có đủ bốn thuộc tính kiểm tra được yêu cầu.
- Chưa xác minh URL GitHub Pages trực tiếp, trình duyệt ẩn danh hoặc hiển thị trên iPhone thật; chưa chạy kiểm tra bảo mật chuyên sâu.
- Chưa lưu ảnh chụp màn hình làm bằng chứng. Biểu mẫu dùng GET nên dữ liệu xuất hiện trong URL/trình duyệt, dù không gửi/lưu lên máy chủ; không dùng luồng mô phỏng này cho dữ liệu nhạy cảm.

## Khai báo AI
GitHub Copilot hỗ trợ rà soát tĩnh mã nguồn và cập nhật tài liệu bàn giao. Xem [docs/AI_LOG.md](docs/AI_LOG.md); các kiểm tra chưa chạy và phần sinh viên cần tự xác nhận được ghi riêng.
