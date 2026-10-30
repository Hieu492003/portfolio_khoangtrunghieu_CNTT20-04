## Nhật ký hỗ trợ AI

### Bối cảnh và quan sát

- Phản hồi ban đầu: màu giao diện không hiển thị và không nhập được chữ ở phần liên hệ.
- Commit `f187b86` đã vô tình đổi đường dẫn stylesheet trong `index.html` từ `css/style.css` thành `css/`. Trình duyệt không thể nạp tệp CSS, khiến giao diện mất màu và định dạng.
- Lần kiểm tra trình duyệt trước đó diễn ra trước thay đổi này nên không phản ánh đúng phiên bản mới nhất. URL GitHub Pages cũng trả HTTP 404; không có bản triển khai trực tuyến để đối chiếu.

### Quyết định và thay đổi

- Khôi phục liên kết chính xác tới `css/style.css`; không thêm JavaScript vì biểu mẫu không cần mã phía máy khách để nhận dữ liệu và kiểm tra ràng buộc HTML.
- Giữ cỡ chữ trường nhập 16px, màu con trỏ và viền hover/focus để vùng nhập dễ nhận biết, đồng thời hạn chế tự phóng to trên điện thoại.
- Sửa liên kết email để khớp địa chỉ hiển thị.

### Kiểm chứng

- Máy chủ HTTP cục bộ trả HTTP 200 cho `index.html` và `css/style.css`.
- Trình duyệt xác nhận stylesheet có 192 quy tắc, màu nút chính được áp dụng, trường nhập hiển thị cỡ chữ 16px và nhận dữ liệu.
- Ở viewport 375px (chiều rộng trang khả dụng 360px), chiều rộng tài liệu bằng chiều rộng viewport, không tràn ngang.
- Biểu mẫu hợp lệ với dữ liệu giả, mở `ket-qua.html` và hiển thị cảnh báo không gửi email; dữ liệu GET xuất hiện trong URL.
- URL GitHub Pages vẫn trả HTTP 404. Cần bật/khôi phục deploy, xác nhận URL công khai, ghi SHA bản deploy và bổ sung ảnh minh chứng/video.
