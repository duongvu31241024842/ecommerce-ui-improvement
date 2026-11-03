# E-commerce UI Improvement

## 1. Giới thiệu
Bài tập cá nhân môn Phát triển ứng dụng WEB/TMĐT.

- **Buổi 1:** khảo sát website bán cà phê Phương Vy Coffee và thiết kế lại thẻ sản phẩm ở trang danh mục bằng HTML/CSS.
- **Buổi 2:** tiếp tục hoàn thiện cùng sản phẩm đó, thực hành HTML5 ngữ nghĩa, CSS selector, Box Model, Flexbox, CSS Grid, hiệu ứng hover/focus, kiểm tra giao diện và tự sửa lỗi.

Khu vực trọng tâm là danh sách 4 thẻ sản phẩm. Mỗi thẻ hiển thị hình ảnh, tên, loại hạt, mức rang, cách pha phù hợp, giá và các nút thao tác để khách dễ so sánh sản phẩm.

## 2. Website tham khảo và khu vực đã cải tiến
- Tên website: Phương Vy Coffee
- URL: https://phuongvycoffee.com
- Khu vực đã khảo sát: trang chủ, danh mục sản phẩm, chi tiết sản phẩm, tìm kiếm, giỏ hàng.
- Khu vực đã cải tiến: danh sách thẻ sản phẩm ở trang danh mục, kèm menu điều hướng ở đầu trang.

## 3. Kỹ thuật HTML5/CSS3 đã thực hành
- **HTML5 ngữ nghĩa:** `header`, `nav`, `main`, `section`, `article`, `footer`, thứ bậc tiêu đề `h1` → `h2`, `img` có `alt`, `ul`/`li` cho nhóm nhãn, `a` cho liên kết, `del` cho giá gốc, `aria-label` cho liên kết "Xem chi tiết".
- **CSS tách file:** `css/style.css`, dùng biến màu ở `:root`, `box-sizing: border-box`.
- **Selector:** element selector (`a`), class selector (`.price`, `.price-new`), descendant selector (`.product-card .btn-detail`).
- **Box Model:** `margin`, `padding`, `border`, `border-radius` cho thẻ sản phẩm, giá và nút.
- **Flexbox:** menu điều hướng (`.nav-menu`), nhóm thao tác trong thẻ (`.product-actions`), nội dung bên trong thẻ; dùng `display: flex`, `justify-content`, `align-items`, `gap`, `flex-direction`.
- **CSS Grid:** lưới sản phẩm (`.product-grid`) với `grid-template-columns: repeat(...)` và `gap`; ảnh dùng `aspect-ratio` và `object-fit: cover`.
- **Responsive:** `@media` đổi lưới từ 4 cột sang 3 cột (dưới 900px) và 2 cột (dưới 600px).
- **Hover và focus:** `:hover`, `:focus-visible`, `:active` kèm `transition` cho liên kết "Xem chi tiết" và nút "Thêm vào giỏ".

## 4. Cách chạy
Mở file index.html bằng trình duyệt.

Xem trực tiếp: https://duongvu31241024842.github.io/ecommerce-ui-improvement/

Cấu trúc thư mục:

```
ecommerce-ui-improvement/
├── index.html
├── css/
│   └── style.css
├── images/
│   └── ca-phe-1.svg ... ca-phe-4.svg
├── README.md
└── AI_USAGE.md
```

## 5. Những thay đổi đã thực hiện

**Buổi 1**
- Thiết kế lại thẻ sản phẩm: ảnh ở trên, nhãn loại hạt trên ảnh, bên dưới là tên, mức rang (có chấm màu), tag cách pha, giá và nút mua.
- Thêm cách hiển thị giá khuyến mãi: giá mới, giá gốc gạch ngang, nhãn giảm giá.
- Tên sản phẩm 4 ban đầu lặp lại thông tin đã có ở nhãn loại hạt, mức rang và tag cách pha, nên được rút gọn thành "Cà phê Cầu Đất 250g".

**Buổi 2**
- Thêm `<nav>` với ba liên kết ở đầu trang, căn giữa bằng Flexbox.
- Thêm liên kết "Xem chi tiết" ở mỗi thẻ, định dạng thành nút bằng descendant selector, `padding`, `border`, `border-radius`; xếp cùng nút "Thêm vào giỏ" bằng Flexbox và `gap`.
- Gom giá gốc vào thẻ `del`, thêm `aria-label` riêng cho từng liên kết "Xem chi tiết", cho liên kết "Sản phẩm" trỏ tới khu vực sản phẩm.
- Giá thường dùng màu chữ bình thường, chỉ giá khuyến mãi màu đỏ để giá giảm nổi bật.
- Thêm hiệu ứng `:hover`, `:focus-visible`, `:active` cho nút; đổi màu hover sang cam đậm hơn để chữ dễ đọc.
- Tự phát hiện và sửa hai vấn đề: nhãn giảm giá và giá khuyến mãi mất màu đỏ do thiếu biến `--color-sale` trong `:root`; nhãn cách pha bị xuống dòng ở màn hình điện thoại 375px.

## 6. Công cụ AI đã sử dụng và cách kiểm tra kết quả
Công cụ: Claude.

AI được dùng để phân tích mã hiện tại, kiểm tra cấu trúc HTML5, gợi ý CSS selector, Box Model, Flexbox, Grid, hiệu ứng hover/focus và tìm nguyên nhân lỗi. Tôi không dùng nguyên kết quả của AI: mỗi gợi ý được đối chiếu với trang chạy thật bằng Chrome DevTools ở độ rộng 1366px, 768px và 375px trước khi áp dụng. Một số gợi ý tôi bỏ hoặc điều chỉnh, ví dụ không đổi tên sản phẩm 4 theo gợi ý của AI và không thêm chữ dẫn "Phù hợp pha:" vì làm khung thẻ chật hơn. Prompt chi tiết và phần kiểm tra xem trong file AI_USAGE.md.

## 7. Đường dẫn
- GitHub repository: https://github.com/duongvu31241024842/ecommerce-ui-improvement
- GitHub Pages: https://duongvu31241024842.github.io/ecommerce-ui-improvement/

## 8. Báo cáo kiểm thử

| Nội dung kiểm tra | Kết quả | Ghi chú |
|---|---|---|
| Trang HTML mở được | Đạt | Hiển thị đủ menu, tiêu đề và 4 thẻ sản phẩm |
| CSS được áp dụng | Đạt | Đường dẫn `css/style.css` đúng; đã sửa lỗi thiếu biến `--color-sale` |
| Hình ảnh hiển thị đúng | Đạt | 4 ảnh SVG nằm trọn trong khung, không méo |
| Liên kết hoạt động | Đạt có ghi chú | Liên kết "Sản phẩm" cuộn tới khu vực sản phẩm; các liên kết còn lại dùng `href="#"` vì chưa có trang đích |
| Bố cục không bị tràn nghiêm trọng | Đạt | 1366px: 4 cột; 768px: 3 cột; 375px: 2 cột, không có thanh cuộn ngang |
| Hover/focus hoạt động | Đạt | Rê chuột đổi màu mượt, phím Tab hiện viền focus, nhấn giữ nút thu nhỏ nhẹ |
| Đã tự sửa ít nhất một vấn đề | Đạt | Sửa 2 vấn đề: thiếu biến `--color-sale`; nhãn cách pha xuống dòng ở 375px |
