## Nhật ký hỗ trợ AI

### Bối cảnh và quan sát

- Phản hồi ban đầu: màu giao diện không hiển thị và không nhập được chữ ở phần liên hệ.
- Kiểm tra trang `index.html` trên trình duyệt cục bộ: stylesheet `css/style.css` được tải; màu nền, màu chữ và nút chính được áp dụng. Các trường nhập không bị `disabled` hoặc `readonly`, và có thể nhập dữ liệu thử nghiệm.
- Tệp `ai_log.md` ban đầu chỉ ghi lại hai dòng phản hồi này; nội dung được chuyển thành nhật ký có quan sát, quyết định và kết quả kiểm thử trong `AI_LOG.md`.

### Quyết định và thay đổi

- Không thêm JavaScript và không đổi cách gửi biểu mẫu tĩnh, vì lỗi nhập liệu không tái hiện được.
- Tăng cỡ chữ trường nhập lên 16px để tránh phóng to trang ngoài ý muốn trên một số điện thoại; thêm màu con trỏ và trạng thái viền khi rê chuột.
- Sửa liên kết email để khớp địa chỉ đang hiển thị trên trang.

### Kiểm chứng

- Đã kiểm tra stylesheet được trình duyệt tải và các màu giao diện được áp dụng.
- Đã nhập dữ liệu giả, gửi biểu mẫu và xác nhận trang kết quả mô phỏng cảnh báo rằng email không được gửi.
- Cần kiểm tra lại URL GitHub Pages sau khi bật triển khai; lần kiểm tra hiện tại trả về HTTP 404.
