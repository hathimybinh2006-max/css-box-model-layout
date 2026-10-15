# Xây Dựng Bố Cục Với Mô Hình Hộp CSS (CSS Box Model Layout)

Bài thực hành so sánh sự khác biệt thực tế giữa `box-sizing: content-box` và `box-sizing: border-box`.

## Thông số kỹ thuật của các thẻ
- Khai báo kích thước: `width: 280px`, `height: 150px`
- Phần đệm: `padding: 20px` (ở cả 4 cạnh)
- Đường viền: `border: 5px solid #3498db` (ở cả 4 cạnh)
- Khoảng cách lề: `margin: 20px`

## So sánh kích thước hiển thị thực tế trên trình duyệt (Computed Tab)

| Thuộc tính | Thẻ 1 (`content-box`) | Thẻ 2 & 3 (`border-box`) |
| :--- | :--- | :--- |
| **Khai báo** | `280px × 150px` | `280px × 150px` |
| **Vùng nội dung** | `280px × 150px` | `230px × 100px` (đã trừ padding & border) |
| **Tổng chiều rộng** | `280 + 20×2 + 5×2 = 330px` | `280px` (Cố định chuẩn xác) |
| **Tổng chiều cao** | `150 + 20×2 + 5×2 = 200px` | `150px` (Cố định chuẩn xác) |
| **Màu nền** | `#2ecc71` (Xanh lá cây) | `#f1c40f` (Vàng) & `#e74c3c` (Đỏ) |
