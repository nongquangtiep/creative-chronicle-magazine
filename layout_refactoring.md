# Báo Cáo Phân Tích & Tái Cấu Trúc Bố Cục

Kỹ thuật `position: absolute` nhấc bổng phần tử ra khỏi luồng tài liệu thông thường (*Normal Flow*), khiến thẻ cha hoàn toàn mất chiều cao thực tế (bị co sụp về 0px nếu không gán chiều cao cứng). Khi hiển thị trên di động, việc cố định `height: 400px` và neo các tọa độ `top`, `bottom`, `right` bằng phần trăm cố định khiến các phần tử con đè bẹp lên nhau và che khuất hoàn toàn nội dung bài viết bên dưới.

CSS Grid là giải pháp cứu cánh toàn diện cho bài toán 2D này. Grid cho phép thiết lập hệ thống lưới tự nhiên theo tỉ lệ phân số (`2fr 1fr`), quản lý hàng và cột độc lập mà không cần neo tọa độ. Các ảnh con tự ôm trọn ô lưới được chỉ định bằng `grid-row: 1 / 3`, giữ nguyên chiều cao tự nhiên của thẻ cha và linh hoạt chuyển về dạng 1 cột đơn giản trên màn hình nhỏ mà không cần tính toán thủ công.
