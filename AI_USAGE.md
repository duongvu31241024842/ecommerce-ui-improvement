# AI Usage Log

## 1. Công cụ AI
Tên công cụ: Claude

## 2. Mục đích sử dụng
**Buổi 1**
- Phân tích 5 khu vực của website Phương Vy Coffee (trang chủ, danh mục, chi tiết sản phẩm, tìm kiếm, giỏ hàng).
- Đề xuất phương án thiết kế và bố cục thẻ sản phẩm.
- Tạo mã HTML/CSS ban đầu.

**Buổi 2**
- Phân tích mã nguồn hiện tại và kiểm tra cấu trúc HTML5.
- Hỗ trợ thực hành CSS selector, Box Model, Flexbox, CSS Grid, hover/focus.
- Tìm nguyên nhân lỗi hiển thị và gợi ý cấu trúc README.

## 3. Prompt đã sử dụng

### Buổi 1
**Prompt 1 – Phân tích website:**
> Bạn là chuyên gia phân tích nghiệp vụ và thiết kế trải nghiệm người dùng cho website thương mại điện tử. Tôi đang khảo sát website: Phương Vy Coffee – https://phuongvycoffee.com. Hãy giúp tôi lập bảng phân tích các khu vực: trang chủ, danh mục sản phẩm, chi tiết sản phẩm, tìm kiếm, giỏ hàng. Với mỗi khu vực, hãy nêu: mục đích của chức năng; thành phần giao diện cần có; điểm thuận tiện đối với khách hàng; một vấn đề có thể phát sinh; một đề xuất cải tiến. Không khẳng định những tính năng chưa được kiểm chứng. Phân biệt rõ nhận xét dựa trên quan sát và đề xuất của AI.

**Prompt 2 – Đề xuất giao diện:**
> Tôi đang thực hiện bài tập phát triển giao diện website thương mại điện tử bằng HTML5 và CSS3. Tôi muốn cải tiến khu vực: thẻ sản phẩm ở trang danh mục của website bán cà phê, hiển thị thêm nhãn loại cà phê, mức rang, cách pha phù hợp, giá và nút mua. Đối tượng sử dụng: khách hàng mua sắm trực tuyến tại Việt Nam. Hãy đề xuất: bố cục giao diện, các thành phần HTML cần sử dụng, cách tổ chức CSS, cách hiển thị trên máy tính và điện thoại, những điểm cần kiểm tra về khả năng sử dụng. Trước tiên, hãy giải thích phương án thiết kế. Chưa tạo toàn bộ mã nguồn cho đến khi tôi yêu cầu.

**Prompt 3 – Tạo mã nguồn:**
> Dựa trên phương án đã thống nhất, hãy tạo một trang giao diện thương mại điện tử bằng HTML5 và CSS3. Yêu cầu: giao diện có tiêu đề và khu vực sản phẩm; có tối thiểu 4 sản phẩm mẫu; mỗi sản phẩm có hình ảnh, tên, giá và nút thao tác; bố cục phù hợp với màn hình máy tính và điện thoại; mã HTML có cấu trúc rõ ràng; CSS được tách thành file riêng; không sử dụng backend hoặc cơ sở dữ liệu; không đưa thư viện hoặc thành phần không cần thiết vào dự án. Giải thích cách chạy trang web và những phần tôi cần kiểm tra.

### Buổi 2
Các prompt dưới đây theo mẫu của đề bài, với phần `[Dán mã ...]` được thay bằng mã `index.html` và `css/style.css` thật của tôi.

- **Prompt 1 – Phân tích mã hiện tại:** nhờ AI xác định thành phần HTML đã có, phần còn thiếu hoặc chưa hợp lý, ba vấn đề về cấu trúc và trình bày, cách cải thiện và thứ tự thực hiện; yêu cầu chưa viết lại toàn bộ mã.
- **Prompt 2 – Kiểm tra cấu trúc HTML5:** nhờ AI kiểm tra `header`, `nav`, `main`, `section`, `article`, `footer`, thứ bậc tiêu đề, `img`/`alt`/`a`, thẻ chưa đóng hoặc lồng sai; yêu cầu phân biệt lỗi cần sửa và đề xuất cải thiện.
- **Prompt 3 – Tạo CSS cơ bản:** nhờ AI hướng dẫn liên kết `css/style.css`, định dạng font, màu, `margin` cho `body`, ảnh không vượt khung, kiểm tra đường dẫn CSS.
- **Prompt 4 – Selector và Box Model:** nhờ AI hướng dẫn element, class, descendant selector, `margin`, `padding`, `border`, `border-radius` trên thẻ sản phẩm và giải thích `box-sizing: border-box`.
- **Prompt 5 – Flexbox:** nhờ AI hướng dẫn `display: flex`, `justify-content`, `align-items`, `gap` cho menu và nhóm nút.
- **Prompt 6 – CSS Grid:** nhờ AI hướng dẫn `grid-template-columns`, `repeat`, `gap`, giữ tỉ lệ ảnh và `object-fit: cover` cho danh sách sản phẩm.
- **Prompt 7 – Hover và focus:** nhờ AI hướng dẫn `:hover`, `transition`, `:focus-visible`, độ tương phản màu, giữ bố cục không đổi.
- **Prompt 8 – Kiểm tra lỗi:** mô tả lỗi nhãn "-15%" mất nền đỏ và giá khuyến mãi hiển thị màu đen; nhờ AI xác định nguyên nhân đã xác định và giả thuyết cần kiểm tra, đề xuất cách sửa ít thay đổi nhất.
- **Prompt 9 – README:** nhờ AI đề xuất cấu trúc README 7 mục, không tự bịa thông tin dự án.

## 4. Kết quả AI đề xuất

**Buổi 1**
- Bảng phân tích 5 khu vực, mỗi nhận xét được gắn nhãn là quan sát hay đề xuất của AI.
- Phương án thẻ sản phẩm: ảnh ở trên, nhãn loại hạt trên ảnh, bên dưới là tên, mức rang, cách pha, giá và nút mua. Lưới 4/3/2 cột theo kích thước màn hình.
- Mã nguồn gồm index.html, css/style.css và 4 ảnh minh họa dạng SVG trong thư mục images/.

**Buổi 2**
- Phân tích mã: thiếu `<nav>` và liên kết `<a>`, giá thường cùng màu đỏ với giá khuyến mãi, nút chưa có `:active`, màu cam chưa đủ tương phản, bốn liên kết "Xem chi tiết" giống hệt nhau, giá gốc dùng `span` thay vì `del`.
- Kiểm tra HTML: cấu trúc đóng và lồng thẻ đúng, thứ bậc `h1` → `h2` hợp lý; đề xuất `aria-label`, `del`, `id` cho khu vực sản phẩm, căn lại thụt lề.
- CSS: biến màu ở `:root`, `box-sizing`, element, class và descendant selector, Flexbox cho menu và nhóm nút, Grid cho lưới sản phẩm, `:hover`, `:focus-visible`, `:active`.
- Lỗi hiển thị: khối `:root` thiếu biến `--color-sale`; cách sửa là thêm lại một dòng khai báo.

## 5. Kiểm tra và điều chỉnh

**Buổi 1**
- Đối chiếu bảng phân tích của AI với website thật. AI không mở được trang tìm kiếm và giỏ hàng nên tôi tự thử: tìm "espresso", "pha máy" không gợi ý sản phẩm phù hợp; giỏ hàng bắt nhập địa chỉ thủ công; trang danh mục có sắp xếp theo giá nhưng không có bộ lọc sản phẩm. Tôi loại các nhận xét chưa có bằng chứng và sửa theo kết quả thật.
- Mở trang bằng Chrome, dùng DevTools kiểm tra ở kích thước máy tính, 768px và 375px.
- Tự chỉnh sửa: tên sản phẩm 4 lặp lại thông tin đã có ở nhãn loại hạt, mức rang và cách pha, nên tôi rút gọn thành "Cà phê Cầu Đất 250g".
- Không sử dụng ảnh của website tham khảo vì lý do bản quyền, dùng ảnh minh họa tự vẽ.

**Buổi 2**
- Đối chiếu từng nhận xét của AI với trang chạy thật và ảnh chụp ở 1366px, 768px, 375px trước khi sửa mã.
- **Đã dùng:** thêm `<nav>` và `<a>`; `aria-label` cho liên kết "Xem chi tiết"; `del` cho giá gốc; `id` cho khu vực sản phẩm; giá thường dùng màu chữ bình thường; `:hover`, `:focus-visible`, `:active`; màu cam đậm hơn cho hover và focus; Flexbox cho menu và nhóm nút; thêm biến `--color-sale` bị thiếu.
- **Không dùng hoặc điều chỉnh:**
  - Không đổi tên sản phẩm 4 thành "Arabica Cầu Đất 250g" vì chữ "Arabica" đã có ở nhãn loại hạt, mỗi thông tin chỉ nên xuất hiện một lần.
  - Không thêm chữ dẫn "Phù hợp pha:" vì làm khung thẻ chật hơn.
  - Không đặt `margin` và `padding` cho `.product-card`, vì khoảng cách giữa các thẻ đã do `gap` của lưới đảm nhận.
  - Dùng `display: block` thay vì `inline-block` cho nút "Xem chi tiết" để rộng bằng nút bên dưới.
  - Dùng `justify-content: center` thay vì `space-between` cho menu để đồng bộ với tiêu đề căn giữa.
  - Giữ tỉ lệ ảnh `4 / 3` thay vì `1 / 1` để thẻ gọn hơn; dùng lưới 4/3/2 cột thay vì cố định 2 cột.
  - Chưa thêm `<meta name="description">`, `width`/`height` cho ảnh, `minmax(0, 1fr)`, vì chưa cần cho phạm vi bài.
- **Tự phát hiện và tự sửa:**
  - Nhãn giảm giá và giá khuyến mãi mất màu đỏ do thiếu biến `--color-sale` trong `:root`; AI giúp làm rõ nguyên nhân, tôi mở `:root` kiểm tra, thêm lại biến và tải lại trang để xác nhận.
  - Nhãn cách pha bị xuống dòng ở màn hình 375px; tôi tự giảm cỡ chữ, khoảng đệm và khoảng cách của nhãn trong `@media (max-width: 600px)`.
  - Dòng `<h2>` của sản phẩm 4 thụt lề lệch trong `index.html`; tôi căn lại cho thẳng hàng.

## 6. Phần tôi hiểu và có thể giải thích
- `<nav>`: khung chứa các liên kết điều hướng chính; khác `<div>` ở chỗ trình duyệt và trình đọc màn hình hiểu đây là menu.
- `<article class="product-card">`: mỗi sản phẩm là một khối nội dung độc lập; `<h2>` là tên, `<ul>` là các tag cách pha, `<del>` là giá gốc, `<button>` là nút mua.
- `<img>` và `alt`: `alt` hiển thị thay ảnh khi ảnh lỗi và được trình đọc màn hình đọc lên.
- `:root` và biến màu (`--color-primary`, `--color-accent`, `--color-sale`...): lưu màu một chỗ, các quy tắc khác dùng `var(...)`; thiếu một biến thì các chỗ dùng nó mất màu, như lỗi nhãn giảm giá.
- Selector: `a` (element), `.price` (class), `.product-card .btn-detail` (descendant, chỉ áp dụng cho liên kết nằm trong thẻ sản phẩm).
- `margin` là khoảng trống bên ngoài, `padding` là khoảng trống bên trong; `box-sizing: border-box` làm `width` bao gồm cả padding và border.
- `display: flex` đặt trên phần tử cha; `justify-content` căn theo trục chính, `align-items` căn theo trục phụ, `gap` tạo khoảng cách giữa các phần tử.
- `display: grid` ở `.product-grid` với `grid-template-columns: repeat(4, 1fr)` và `gap`; `@media` đổi thành 3 và 2 cột; `object-fit: cover` giữ ảnh phủ kín khung không méo.
- `-webkit-line-clamp: 2` ở `.product-name`: cắt tên dài ở 2 dòng, giúp chiều cao các thẻ gần như nhau.
- `:hover` (rê chuột), `:focus-visible` (chọn bằng bàn phím), `:active` (đang nhấn) và `transition` làm màu đổi mượt.
