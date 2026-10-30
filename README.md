# Portfolio cá nhân — Khoàng Trung Hiếu

Portfolio tĩnh được xây dựng bằng HTML và CSS cho học phần **FIT4014 — Thiết kế Web và triển khai hệ thống phần mềm**. Đây là bản bàn giao portfolio v7 cho bài đánh giá A2.2.

## Nội dung

- Giới thiệu, kỹ năng, dự án và lộ trình học tập.
- Bố cục responsive, điều hướng tới các phần và trạng thái focus cho bàn phím.
- Biểu mẫu liên hệ có kiểm tra dữ liệu HTML5. Biểu mẫu chỉ mô phỏng; không gửi email và không lưu dữ liệu.
- Trang [ket-qua.html](./ket-qua.html) giải thích kết quả gửi thử.

## Chạy và kiểm tra trên máy

1. Tải hoặc clone repository.
2. Mở `index.html` trực tiếp trong trình duyệt, hoặc mở thư mục bằng VS Code và chạy bằng tiện ích Live Server.
3. Kiểm tra các liên kết điều hướng, CSS responsive và biểu mẫu ở cuối trang. Dùng dữ liệu giả khi thử gửi: biểu mẫu GET có thể đưa dữ liệu vào URL và lịch sử trình duyệt.

Tệp chính:

- [index.html](./index.html) — trang portfolio.
- [css/style.css](./css/style.css) — giao diện và bố cục responsive.
- [ket-qua.html](./ket-qua.html) — trang kết quả mô phỏng.
- [AI_LOG.md](./AI_LOG.md) — vấn đề, quyết định và kiểm chứng có hỗ trợ AI.
- [RELEASE_NOTES.md](./RELEASE_NOTES.md) — ghi chú bản bàn giao.
- [CHECKLIST.md](./CHECKLIST.md) — checklist kiểm chứng và triển khai.

## Repository và GitHub Pages

- Repository: <https://github.com/Hieu492003/2071020070_khoangtrunghieu_lab5>
- URL Pages dự kiến: <https://hieu492003.github.io/2071020070_khoangtrunghieu_lab5/>
- Nguồn triển khai phù hợp với cấu trúc hiện tại: nhánh `main`, thư mục gốc `/` (nơi đặt `index.html`).

**Trạng thái:** URL Pages và API cấu hình Pages trả về HTTP 404 trong lần kiểm tra ngày 30/10/2026; chưa xác nhận có bản triển khai công khai. Sau khi push bản sửa, kiểm tra Settings → Pages; nếu chưa bật, chọn nhánh `main` và thư mục `/(root)`, đợi deploy rồi kiểm tra lại URL trước khi nộp.

## Cải tiến giao diện và kiểm chứng

- **Vấn đề trước khi sửa:** `index.html` trỏ tới `css/` thay vì `css/style.css`; stylesheet không được nạp nên giao diện mất màu, bố cục và trạng thái focus.
- **Tiêu chí:** trang phải nạp stylesheet cục bộ, giữ bố cục responsive, thể hiện màu nhận diện và cho phép nhìn rõ con trỏ/focus trong trường nhập.
- **Cách sửa:** khôi phục đường dẫn stylesheet; giữ cỡ chữ 16px và trạng thái hover/focus của các trường nhập.
- **Kiểm chứng cục bộ:** máy chủ HTTP trả 200 cho `index.html` và `css/style.css`; trình duyệt áp dụng màu nút, trường nhập 16px, nhập được dữ liệu và không tràn ngang ở viewport 375px. Biểu mẫu hợp lệ mở trang kết quả mô phỏng; chỉ dùng dữ liệu giả vì GET đưa dữ liệu vào URL.
- **Kiểm chứng công khai:** chưa thực hiện thành công; URL GitHub Pages hiện trả HTTP 404.
- **Minh chứng:** cần chụp ảnh trước/sau trên cùng viewport và ảnh Network của bản sau khi sửa; bổ sung link ảnh hoặc video demo tại đây sau khi lưu minh chứng. Không đánh dấu deploy là hoàn tất trước khi URL công khai mở được.

## Thông tin nộp LMS

Điền thông tin cá nhân/lớp và SHA sau khi tạo commit cuối, push, triển khai và kiểm chứng:

| Thông tin | Giá trị |
|---|---|
| Họ tên — MSSV — lớp | Khoàng Trung Hiếu — 2071020070 — bổ sung lớp |
| Link repository | <https://github.com/Hieu492003/2071020070_khoangtrunghieu_lab5> |
| URL GitHub Pages đã kiểm tra | Chưa triển khai; URL dự kiến ở trên |
| Nhánh / thư mục nguồn | `main` / `/ (root)` |
| SHA mã nguồn đã kiểm thử và push | `fe942990948ca1db8a9722e42523222bd71fa176` (chưa xác nhận được bản deploy vì URL Pages trả HTTP 404) |
| Hồ sơ | README, AI_LOG, RELEASE_NOTES và CHECKLIST trong repository |
| Minh chứng / demo | Bổ sung ảnh Network, ảnh cải tiến giao diện và video demo sau khi deploy |
