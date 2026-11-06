# Nhật ký hỗ trợ AI

Nhật ký ghi lại phần AI hỗ trợ; người học cần tự xem lại mã và xác nhận các kết quả trước khi nộp.

## Sự cố và cách xử lý trước đó

- Đường dẫn stylesheet từng bị đổi từ `css/style.css` thành `css/`, khiến trang không nạp CSS. Đã khôi phục đường dẫn trong `index.html`.
- Biểu mẫu liên hệ là mô phỏng tĩnh: HTML5 kiểm tra dữ liệu rồi chuyển sang `ket-qua.html`; biểu mẫu không gửi email và không lưu dữ liệu.
- Đã sửa liên kết email và giữ cỡ chữ trường nhập 16px, cùng trạng thái focus dễ nhận biết.

## Kết quả kiểm chứng được ghi nhận trước đây

- Máy chủ HTTP cục bộ trả HTTP 200 cho `index.html` và `css/style.css`.
- Trình duyệt xác nhận stylesheet được áp dụng, trường nhập nhận dữ liệu và biểu mẫu chuyển tới trang kết quả với dữ liệu giả.
- Ở viewport 375px, tài liệu không tràn ngang.
- URL GitHub Pages từng trả HTTP 404; chưa có bằng chứng deploy trực tuyến thành công.
- Commit `fe942990948ca1db8a9722e42523222bd71fa176` được ghi nhận đã push lên `main`. Trạng thái deploy và nội dung trực tuyến cần được kiểm tra lại.

## Hỗ trợ hồ sơ Lab 8 ngày 2026-11-06

- Sắp xếp tài liệu bàn giao trong `docs/`, thêm checklist và tạo báo cáo Word từ các thông tin đã có trong repository.
- Các mục chưa thực hiện hoặc chưa có ảnh được ghi rõ là đang chờ; không tự điền tên bạn học, góp ý, kết quả deploy hay ảnh minh chứng.
- Người học cần đọc lại báo cáo, điền phần kiểm tra chéo sau khi thực hiện thật và bổ sung ảnh trong `docs/evidence/` trước khi nộp.
