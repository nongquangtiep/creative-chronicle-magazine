# Nhật Ký Truy Vấn AI (AI Prompt Log)

- **Câu hỏi 1 (CSS Grid span & aspect-ratio):** "Làm thế nào để tạo bố cục ảnh khảm (Mosaic) 1 ảnh lớn bên trái chiếm 2 hàng và 2 ảnh nhỏ bên phải bằng CSS Grid mà không cần cố định chiều cao bằng px?"
  - *Ứng dụng:* Dùng `grid-template-columns: 2fr 1fr;` kết hợp `grid-row: 1 / 3;` cho `.photo-main` và `object-fit: cover` cho thẻ ảnh.

- **Câu hỏi 2 (Bootstrap Responsive Breakpoints):** "Cách chia 4 card bài viết để hiển thị 4 cột trên Desktop (>=992px), 2 cột trên Tablet (>=768px) và 1 cột trên Mobile (<768px) bằng hệ thống lưới của Bootstrap 5?"
  - *Ứng dụng:* Áp dụng bộ class chuẩn `col-12 col-md-6 col-lg-3` vào từng phần tử con trong hàng `<div class="row g-4">`.

- **Câu hỏi 3 (Bootstrap Flex Utilities):** "Các class tiện ích Bootstrap nào thay thế nhanh chóng cho CSS `display: flex`, căn giữa dọc và tự xuống dòng trên điện thoại?"
  - *Ứng dụng:* Thay thế hoàn toàn code CSS thanh Author bằng `d-flex justify-content-between align-items-center flex-wrap gap-3`.
