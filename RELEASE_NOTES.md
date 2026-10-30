# Release notes

## v7 — 2026-10-30

### Cải tiến

- Khôi phục đường dẫn stylesheet bị sai (`css/` → `css/style.css`), sửa nguyên nhân giao diện không có màu và bố cục.
- Tăng cỡ chữ trường liên hệ lên 16px, thêm màu con trỏ và trạng thái hover để dễ nhận biết vùng nhập, đặc biệt trên điện thoại.
- Sửa đích liên kết email để trùng với địa chỉ hiển thị.
- Chuyển ghi chú phản hồi ban đầu thành nhật ký AI có quyết định và kết quả kiểm chứng.
- Bổ sung hướng dẫn chạy, kiểm chứng, triển khai và hồ sơ nộp bài; mô tả rõ trạng thái Pages chưa xác minh.

### Kiểm chứng

- Máy chủ HTTP cục bộ trả 200 cho HTML và CSS; trình duyệt xác nhận màu, nhập liệu, responsive 375px và kết quả biểu mẫu mô phỏng.
- URL GitHub Pages dự kiến hiện trả về HTTP 404; cần bật Pages và kiểm tra lại sau deploy.

### Hạn chế và bàn giao

- Biểu mẫu là mô phỏng tĩnh, không gửi email và không lưu dữ liệu.
- Mã nguồn đã push tại commit `fe942990948ca1db8a9722e42523222bd71fa176`; chưa có ảnh minh chứng trước/sau hoặc video demo được lưu trong repository.
- Cần bật/cấu hình Pages, xác nhận URL công khai và bổ sung minh chứng; theo dõi các mục còn lại trong [CHECKLIST.md](./CHECKLIST.md).
