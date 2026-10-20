# AI Usage Log

## 1. Công cụ AI
Tên công cụ: Claude

## 2. Mục đích sử dụng
- Phân tích 5 khu vực của website Phương Vy Coffee (trang chủ, danh mục, chi tiết sản phẩm, tìm kiếm, giỏ hàng).
- Đề xuất phương án thiết kế và bố cục thẻ sản phẩm.
- Tạo mã HTML/CSS ban đầu.
- Gợi ý các điểm có thể cải thiện trong mã nguồn.

## 3. Prompt đã sử dụng
**Prompt 1 – Phân tích website:**
> Bạn là chuyên gia phân tích nghiệp vụ và thiết kế trải nghiệm người dùng cho website thương mại điện tử. Tôi đang khảo sát website: Phương Vy Coffee – https://phuongvycoffee.com. Hãy giúp tôi lập bảng phân tích các khu vực: trang chủ, danh mục sản phẩm, chi tiết sản phẩm, tìm kiếm, giỏ hàng. Với mỗi khu vực, hãy nêu: mục đích của chức năng; thành phần giao diện cần có; điểm thuận tiện đối với khách hàng; một vấn đề có thể phát sinh; một đề xuất cải tiến. Không khẳng định những tính năng chưa được kiểm chứng. Phân biệt rõ nhận xét dựa trên quan sát và đề xuất của AI.

**Prompt 2 – Đề xuất giao diện:**
> Tôi đang thực hiện bài tập phát triển giao diện website thương mại điện tử bằng HTML5 và CSS3. Tôi muốn cải tiến khu vực: thẻ sản phẩm ở trang danh mục của website bán cà phê, hiển thị thêm nhãn loại cà phê, mức rang, cách pha phù hợp, giá và nút mua. Đối tượng sử dụng: khách hàng mua sắm trực tuyến tại Việt Nam. Hãy đề xuất: bố cục giao diện, các thành phần HTML cần sử dụng, cách tổ chức CSS, cách hiển thị trên máy tính và điện thoại, những điểm cần kiểm tra về khả năng sử dụng. Trước tiên, hãy giải thích phương án thiết kế. Chưa tạo toàn bộ mã nguồn cho đến khi tôi yêu cầu.

**Prompt 3 – Tạo mã nguồn:**
> Dựa trên phương án đã thống nhất, hãy tạo một trang giao diện thương mại điện tử bằng HTML5 và CSS3. Yêu cầu: giao diện có tiêu đề và khu vực sản phẩm; có tối thiểu 4 sản phẩm mẫu; mỗi sản phẩm có hình ảnh, tên, giá và nút thao tác; bố cục phù hợp với màn hình máy tính và điện thoại; mã HTML có cấu trúc rõ ràng; CSS được tách thành file riêng; không sử dụng backend hoặc cơ sở dữ liệu; không đưa thư viện hoặc thành phần không cần thiết vào dự án. Giải thích cách chạy trang web và những phần tôi cần kiểm tra.

## 4. Kết quả AI đề xuất
- Bảng phân tích 5 khu vực, mỗi nhận xét được gắn nhãn là quan sát hay đề xuất của AI.
- Phương án thẻ sản phẩm: ảnh ở trên, nhãn loại hạt trên ảnh, bên dưới là tên, mức rang, cách pha, giá và nút mua. Lưới 4/3/2 cột theo kích thước màn hình.
- Mã nguồn gồm index.html, css/style.css và 4 ảnh minh họa dạng SVG trong thư mục images/.

## 5. Kiểm tra và điều chỉnh
- Đối chiếu bảng phân tích của AI với website thật. AI không mở được trang tìm kiếm và giỏ hàng nên tôi tự thử: tìm "espresso", "pha máy" không gợi ý sản phẩm phù hợp; giỏ hàng bắt nhập địa chỉ thủ công; trang danh mục có sắp xếp theo giá nhưng không có bộ lọc sản phẩm. Tôi loại các nhận xét chưa có bằng chứng và sửa theo kết quả thật.
- Mở trang bằng Chrome, dùng DevTools kiểm tra ở kích thước máy tính, 768px và 375px.
- Tự chỉnh sửa: tên sản phẩm 4 lặp lại thông tin đã có ở nhãn loại hạt, mức rang và cách pha, nên tôi rút gọn thành "Cà phê Cầu Đất 250g".
- Không sử dụng ảnh của website tham khảo vì lý do bản quyền, dùng ảnh minh họa tự vẽ.

## 6. Phần tôi hiểu và có thể giải thích
- `<article class="product-card">`: mỗi sản phẩm là một thẻ độc lập, trong đó `<h2>` là tên, `<ul>` là các tag cách pha, `<button>` là nút mua.
- `:root` và biến màu (`--color-primary`, `--color-accent`...): lưu màu một chỗ để đổi cả trang.
- `display: grid` ở `.product-grid` và `grid-template-columns`: tạo lưới thẻ 4 cột, đổi thành 3 và 2 cột bằng `@media`.
- `display: flex` với `flex-direction: column` trong thẻ, kết hợp `margin-top: auto` ở `.product-footer`: đẩy phần giá và nút xuống đáy thẻ để các thẻ đều nhau.
- `-webkit-line-clamp: 2` ở `.product-name`: cắt tên dài ở 2 dòng, giúp chiều cao các thẻ gần như nhau.
- `@media (max-width: ...)`: đổi số cột và cỡ chữ theo kích thước màn hình.
