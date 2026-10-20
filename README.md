# E-commerce UI Improvement

## 1. Giới thiệu
Bài tập cải tiến giao diện thẻ sản phẩm ở trang danh mục của website bán cà phê. Thẻ sản phẩm mới hiển thị rõ hình ảnh, tên, loại hạt, mức rang, cách pha phù hợp, giá và nút mua, để khách dễ so sánh các sản phẩm.

## 2. Website tham khảo
- Tên website: Phương Vy Coffee
- URL: https://phuongvycoffee.com
- Khu vực đã khảo sát: trang chủ, danh mục sản phẩm, chi tiết sản phẩm, tìm kiếm, giỏ hàng. Khu vực được cải tiến: thẻ sản phẩm ở trang danh mục.

## 3. Chức năng
- Hiển thị danh sách 4 sản phẩm mẫu dạng lưới thẻ.
- Hiển thị hình ảnh, tên, loại hạt (Arabica/Robusta/Blend), mức rang và cách pha phù hợp.
- Hiển thị giá, giá khuyến mãi kèm giá gốc gạch ngang và nhãn giảm giá.
- Nút "Thêm vào giỏ" (chỉ là giao diện, chưa có xử lý).
- Bố cục hỗ trợ nhiều kích thước màn hình: 4 cột trên máy tính, 3 cột trên máy tính bảng, 2 cột trên điện thoại.

## 4. Công nghệ
- HTML5
- CSS3

## 5. Cách chạy
Mở file index.html bằng trình duyệt.

## 6. Cải tiến đã thực hiện
**Vấn đề ban đầu:** thẻ sản phẩm trên website tham khảo chỉ có ảnh, tên và một mức giá, nên khách khó biết loại hạt, mức rang hay cách pha phù hợp nếu không đọc kỹ tên hoặc mở từng trang. Dòng khuyến mãi lặp lại ở mọi thẻ cũng làm thẻ rối.

**Thay đổi đã thực hiện:**
- Thiết kế lại thẻ: ảnh ở trên, nhãn loại hạt trên ảnh, bên dưới là tên, mức rang (có chấm màu), tag cách pha, giá và nút mua.
- Thêm cách hiển thị giá khuyến mãi (giá mới, giá gốc gạch ngang, nhãn giảm giá).
- Tự chỉnh sửa: tên sản phẩm 4 ban đầu là "Arabica rang nhạt dùng cho cold brew 250g", lặp lại thông tin đã có ở nhãn loại hạt, mức rang và tag cách pha. Tôi rút gọn thành "Cà phê Cầu Đất 250g" để mỗi thông tin chỉ xuất hiện một lần, thẻ gọn hơn và dễ so sánh hơn.

## 7. Hỗ trợ từ AI
AI (Claude) hỗ trợ phân tích 5 khu vực của website tham khảo, đề xuất phương án thiết kế thẻ sản phẩm và tạo mã HTML/CSS ban đầu. Tôi đối chiếu nhận xét của AI với website thật, tự thử tìm kiếm và giỏ hàng, kiểm tra giao diện ở nhiều kích thước bằng Chrome DevTools và tự chỉnh sửa tên sản phẩm. Chi tiết xem trong file AI_USAGE.md.
