# BỘ PROMPT GOOGLE STITCH THIẾT KẾ GIAO DIỆN LMS (MINI-UDEMY)
**Đề tài:** Xây dựng Website Quản lý Học tập Trực tuyến (Learning Management System)  
**Quy chuẩn khung:** Kế thừa chuẩn 5 Layer từ `khung_prompt_stitch_google_uxui_lms.md`  
**Công nghệ đích:** Laravel Framework & Cơ sở dữ liệu MySQL 22 bảng đã chuẩn hóa  
**Mục đích:** Cung cấp đầy đủ 23 prompt độc lập, có thể sao chép trực tiếp vào **Google Stitch** để sinh artboard giao diện độ chính xác cao phục vụ báo cáo Giảng viên Hướng dẫn.

---

## MỤC LỤC BỘ PROMPT (23 MÀN HÌNH)

### I. PHÂN HỆ HỌC VIÊN & CÔNG CỘNG (STUDENT & PUBLIC - 10 MÀN HÌNH)
* [PROMPT 01 - SCR-STU-01: Trang chủ (Homepage / Landing Page)](#prompt-01---scr-stu-01-trang-chủ-homepage--landing-page)
* [PROMPT 02 - SCR-STU-02: Khám phá & Bộ lọc Khóa học (Search & Catalog)](#prompt-02---scr-stu-02-khám-phá--bộ-lọc-khóa-học-search--catalog)
* [PROMPT 03 - SCR-STU-03: Chi tiết Khóa học (Course Landing Page)](#prompt-03---scr-stu-03-chi-tiết-khóa-học-course-landing-page)
* [PROMPT 04 - SCR-STU-04: Giỏ hàng & Thanh toán (Checkout Page)](#prompt-04---scr-stu-04-giỏ-hàng--thanh-toán-checkout-page)
* [PROMPT 05 - SCR-STU-05: Thông báo Kết quả Thanh toán (Payment Status / IPN Result)](#prompt-05---scr-stu-05-thông-báo-kết-quả-thanh-toán-payment-status--ipn-result)
* [PROMPT 06 - SCR-STU-06: Bảng điều khiển Học tập (My Learning Dashboard)](#prompt-06---scr-stu-06-bảng-điều-khiển-học-tập-my-learning-dashboard)
* [PROMPT 07 - SCR-STU-07: Phòng học / Trình phát Bài giảng (Core Learning Player)](#prompt-07---scr-stu-07-phòng-học--trình-phát-bài-giảng-core-learning-player)
* [PROMPT 08 - SCR-STU-08: Làm bài kiểm tra Trắc nghiệm (Quiz Assessment)](#prompt-08---scr-stu-08-làm-bài-kiểm-tra-trắc-nghiệm-quiz-assessment)
* [PROMPT 09 - SCR-STU-09: Chứng chỉ Điện tử & Tra cứu QR (Certificate Verification)](#prompt-09---scr-stu-09-chứng-chỉ-điện-tử--tra-cứu-qr-certificate-verification)
* [PROMPT 10 - SCR-STU-10: Hồ sơ Cá nhân & Lịch sử Đơn hàng (Profile & Orders)](#prompt-10---scr-stu-10-hồ-sơ-cá-nhân--lịch-sử-đơn-hàng-profile--orders)

### II. PHÂN HỆ GIẢNG VIÊN (INSTRUCTOR BACKOFFICE - 6 MÀN HÌNH)
* [PROMPT 11 - SCR-INS-01: Bảng điều khiển Giảng viên (Instructor Dashboard)](#prompt-11---scr-ins-01-bảng-điều-khiển-giảng-viên-instructor-dashboard)
* [PROMPT 12 - SCR-INS-02: Thông tin Cơ bản & Định giá Khóa học (Course Info & Pricing)](#prompt-12---scr-ins-02-thông-tin-cơ-bản--định-giá-khóa-học-course-info--pricing)
* [PROMPT 13 - SCR-INS-03: Trình soạn thảo Giáo trình (Curriculum Builder)](#prompt-13---scr-ins-03-trình-soạn-thảo-giáo-trình-curriculum-builder)
* [PROMPT 14 - SCR-INS-04: Trình tạo Đề thi Trắc nghiệm (Quiz Builder)](#prompt-14---scr-ins-04-trình-tạo-đề-thi-trắc-nghiệm-quiz-builder)
* [PROMPT 15 - SCR-INS-05: Quản lý Hỏi đáp & Đánh giá (Q&A & Review Management)](#prompt-15---scr-ins-05-quản-lý-hỏi-đáp--đánh-giá-qa--review-management)
* [PROMPT 16 - SCR-INS-06: Ví Doanh thu & Yêu cầu Rút tiền (Wallet & Payout)](#prompt-16---scr-ins-06-ví-doanh-thu--yêu-cầu-rút-tiền-wallet--payout)

### III. PHÂN HỆ QUẢN TRỊ VIÊN (ADMIN PORTAL - 7 MÀN HÌNH)
* [PROMPT 17 - SCR-ADM-01: Báo cáo Tổng quan Toàn sàn (Admin Executive Dashboard)](#prompt-17---scr-adm-01-báo-cáo-tổng-quan-toàn-sàn-admin-executive-dashboard)
* [PROMPT 18 - SCR-ADM-02: Kiểm duyệt & Xuất bản Khóa học (Course Moderation & Preview)](#prompt-18---scr-adm-02-kiểm-duyệt--xuất-bản-khóa-học-course-moderation--preview)
* [PROMPT 19 - SCR-ADM-03: Quản lý Cây Danh mục Đào tạo (Category Management)](#prompt-19---scr-adm-03-quản-lý-cây-danh-mục-đào-tạo-category-management)
* [PROMPT 20 - SCR-ADM-04: Quản lý Mã giảm giá (Coupon Management)](#prompt-20---scr-adm-04-quản-lý-mã-giảm-giá-coupon-management)
* [PROMPT 21 - SCR-ADM-05: Quản trị Đơn hàng & Đối soát (Order & Audit Management)](#prompt-21---scr-adm-05-quản-trị-đơn-hàng--đối-soát-order--audit-management)
* [PROMPT 22 - SCR-ADM-06: Phê duyệt Yêu cầu Rút tiền (Payout Management)](#prompt-22---scr-adm-06-phê-duyệt-yêu-cầu-rút-tiền-payout-management)
* [PROMPT 23 - SCR-ADM-07: Quản trị Người dùng & Phân quyền (User & Access Control)](#prompt-23---scr-adm-07-quản-trị-người-dùng--phân-quyền-user--access-control)

---

## I. PHÂN HỆ HỌC VIÊN & CÔNG CỘNG (STUDENT & PUBLIC)

---

### PROMPT 01 - SCR-STU-01: Trang chủ (Homepage / Landing Page)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-STU-01: Trang chủ nền tảng LMS (Homepage / Public Landing)
- Role / User: Khách vãng lai (Guest) & Học viên (Student)
- Objective: Quảng bá nền tảng, cho phép tìm kiếm nhanh, khám phá danh mục đào tạo và hiển thị danh sách khóa học thịnh hành theo SRS F1.1 và F2.1.
- Theme/Style: Modern Clean EdTech SaaS, Canvas background #F8FAFC, Card #FFFFFF with border #E2E8F0, Primary Accent #4F46E5, Font Inter/Jakarta Sans, 8px border-radius.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px, Container Max-width 1280px, 12-column grid.
- Structure: Sticky Topbar (h=72px) + Hero Search Section + Category Carousel + Featured Courses Section (4 cols) + Career Learning Paths Banner + Footer.
- Visual Hierarchy: Mắt người dùng tập trung trước tiên vào Ô tìm kiếm nổi bật tại Hero Banner, sau đó quét qua lưới Khóa học thịnh hành có giá và số sao rating.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Header/Navigation:
  * Brand Logo "EduMaster LMS" bên trái.
  * Dropdown "Danh mục khóa học" trỏ dữ liệu cây `categories(name, slug)`.
  * Input Search bar to bản giữa header: Placeholder "Tìm kiếm bất kỳ khóa học, kỹ năng hoặc giảng viên...".
  * Bên phải: Nút Icon Giỏ hàng (kèm badge số lượng), Nút Outline "Đăng nhập", Nút Solid Primary `#4F46E5` "Đăng ký miễn phí".
- Hero Section:
  * Badge nhỏ: "🔥 Nền tảng học lập trình & công nghệ hàng đầu".
  * Tiêu đề lớn H1: "Học tập không giới hạn. Nâng tầm sự nghiệp công nghệ."
  * Sub-text: "Hơn 500+ khóa học thực chiến từ các chuyên gia đầu ngành. Học tuần tự, cấp chứng chỉ chuẩn quốc tế."
  * Stats counter: "120,000+ Học viên", "450+ Khóa học", "98% Hài lòng".
- Featured Categories:
  * Tiêu đề H2: "Khám phá danh mục nổi bật".
  * Lưới 6 cards danh mục (`categories.name`, `icon` SVG, số lượng khóa học): Lập trình Web, Mobile App, DevOps & Cloud, Khoa học Dữ liệu, UI/UX Design, Trí tuệ Nhân tạo.
- Trending Courses Section:
  * Tiêu đề H2 kèm Tab lọc nhanh (Tất cả, Mới nhất, Bán chạy nhất).
  * Lưới 4 cột Course Cards (Ánh xạ `courses`, `users`, `course_reviews`):
    - Thumbnail hình ảnh khóa học (`courses.thumbnail`).
    - Tag cấp độ màu xanh nhạt (`courses.level`: Beginner/All levels).
    - Tiêu đề khóa học (`courses.title`).
    - Tên giảng viên (`users.name`).
    - Đánh giá sao vàng Amber `#F59E0B` (VD: "4.9 ★ (1,240 đánh giá)").
    - Giá tiền: Giá bán thực tế (`courses.price`) in đậm to bản + Giá gốc gạch ngang (`courses.original_price`).
- Career Roadmaps Banner (Học tập F8):
  * Card nền gradient tím nhẹ: "Lộ trình học bài bản từ Zero đến Đi làm" (Front-end, Back-end Laravel).

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Default state có dữ liệu đầy đủ, hiển thị khóa học nổi bật.
- Realistic Dummy Data:
  * Khóa học 1: "Lập trình Backend chuyên nghiệp với Laravel 11", Giảng viên: "ThS. Nguyễn Văn Quang", Giá: "499,000 đ" (Giá gốc: "1,200,000 đ"), Rating: "4.9 ★ (850)".
  * Khóa học 2: "ReactJS & Next.js Toàn Tập Cho Người Mới", Giảng viên: "Trần Anh Tuấn", Giá: "0 đ" (Badge Miễn phí), Rating: "4.8 ★ (2,100)".
- Key Actions / CTAs: Nút "Đăng ký ngay" (Hero), Nút "Xem chi tiết khóa học" khi hover vào Card.

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Thẻ Course Card đổ bóng nhẹ `shadow-sm`, hover nhấc nhẹ 2px `shadow-md`.
- Badge "Miễn phí" dùng màu nền xanh ngọc `#D1FAE5` chữ `#065F46`.
- Không vẽ hiệu ứng hoạt họa phức tạp; tập trung đường nét thẻ sắc nét, chuẩn responsive desktop.
```

---

### PROMPT 02 - SCR-STU-02: Khám phá & Bộ lọc Khóa học (Search & Catalog)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-STU-02: Khám phá & Bộ lọc Khóa học (Search & Course Catalog)
- Role / User: Khách vãng lai & Học viên
- Objective: Cung cấp bộ lọc đa chiều (danh mục, cấp độ, giá, đánh giá) và sắp xếp kết quả tìm kiếm khóa học theo SRS F2.1.
- Theme/Style: Clean Modern SaaS, Nền canvas #F8FAFC, Khung lọc thẻ card trắng bo viền mỏng #E2E8F0, Accent #4F46E5.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px, Container 1280px.
- Structure: Sticky Topbar (h=72px) + Breadcrumb bar + Left Filter Sidebar (w=280px) + Main Catalog Grid (w=960px, 3 cột) + Pagination Footer.
- Visual Hierarchy: Bộ lọc bên trái cố định giúp người dùng định hình tiêu chí; lưới khóa học bên phải cập nhật tức thì tương ứng.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Topbar & Breadcrumb:
  * Breadcrumb: "Trang chủ / Danh mục / Lập trình Web".
- Left Filter Sidebar (w=280px, Card trắng bo tròn 12px, padding 20px):
  * Khối 1: Danh mục (`categories`): Checklist các danh mục cha con kèm số lượng (VD: "[x] Lập trình Laravel (24)").
  * Khối 2: Cấp độ (`courses.level`): Checkboxes [ ] Tất cả cấp độ, [x] Mới bắt đầu, [ ] Trung cấp, [ ] Nâng cao.
  * Khối 3: Mức giá (`courses.price`): Radio buttons: (o) Tất cả, ( ) Miễn phí (`price = 0`), ( ) Có phí (`price > 0`).
  * Khối 4: Đánh giá (`course_reviews`): Radio từ 4.5 sao trở lên, từ 4.0 sao trở lên.
  * Nút Text cuối sidebar: "Xóa toàn bộ bộ lọc" (Reset filter).
- Main Catalog Area (960px):
  * Header kết quả: Tiêu đề H2 "Khóa học Lập trình Web (Tìm thấy 38 khóa học)" + Dropdown Sắp xếp bên phải: "Mới nhất", "Đánh giá cao nhất", "Giá: Thấp đến cao".
  * Lưới Course Cards (3 cột, mỗi hàng 3 thẻ):
    - Thumbnail ảnh 16:9 (`courses.thumbnail`).
    - Badge cấp độ nhỏ góc ảnh (`courses.level`).
    - Tiêu đề khóa học 2 dòng (`courses.title`).
    - Giảng viên (`users.name`) kèm avatar nhỏ.
    - Điểm sao trung bình Amber `#F59E0B` + số lượng đánh giá.
    - Giá bán thực tế (`courses.price`) màu tím `#4F46E5` + Giá gạch ngang (`courses.original_price`).
  * Pagination: Bộ nút phân trang [1] [2] [3] ... [Trang tiếp].

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Default state có áp dụng bộ lọc "[x] Lập trình Laravel" và "[x] Mới bắt đầu".
- Realistic Dummy Data:
  * Card 1: "Xây dựng RESTful API chuyên nghiệp với Laravel 11", Giá: "599,000 đ", Giảng viên: "Nguyễn Văn Quang", Rating: "4.9 ★ (120)".
  * Card 2: "Laravel & Vue.js Fullstack Masterclass 2026", Giá: "799,000 đ", Giảng viên: "Lê Hoàng Long", Rating: "4.8 ★ (95)".
- Key Actions / CTAs: Click vào thẻ chuyển hướng sang `SCR-STU-03: Chi tiết khóa học`.

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Thẻ Card tỉ lệ cân đối, khoảng cách giữa các thẻ gap=24px.
- Checkbox trạng thái checked có màu nền tím `#4F46E5` có icon tích trắng.
```

---

### PROMPT 03 - SCR-STU-03: Chi tiết Khóa học (Course Landing Page)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-STU-03: Chi tiết Khóa học (Course Landing Page)
- Role / User: Khách vãng lai & Học viên
- Objective: Cung cấp thông tin giáo trình, video xem thử miễn phí, đánh giá xã hội và kích thích hành vi Mua khóa học theo SRS F2.2.
- Theme/Style: Modern EdTech, Hero Dark Theater `#0F172A`, Thân trang Canvas trắng `#FFFFFF`, Accent Button `#F59E0B` (Amber) và `#4F46E5`.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px.
- Structure: Sticky Topbar + Hero Dark Banner (h=320px) + 2 Cột nội dung (Cột trái 68% chi tiết + Cột phải 32% Sticky Purchase Box).
- Visual Hierarchy: Mắt người dùng bị hút vào Khối Sticky Mua hàng góc phải với Video Trailer và Nút CTA màu cam "Mua ngay".

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Hero Dark Banner (Nền `#0F172A`, chữ trắng):
  * Breadcrumb: "Trang chủ / Lập trình Web / Laravel".
  * Tiêu đề H1 lớn: "Xây dựng Hệ thống E-Commerce & LMS với Laravel 11 Chuyên Sâu" (`courses.title`).
  * Đoạn tóm tắt (`courses.summary`): "Làm chủ kiến trúc Clean Architecture, Repository Pattern, Cổng thanh toán VNPAY, Queue Jobs và bảo mật hệ thống."
  * Meta bar: Badge "Bán chạy nhất", Rating "4.9 ★ (420 đánh giá)", Số học viên "1,850 học viên", Tác giả: "Giảng viên: Nguyễn Văn Quang", Cập nhật lần cuối: "10/2026".
- Cột trái Main Content (68% layout, padding 32px):
  * Khung "Bạn sẽ học được gì?" (What you'll learn): Viền bo mỏng màu tím nhạt, 2 cột tích xanh gồm 6 mục tiêu đầu ra.
  * Khối "Nội dung khóa học" (Curriculum Accordion - Ánh xạ `chapters`, `lessons`, `lesson_videos`):
    - Thanh tóm tắt: "8 chương • 64 bài học • Tổng thời lượng 14 giờ 25 phút".
    - Accordion Chương 1: "Cài đặt & Kiến trúc Tổng quan (4 bài học - 45 phút)".
      * Bài 1: Video icon - "Giới thiệu kiến trúc hệ thống (10:15)" -> Badge xanh "Học thử" (`is_free_preview = TRUE`) có nút Preview mở modal video.
      * Bài 2: Video icon - "Cài đặt môi trường Docker & MySQL (15:20)".
      * Bài 3: Article icon - "Tài liệu Cheat-sheet câu lệnh Artisan".
  * Khối "Mô tả khóa học" (`courses.description` dạng Markdown render chuẩn đẹp).
  * Khối "Thông tin giảng viên" (`users`, `instructor_profiles`): Avatar tròn, Headline "Senior Backend Engineer tại TechCorp", Số khóa học, Bio tóm tắt.
  * Khối "Đánh giá từ học viên" (`course_reviews`): Điểm trung bình to 4.9/5, thanh tỷ lệ 5 sao (88%), danh sách nhận xét kèm ngày đánh giá và phản hồi của giảng viên.
- Cột phải Sticky Purchase Card (32%, ghim cố định khi scroll):
  * Khung Video Trailer (`courses.promo_video_url` có nút Play to ở giữa).
  * Giá bán (`courses.price`): "599,000 đ" (Font to 32px, bold), Giá gốc (`courses.original_price`): "1,499,000 đ" gạch ngang, Badge "-60% Giảm giá".
  * Nút CTA 1: "Mua ngay" (Button to, Full-width, Nền cam `#F59E0B`, chữ trắng, font-bold).
  * Nút CTA 2: "Thêm vào giỏ hàng" (Button Outline tím `#4F46E5`).
  * Danh sách quyền lợi kèm icon tích: "Truy cập trọn đời", "Học trên máy tính và điện thoại", "Cấp chứng chỉ tốt nghiệp điện tử", "Cam kết hoàn tiền trong 7 ngày".

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Default state dành cho khách chưa mua khóa học.
- Realistic Dummy Data: Khóa học "Xây dựng Hệ thống E-Commerce & LMS với Laravel 11", Giá "599,000 đ".
- Key Actions / CTAs: Nút "Mua ngay" dẫn trực tiếp sang `SCR-STU-04: Checkout`.

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Sticky Box bên phải có bóng đổ nổi bật `shadow-lg`, bo góc `rounded-2xl`.
- Đảm bảo huy hiệu "Học thử" (Free Preview) có màu xanh lá nổi bật để gây chú ý.
```

---

### PROMPT 04 - SCR-STU-04: Giỏ hàng & Thanh toán (Checkout Page)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-STU-04: Giỏ hàng & Thanh toán (Checkout Page)
- Role / User: Học viên (Bắt buộc đăng nhập tài khoản)
- Objective: Xác thực thông tin đơn hàng, nhập mã khuyến mãi coupon và chọn cổng thanh toán ngân hàng VNPAY theo SRS F2.4, F2.5.
- Theme/Style: Clean Financial / SaaS, Nền canvas #F8FAFC, Card trắng viền #E2E8F0, Nút thanh toán VNPAY nổi bật.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px, Container 1100px (Centered form).
- Structure: Minimal Topbar (Logo + Khóa bảo mật SSL badge) + 2 Cột thanh toán (Cột trái 60% Đơn hàng & Cổng thanh toán + Cột phải 40% Tóm tắt chi phí).
- Visual Hierarchy: Người dùng kiểm tra thông tin khóa học bên trái và bấm xác nhận thanh toán ở thẻ tóm tắt chi phí bên phải.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Topbar tối giản:
  * Logo hệ thống, Dòng chữ "Thanh toán an toàn 256-bit SSL encryption" có icon ổ khóa xanh lá.
- Cột trái: Thông tin đơn & Phương thức thanh toán (60%):
  * Mục 1: Khóa học đăng ký mua (`order_items`, `courses`):
    - Thẻ khóa học tóm tắt: Thumbnail nhỏ (100x60px), Tiêu đề khóa học, Tên tác giả, Giá gốc và Giá bán.
  * Mục 2: Chọn phương thức thanh toán (`orders.payment_method`):
    - Option 1 (Selected): Card radio chọn "Cổng thanh toán VNPAY (Quét mã VNPAY-QR / Thẻ ATM / Internet Banking)" kèm logo VNPAY chuẩn.
    - Option 2: Card radio chọn "Ví điện tử MoMo" kèm logo MoMo.
- Cột phải: Tóm tắt đơn hàng & Áp mã giảm giá (`orders`, `coupons`):
  * Card tóm tắt chi phí (Sticky Card):
    - Dòng "Giá gốc": "1,499,000 đ" (`orders.total_amount`).
    - Ô nhập mã giảm giá (`coupons.code`): Input text "Nhập mã khuyến mãi" + Nút "Áp dụng" màu tím.
    - Dòng "Giảm giá khuyến mãi": "-900,000 đ" (Khuyến mãi khóa học).
    - Dòng "Mã giảm giá (DISCOUNT100K)": "-100,000 đ" (Màu xanh lá có icon thẻ giảm giá).
    - Đường kẻ ngăn cách mảnh.
    - Dòng "Tổng thanh toán cuối cùng" (`orders.final_amount`): "499,000 đ" (In đậm to bản, cỡ chữ 28px, màu tím `#4F46E5`).
    - Nút CTA chính: "Tiến hành thanh toán qua VNPAY" (Full-width, h=52px, màu xanh thương hiệu VNPAY hoặc Primary `#4F46E5`, chữ trắng).
    - Ghi chú bảo mật: "Bằng việc hoàn tất thanh toán, bạn đồng ý với Điều khoản dịch vụ và Chính sách hoàn tiền 7 ngày của chúng tôi."

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: State đã áp dụng mã coupon `DISCOUNT100K` thành công.
- Realistic Dummy Data: Khóa học "Lập trình Laravel 11", Mã đơn dự kiến `ORD-20261105-8821`, Giá thực trả: "499,000 đ".
- Key Actions / CTAs: Nút "Tiến hành thanh toán qua VNPAY" kích hoạt chuyển hướng sang cổng thanh toán.

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Thẻ phương thức thanh toán có viền tím viền đôi khi ở trạng thái Active (Checked).
- Dòng chữ giảm giá hiển thị sắc nét bằng font số Tabular numbers (căn lề thẳng cột).
```

---

### PROMPT 05 - SCR-STU-05: Thông báo Kết quả Thanh toán (Payment Status / IPN Result)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-STU-05: Thông báo Kết quả Thanh toán (Payment Status / IPN Result)
- Role / User: Học viên
- Objective: Xác nhận trạng thái kích hoạt ghi danh thành công sau khi nhận Webhook IPN và điều hướng học viên vào phòng học theo SRS F2.6.
- Theme/Style: Clean Celebration Card, Nền canvas #F8FAFC, Card trắng căn giữa w=600px, Icon thành công màu xanh lục #10B981.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px.
- Structure: Topbar thông thường + Thẻ kết quả giao dịch đặt chính giữa màn hình (Center Modal Card w=600px).
- Visual Hierarchy: Icon tích xanh hoạt họa ở đỉnh thẻ, tiếp đến dòng thông báo "Thanh toán thành công" và nút CTA lớn "Bắt đầu học ngay".

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Center Result Card (Card trắng bo góc 16px, padding 40px, shadow-md):
  * Icon tròn lớn màu xanh lục `#10B981` có hình dấu tích trắng ở giữa.
  * Tiêu đề H2: "Thanh toán thành công!" (Màu xanh đậm `#065F46`).
  * Lời chúc mừng: "Chúc mừng bạn đã ghi danh thành công vào khóa học. Quyền truy cập trọn đời đã được kích hoạt."
  * Hộp chi tiết giao dịch (Nền xám nhạt `#F1F5F9`, bo góc 8px, padding 16px):
    - Dòng 1: "Mã đơn hàng:" `orders.order_code` (VD: `ORD-20261105-8821`).
    - Dòng 2: "Mã giao dịch ngân hàng:" `orders.transaction_id` (VD: `VNPAY14892011`).
    - Dòng 3: "Khóa học:" `courses.title` ("Lập trình Laravel 11 Chuyên Sâu").
    - Dòng 4: "Số tiền thanh toán:" `orders.final_amount` ("499,000 đ").
    - Dòng 5: "Thời gian giao dịch:" `orders.created_at` ("05/11/2026 21:15").
  * Nhóm nút hành động:
    - Nút CTA chính: "Bắt đầu học ngay" (Button to, Full-width, Nền tím `#4F46E5`, chữ trắng) dẫn vào `SCR-STU-07`.
    - Nút phụ: "Xem hóa đơn của tôi" (Button text dẫn về `SCR-STU-10`).
  * Dòng ghi chú nhỏ: "Biên lai thanh toán điện tử đã được gửi tự động tới email của bạn."

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Success State (Giao dịch hoàn tất thành công).
- Realistic Dummy Data: Mã đơn `ORD-20261105-8821`, Mã VNPAY `14892011`, Khóa học Laravel 11.
- Key Actions / CTAs: Nút "Bắt đầu học ngay" điều hướng thẳng vào phòng học bài đầu tiên.

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Thiết kế thẻ gọn gàng, tạo cảm giác an tâm và phấn khởi cho học viên sau khi chuyển tiền.
- Bố cục căn lề chính giữa tuyệt đối theo trục dọc và ngang.
```

---

### PROMPT 06 - SCR-STU-06: Bảng điều khiển Học tập (My Learning Dashboard)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-STU-06: Bảng điều khiển Học tập (My Learning Dashboard)
- Role / User: Học viên đã đăng nhập
- Objective: Quản lý danh mục các khóa học đã mua, theo dõi tỷ lệ phần trăm tiến độ và tiếp tục học bài dở dang theo SRS F4.1.
- Theme/Style: Modern Student Portal, Nền canvas #F8FAFC, Card trắng viền bo tròn 12px, Thanh tiến độ màu tím #4F46E5.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px, Container 1280px.
- Structure: Topbar có Avatar người dùng + Tiêu đề trang + Tabs lọc khóa học + Lưới Khóa học sở hữu (3 cột).
- Visual Hierarchy: Mắt học viên quét qua thanh tiến độ % của các khóa học đang theo học để chọn tiếp tục học.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Page Header:
  * Tiêu đề H1: "Khóa học của tôi".
  * Sub-text: "Theo dõi tiến độ học tập và duy trì thói quen học mỗi ngày."
  * Thanh Tabs lọc trạng thái: Tab "[Tất cả (3)]", Tab "[Đang học (2)]", Tab "[Đã hoàn thành (1)]".
- Lưới khóa học cá nhân (3 cột, ánh xạ `enrollments`, `courses`, `lesson_progress`):
  * Thẻ Khóa học 1 (Đang học dở):
    - Thumbnail ảnh (`courses.thumbnail`).
    - Tiêu đề khóa học: "Xây dựng RESTful API với Laravel 11".
    - Tên giảng viên: "Nguyễn Văn Quang".
    - Thanh Progress Bar: Nền xám nhạt, thanh chạy màu tím `#4F46E5` thể hiện 65%.
    - Dòng chỉ số tiến độ: "18 / 28 bài học (65%)".
    - Nút CTA: "Tiếp tục học" (Nền tím `#4F46E5`, chữ trắng) dẫn tới vị trí giây phát dừng lần trước (`last_watch_second`).
  * Thẻ Khóa học 2 (Đã hoàn thành 100%):
    - Tiêu đề: "HTML5, CSS3 & JavaScript Cơ Bản Cho Người Mới".
    - Thanh Progress Bar: 100% màu xanh lá `#10B981`.
    - Dòng chỉ số: "40 / 40 bài học (Hoàn thành)".
    - Nút CTA: "Xem & Tải chứng chỉ" (Nút nền vàng Amber `#F59E0B` có icon Cúp vàng) dẫn sang `SCR-STU-09`.
- Widget nhỏ bên phải (Gamification F8): Thẻ chuỗi ngày học liên tục (Streak: 🔥 5 ngày liên tiếp).

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Default state có 3 khóa học trong danh sách.
- Realistic Dummy Data: Khóa học Laravel 11 (65%), Khóa học ReactJS (20%), Khóa học Web cơ bản (100%).
- Key Actions / CTAs: Nút "Tiếp tục học" và "Xem chứng chỉ".

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Thanh Progress bar mỏng 8px bo tròn 2 đầu mượt mà.
- Khoảng cách thẻ grid gap=24px, đổ bóng nhẹ.
```

---

### PROMPT 07 - SCR-STU-07: Phòng học / Trình phát Bài giảng (Core Learning Player)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-STU-07: Phòng học & Trình phát Bài giảng (Core Learning Player)
- Role / User: Học viên đang học khóa học
- Objective: Màn hình trung tâm của hệ thống cho phép xem video bài giảng, ghi nhớ vị trí dừng, mở khóa bài tuần tự, tạo ghi chú timestamp và hỏi đáp lồng nhau theo SRS F4.2, F4.3, F4.4, F4.7.
- Theme/Style: Dark Theater Focus Mode, Toàn màn hình Nền tối #0B0F19, Sidebar giáo trình nền #1E293B, Điểm nhấn tím #6366F1 và tích xanh #10B981.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px (Full Width Fluid Layout, không khoảng trắng thừa).
- Structure: Minimal Top Header (h=56px) + Cột trái Workspace xem video & Tabs tương tác (75%) + Cột phải Sidebar Giáo trình tuần tự (25%).
- Visual Hierarchy: Khung video 16:9 sắc nét ở góc nhìn chính, tiếp đến là Sidebar danh sách bài học có icon tích xanh và ổ khóa thể hiện quy luật học tuần tự.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Top Minimal Header (Nền `#0B0F19`, viền dưới mỏng `#1E293B`):
  * Nút mũi tên "Quay lại Khóa học của tôi", Tiêu đề khóa học in nhỏ bên cạnh.
  * Tỷ lệ tiến độ tổng thể góc phải: "Tiến độ: 14/28 bài học (50%)".
- Cột trái Workspace (75% chiều rộng):
  * Khung Video Player HTML5 16:9 (`lesson_videos.video_url`):
    - Video đang phát với thanh điều khiển mờ khi hover: Nút Play/Pause, Thời lượng hiện tại / Tổng thời lượng `04:25 / 15:30`, Nút chọn tốc độ phát (1x, 1.25x, 1.5x), Nút phóng to toàn màn hình.
  * Dải thanh điều hướng ngay dưới Video:
    - Tiêu đề bài học lớn H2: "Bài 14: Xây dựng Middleware phân quyền trong Laravel" (`lessons.title`).
    - Nút "← Bài trước" (Màu xám).
    - Nút "Bài tiếp theo →" (Nút tím `#6366F1`, sáng rõ nếu bài hiện tại đã xem $\ge 80\%$, bị khóa mờ nếu chưa đủ điều kiện).
  * Khối Tabs đa chức năng phía dưới (Nền tối `#111827`, bo góc 12px, padding 20px):
    - **Tab 1: Ghi chú video (Timestamped Notes - Ánh xạ `lesson_notes`):**
      * Nút bấm "+ Tạo ghi chú tại 04:25" (Bấm vào tạm dừng video và mở ô nhập text).
      * Danh sách các ghi chú đã lưu: Thẻ ghi chú hiển thị Badge thời gian màu tím `[02:15]`, nội dung ghi chú "Cần chú ý cách cấu hình middleware trong bootstrap/app.php". Click vào badge `[02:15]` video tự động tua lại đúng giây 135.
    - **Tab 2: Hỏi & Đáp Q&A (Ánh xạ `lesson_comments`):**
      * Form nhập câu hỏi mới (hỗ trợ chèn code định dạng markdown).
      * Cây bình luận đa tầng: Bình luận của Học viên A -> Nút Trả lời -> Bình luận thụt dòng phản hồi của Giảng viên (kèm badge "Giảng viên").
    - **Tab 3: Tổng quan & Tài liệu tải về:** Tải file mã nguồn đính kèm `source-code-bai-14.zip`.
- Cột phải Sidebar Giáo trình tuần tự (25% chiều rộng, nền `#1E293B`, scroll độc lập):
  * Tiêu đề: "Nội dung khóa học".
  * Accordion Chương 1: "Kiến trúc cơ bản (5/5 hoàn thành)" -> Mở ra 5 bài đều có **Icon Tích xanh tròn `#10B981`** (`is_completed = TRUE`).
  * Accordion Chương 2: "Xử lý Request & Middleware (Đang học)":
    - Bài 13: Icon tích xanh lá (Đã xong).
    - Bài 14: **Icon Đang phát màu tím sáng (Active lesson)**.
    - Bài 15: **Icon Ổ khóa màu xám (Locked)** (`is_completed = FALSE`, không thể click).
    - Bài 16 (Quiz): Icon bài thi trắc nghiệm bị khóa.

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Đang phát Bài 14 tại phút 04:25, Tab Ghi chú đang mở hiển thị các ghi chú đã lưu.
- Realistic Dummy Data: Bài học Laravel Middleware, 2 ghi chú tại [01:10] và [04:25].
- Key Actions / CTAs: Nút "+ Tạo ghi chú tại [mốc thời gian]" và Nút "Bài tiếp theo".

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Thiết kế chuẩn Theater mode tương tự F8 / YouTube theater, các chi tiết sắc sảo, độ tương phản cao trên nền đen.
- Các icon ổ khóa và tích xanh phải phân biệt rõ rệt để giảng viên thấy rõ cơ chế "Sequential Learning Engine".
```

---

### PROMPT 08 - SCR-STU-08: Làm bài kiểm tra Trắc nghiệm (Quiz Assessment)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-STU-08: Làm bài kiểm tra Trắc nghiệm (Quiz Assessment)
- Role / User: Học viên
- Objective: Trình làm bài kiểm tra trắc nghiệm có đồng hồ đếm ngược, chấm điểm tự động và hiển thị giải thích đáp án theo SRS F4.5.
- Theme/Style: Focus Assessment UI, Nền canvas trắng xám #F8FAFC, Khung bài thi căn giữa w=860px bo góc #FFFFFF, Điểm nhấn tím #4F46E5.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px.
- Structure: Header bài thi (Tên bài quiz + Đồng hồ đếm ngược) + Vùng câu hỏi trắc nghiệm căn giữa + Thanh điều hướng câu hỏi bên dưới.
- Visual Hierarchy: Đồng hồ đếm ngược trên cùng gây chú ý về thời gian; câu hỏi và 4 lựa chọn trả lời dạng thẻ bấm to rõ ràng ở trung tâm.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Top Quiz Header (Card trắng bo góc 12px, h=64px, flex giữa):
  * Tên bài trắc nghiệm: "Bài kiểm tra cuối Chương 2: Kiến trúc MVC trong Laravel" (`quizzes`).
  * Thanh tiến độ câu hỏi: "Câu 4 / 10".
  * Đồng hồ đếm ngược: Badge đỏ cam có icon đồng hồ "⏱ 12:45" (Đếm lùi từ `quizzes.time_limit_minutes`).
- Main Question Area (Card trắng bo góc 16px, padding 32px, shadow-sm):
  * Tiêu đề câu hỏi (`quiz_questions.question_text`): "Trong Laravel 11, file cấu hình nào chịu trách nhiệm đăng ký Middleware toàn cục của ứng dụng?"
  * Danh sách 4 đáp án lựa chọn (`quiz_answers` dạng thẻ click chọn):
    - Lựa chọn A: Card viền mỏng "app/Http/Kernel.php"
    - Lựa chọn B (Selected): Card viền tím đậm, nền tím nhạt "bootstrap/app.php" (có radio button tím được chọn).
    - Lựa chọn C: Card viền mỏng "config/app.php"
    - Lựa chọn D: Card viền mỏng "routes/web.php"
- Footer Navigation:
  * Nút "← Câu trước" (Outline xám).
  * Nút "Câu tiếp theo →" (Primary tím).
  * Nút "Nộp bài thi" (Nút to góc phải, màu xanh ngọc `#10B981`, chữ trắng).
- Popup/Modal Kết quả thi (Khi nộp bài xong - Ánh xạ `quiz_submissions`):
  * Vòng tròn điểm số: "80%" (Đạt 8/10 câu).
  * Badge to: "CHÚC MỪNG - BẠN ĐÃ ĐẠT!" (Yêu cầu qua môn $\ge 80\%$).
  * Lời giải thích câu hỏi (`quiz_questions.explanation`): "Chính xác! Từ Laravel 11, file Kernel.php đã bị loại bỏ và gom cấu hình vào bootstrap/app.php."
  * Nút CTA: "Tiếp tục sang Bài học tiếp theo" (Mở khóa bài kế tiếp).

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Màn hình đang trả lời Câu hỏi số 4, lựa chọn B đang được chọn.
- Realistic Dummy Data: Đề thi 10 câu trắc nghiệm Laravel, thời gian còn lại 12 phút 45 giây.
- Key Actions / CTAs: Nút "Nộp bài thi".

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Thẻ đáp án có chiều cao tối thiểu 56px, chữ to rõ ràng, hover đổi màu nền nhạt tạo cảm giác tương tác tốt.
```

---

### PROMPT 09 - SCR-STU-09: Chứng chỉ Điện tử & Tra cứu QR (Certificate Verification)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-STU-09: Chứng chỉ Điện tử & Tra cứu Xác thực QR (Certificate View & Verify)
- Role / User: Học viên tốt nghiệp, Nhà tuyển dụng tra cứu công khai
- Objective: Cung cấp bản xem trước chứng chỉ hoàn thành khóa học 100% kèm mã QR tra cứu tính xác thực theo SRS F4.6.
- Theme/Style: Academic Formal / Premium EdTech, Nền xám trang trọng #F1F5F9, Khung chứng chỉ vàng ánh kim & xanh navy, Mã QR sắc nét.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px.
- Structure: Minimal Header + Khung Chứng chỉ mô phỏng PDF căn giữa (w=960px, tỉ lệ ngang A4) + Bảng điều khiển tải/chia sẻ bên dưới.
- Visual Hierarchy: Bản chứng chỉ sang trọng nằm chính giữa với tên học viên viết hoa nổi bật và con dấu đỏ bảo chứng.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Khung Chứng chỉ Tốt nghiệp (A4 Canvas 960x640px, Nền kem nhạt `#FDFAF6`, Viền đôi hoa văn cổ điển):
  * Logo sàn đào tạo: "EDUMASTER ACADEMY - CERTIFICATE OF COMPLETION".
  * Dòng vinh danh: "Chứng chỉ này chứng nhận học viên"
  * Tên học viên lớn H1 (Font Serif trang trọng): "NGUYỄN VĂN QUANG" (`users.name`).
  * Khóa học hoàn thành: "Đã hoàn thành xuất sắc khóa học chuyên sâu: Xây dựng Hệ thống E-Commerce & LMS với Laravel 11" (`courses.title`).
  * Dòng chi tiết: "Thời lượng: 14 giờ học • Điểm bài thi cuối khóa: 95% • Ngày cấp: 05/11/2026" (`certificates.issued_at`).
  * Con dấu mộc đỏ tròn bảo chứng góc trái + Chữ ký số Giám đốc đào tạo góc phải.
  * Góc dưới chính giữa: Mã chứng chỉ duy nhất (`certificates.certificate_code`: `UUID: 6d32c3ad-2b19-40fb-b5bc-c54eb80e46b5`) + Hình ảnh Mã QR Code xác thực.
- Bảng điều khiển hành động bên dưới (w=960px):
  * Badge xanh lá: "✓ ĐÃ XÁC THỰC HỢP LỆ TRÊN HỆ THỐNG".
  * Nút Primary: "Tải xuống bản PDF chính thức" (Nền tím `#4F46E5`, icon download) gọi thư viện Laravel DomPDF.
  * Nút Secondary: "Sao chép liên kết chứng chỉ" (Để đính kèm vào CV / LinkedIn).
  * Hướng dẫn: "Quét mã QR bằng camera điện thoại để mở trang xác thực độc lập."

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Default state hiển thị chứng chỉ hợp lệ của học viên Nguyễn Văn Quang.
- Realistic Dummy Data: Mã UUID `CERT-2026-LV11-0982`, Ngày cấp 05/11/2026.
- Key Actions / CTAs: Nút "Tải xuống bản PDF chính thức".

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Thiết kế chứng chỉ có hoa văn trang nhã, phông chữ có chân (Serif) kết hợp không chân (Sans) chuẩn văn bằng quốc tế.
```

---

### PROMPT 10 - SCR-STU-10: Hồ sơ Cá nhân & Lịch sử Đơn hàng (Profile & Orders)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-STU-10: Hồ sơ Cá nhân & Lịch sử Đơn hàng (Student Profile & Purchase History)
- Role / User: Học viên
- Objective: Cho phép cập nhật thông tin cá nhân, đổi mật khẩu và tra cứu lịch sử mua hàng đối soát theo SRS F1.3, F1.4, F2.7.
- Theme/Style: Clean Dashboard Settings, Nền canvas #F8FAFC, Card trắng bo góc 12px viền #E2E8F0, Accent #4F46E5.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px, Container 1100px.
- Structure: Topbar + 2 Cột (Cột trái 25% Menu điều hướng cài đặt + Cột phải 75% Nội dung Form cài đặt / Bảng đơn hàng).
- Visual Hierarchy: Tab Lịch sử đơn hàng có bảng dữ liệu kế toán rõ ràng kèm trạng thái đơn hàng.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Cột trái Menu Cài đặt (25%):
  * Avatar lớn học viên + Tên học viên (`users.name`) + Email (`users.email`).
  * Menu dọc:
    - [x] Thông tin cá nhân & Bảo mật (Active tab)
    - [ ] Lịch sử đơn hàng & Hóa đơn
  * Banner bên dưới: "Bạn muốn chia sẻ kiến thức?" -> Nút Outline "Đăng ký trở thành Giảng viên" (`F1.4`).
- Cột phải Nội dung (75%):
  * **Chế độ Tab 1: Cài đặt tài khoản (`users`):**
    - Vùng đổi ảnh đại diện (Upload avatar).
    - Form: Họ và tên (`name`), Email (Read-only), Số điện thoại.
    - Đổi mật khẩu: Ô nhập Mật khẩu hiện tại, Mật khẩu mới, Xác nhận mật khẩu mới.
    - Nút "Lưu thay đổi".
  * **Chế độ Tab 2: Lịch sử đơn hàng (`orders`, `order_items`, `coupons`):**
    - Bảng dữ liệu giao dịch:
      * Cột 1: Mã đơn hàng (`order_code`: `ORD-20261105-8821`).
      * Cột 2: Khóa học đã mua.
      * Cột 3: Ngày mua (`created_at`).
      * Cột 4: Số tiền thanh toán (`final_amount`: "499,000 đ") kèm tag mã coupon đã dùng nếu có.
      * Cột 5: Trạng thái badge: `Thành công` (Xanh lá `#10B981`).
      * Cột 6: Hành động: Nút icon "Xem biên lai PDF".

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Màn hình hiển thị Bảng Lịch sử đơn hàng với 2 đơn đã thanh toán thành công.
- Realistic Dummy Data: Học viên "Lê Văn Hùng", Đơn hàng `ORD-20261105-8821` trị giá 499,000 đ thanh toán qua VNPAY.
- Key Actions / CTAs: Nút "Xem biên lai" và Nút "Đăng ký làm Giảng viên".

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Bảng lịch sử có dòng xen kẽ màu (Zebra striping) nhẹ nhàng, chữ số tiền căn lề phải.
```

---

## II. PHÂN HỆ GIẢNG VIÊN (INSTRUCTOR BACKOFFICE)

---

### PROMPT 11 - SCR-INS-01: Bảng điều khiển Giảng viên (Instructor Dashboard)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-INS-01: Bảng điều khiển Giảng viên (Instructor Dashboard)
- Role / User: Giảng viên (`role = 'instructor'`)
- Objective: Thống kê số lượng học viên, doanh thu ví khả dụng và quản lý danh sách các khóa học của mình theo SRS F5.1, F5.3.
- Theme/Style: Professional Instructor Portal, Nền canvas #F8FAFC, Card trắng viền #E2E8F0, Accent #4F46E5.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px.
- Structure: Left Sidebar cố định (w=250px) + Topbar (h=64px) + Main Content (4 Stat Cards trên đỉnh + Bảng khóa học phía dưới).
- Visual Hierarchy: 4 thẻ thống kê KPI màu sắc rõ rệt trên cùng, theo sau là bảng danh sách khóa học kèm trạng thái duyệt.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Left Navigation Sidebar (w=250px, nền trắng viền phải `#E2E8F0`):
  * Logo hệ thống + Badge "Instructor Space".
  * Menu điều hướng:
    - [x] Tổng quan (Dashboard)
    - [ ] Khóa học của tôi
    - [ ] Quản lý Hỏi đáp (Q&A)
    - [ ] Đánh giá & Nhận xét
    - [ ] Doanh thu & Rút tiền
  * Nút chuyển nhanh "Góc nhìn học viên" ở góc đáy.
- Topbar: Tiêu đề "Bảng điều khiển Giảng viên" + Avatar giảng viên góc phải.
- Main Workspace:
  * Top Metric Cards (Lưới 4 cột KPI):
    - Thẻ 1: "Tổng doanh thu ví" (`instructor_profiles.wallet_balance`): "18,450,000 đ" (Icon ví tiền xanh lá).
    - Thẻ 2: "Tổng học viên": "1,420 học viên" (Icon nhóm người màu xanh dương).
    - Thẻ 3: "Đánh giá trung bình": "4.9 ★" (Icon ngôi sao vàng Amber).
    - Thẻ 4: "Khóa học xuất bản": "3 khóa học" (Icon sách màu tím).
  * Header Bảng Khóa học:
    - Tiêu đề H2: "Danh sách khóa học giảng dạy".
    - Nút CTA góc phải: "+ Tạo khóa học mới" (Nút tím `#4F46E5` chữ trắng) dẫn sang `SCR-INS-02`.
  * Bảng dữ liệu Khóa học (`courses`):
    - Cột 1: Khóa học (Thumbnail 60x40px + Tiêu đề).
    - Cột 2: Giá bán (`price`).
    - Cột 3: Số học viên (`enrollments` count).
    - Cột 4: Doanh thu tạo ra.
    - Cột 5: Trạng thái duyệt badge (`courses.status`):
      * `published`: Badge xanh lá "Đã xuất bản".
      * `pending`: Badge vàng cam "Chờ duyệt".
      * `draft`: Badge xám "Bản nháp".
    - Cột 6: Hành động: Nút "Soạn giáo trình" (dẫn sang `SCR-INS-03`), Nút icon sửa/xóa.

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Default state có 3 khóa học ở 3 trạng thái khác nhau (Published, Pending, Draft).
- Realistic Dummy Data: Giảng viên "Nguyễn Văn Quang", Số dư ví 18,450,000 đ.
- Key Actions / CTAs: Nút "+ Tạo khóa học mới".

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Badge trạng thái bo tròn dạng `rounded-full` kèm chấm tròn màu phía trước (`status dot`).
```

---

### PROMPT 12 - SCR-INS-02: Thông tin Cơ bản & Định giá Khóa học (Course Info & Pricing)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-INS-02: Thông tin Cơ bản & Định giá Khóa học (Course Info & Pricing)
- Role / User: Giảng viên
- Objective: Nhập liệu thông tin quảng bá khóa học, danh mục, cấp độ và cấu hình giá bán theo SRS F3.1.
- Theme/Style: Form Builder SaaS, Nền canvas #F8FAFC, Khung form trắng bo góc 12px, Stepper nav ở trên cùng.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px.
- Structure: Left Sidebar Instructor + Topbar + Thanh tiến trình 4 bước (Stepper) + Form nhập liệu chính (w=900px căn giữa).
- Visual Hierarchy: Thanh Stepper chỉ dẫn rõ người dùng đang ở Bước 1 "Thông tin cơ bản", các trường input có nhãn rõ ràng.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Stepper Header (4 bước):
  * [1. Thông tin cơ bản (Active)] ---> [2. Soạn giáo trình] ---> [3. Bài tập Quiz] ---> [4. Gửi phê duyệt].
- Form nhập liệu chính (Ánh xạ bảng `courses`):
  * Khối 1: Thông tin mô tả:
    - Tiêu đề khóa học (`courses.title`): Input text lớn "VD: Làm chủ Laravel 11 từ Zero đến Hero".
    - Tóm tắt ngắn (`courses.summary`): Textarea 3 dòng hiển thị ở thẻ ngoài danh mục.
    - Mô tả chi tiết (`courses.description`): Trình soạn thảo Rich-Text Editor có thanh công cụ (B, I, Code, List, Link).
  * Khối 2: Phân loại & Cấp độ:
    - Dropdown Danh mục (`courses.category_id`): Chọn từ cây danh mục "Lập trình Web > Laravel".
    - Dropdown Cấp độ (`courses.level`): Lựa chọn "Mọi cấp độ (All levels)".
  * Khối 3: Hình ảnh & Video giới thiệu:
    - Vùng tải ảnh bìa (`courses.thumbnail`): Khung kéo thả file (Hỗ trợ JPG/PNG, tỉ lệ 16:9, tối đa 2MB).
    - Ô nhập link Video trailer (`courses.promo_video_url`): Input link YouTube/Vimeo giới thiệu ngắn.
  * Khối 4: Cấu hình giá bán:
    - Ô nhập Giá gốc (`courses.original_price`): "1,200,000 đ".
    - Ô nhập Giá bán thực tế (`courses.price`): "499,000 đ" (Nhập 0đ nếu là khóa học miễn phí).
- Footer Action Bar:
  * Nút Outline: "Lưu bản nháp" (Save Draft).
  * Nút Primary tím `#4F46E5`: "Lưu & Tiếp tục sang Giáo trình →".

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Form đang điền dữ liệu đầy đủ, chuẩn bị bấm tiếp tục sang Bước 2.
- Realistic Dummy Data: Khóa học "Lập trình Web chuyên sâu với Laravel 11", Giá 499,000 đ.
- Key Actions / CTAs: Nút "Lưu & Tiếp tục sang Giáo trình".

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Các trường bắt buộc có dấu hoa thị đỏ `*`, khoảng cách giữa các khối nhập liệu gap=24px.
```

---

### PROMPT 13 - SCR-INS-03: Trình soạn thảo Giáo trình (Curriculum Builder)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-INS-03: Trình soạn thảo Giáo trình Khóa học (Curriculum Builder)
- Role / User: Giảng viên
- Objective: Màn hình trọng tâm cho phép xây dựng cây cấu trúc Chương - Bài học, upload video, soạn bài đọc và thiết lập học thử theo SRS F3.2, F3.3, F3.5.
- Theme/Style: Interactive Tree Builder, Nền canvas #F8FAFC, Card chương #FFFFFF viền #E2E8F0, Nút thêm bài giảng trực quan.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px.
- Structure: Left Sidebar + Stepper Header (Đang ở Bước 2) + Khung soạn giáo trình (w=1000px căn giữa).
- Visual Hierarchy: Các khối Chương dạng Accordion lồng các thẻ Bài học bên trong; icon kéo-thả phân cấp rõ ràng.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Top Action Bar:
  * Nút Outline: "+ Thêm chương học mới" (`chapters`).
  * Nút Primary xanh lá góc phải: "Gửi yêu cầu phê duyệt khóa học (Submit for Review)" (`F3.5`).
- Vùng Cây Giáo trình (Ánh xạ `chapters`, `lessons`, `lesson_videos`, `lesson_articles`):
  * **Khối Chương 1 (`chapters`):** "Chương 1: Tổng quan và Cài đặt môi trường" (Có nút sửa tên, nút xóa chương, icon drag 6 chấm).
    - Bài 1.1 (`lessons`): Thẻ bài học dạng Video:
      * Icon video xanh dương, Tiêu đề bài: "1.1 Giới thiệu mô hình MVC trong Laravel".
      * Thời lượng (`duration_seconds`): "12:30".
      * Toggle switch: "Học thử miễn phí" (`is_free_preview = TRUE`) đang bật xanh.
      * Thao tác: Nút icon Sửa, Nút icon Xóa.
    - Bài 1.2: Thẻ bài học dạng Bài đọc (`lesson_articles`):
      * Icon văn bản, Tiêu đề: "1.2 Tài liệu hướng dẫn cài đặt Docker trên Windows".
    - Nút gạch đứt nét: "+ Thêm bài học mới vào Chương 1" (Bấm mở rộng chọn: Video / Bài đọc / Quiz).
  * **Khối Chương 2 (`chapters`):** "Chương 2: Xây dựng Routing và Controllers (3 bài học)".
    - Danh sách bài học tương tự bên trong.
- Modal Form Thêm Video Bài giảng (Khi bấm thêm bài học):
  * Nhập tiêu đề bài học (`lessons.title`).
  * Khu vực Upload file video MP4 hoặc nhập link đám mây (`lesson_videos.video_url`).
  * Tự động nhận diện và hiển thị thời lượng (VD: "Phát hiện: 15 phút 20 giây").
  * Checkbox: "[x] Cho phép xem thử miễn phí không cần đăng ký".
  * Nút "Lưu bài học".

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Giáo trình đã có 2 Chương và 5 bài học hoàn chỉnh.
- Realistic Dummy Data: Chương 1 có 3 bài, Chương 2 có 2 bài.
- Key Actions / CTAs: Nút "Gửi yêu cầu phê duyệt khóa học".

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Thẻ bài học thụt lề 24px so với thẻ Chương cha để thể hiện quan hệ cha - con (Parent-Child hierarchy).
- Toggle switch trạng thái ON có màu tím `#4F46E5`.
```

---

### PROMPT 14 - SCR-INS-04: Trình tạo Đề thi Trắc nghiệm (Quiz Builder)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-INS-04: Trình tạo Đề thi Trắc nghiệm (Quiz Builder)
- Role / User: Giảng viên
- Objective: Cấu hình quy chế bài kiểm tra và tạo ngân hàng câu hỏi, đáp án trắc nghiệm, giải thích đáp án theo SRS F3.4.
- Theme/Style: Form Assessment Builder, Nền canvas #F8FAFC, Card câu hỏi trắng bo góc 12px, Accent #4F46E5.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px, Container 900px căn giữa.
- Structure: Header bài quiz + Cấu hình chung + Danh sách các khối câu hỏi lặp lại + Nút Lưu ở chân trang.
- Visual Hierarchy: Mỗi câu hỏi là một thẻ card riêng biệt có đánh số thứ tự rõ ràng kèm các phương án trả lời.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Khối Cấu hình chung (`quizzes`):
  * Tiêu đề bài Quiz: "Kiểm tra kiến thức Chương 2: Controller & Middleware".
  * Ô nhập Tỷ lệ % điểm đỗ (`pass_percentage`): "80%".
  * Ô nhập Thời gian làm bài (`time_limit_minutes`): "15 phút" (Ghi chú: "Để trống nếu không giới hạn thời gian").
- Danh sách Câu hỏi (`quiz_questions`, `quiz_answers`):
  * **Thẻ Câu hỏi 1:**
    - Header thẻ: "Câu hỏi 1" + Nút xóa câu hỏi màu đỏ góc phải.
    - Ô nhập đề bài (`question_text`): "Middleware trong Laravel được sử dụng để làm gì?"
    - Danh sách 4 đáp án lựa chọn:
      * Phương án A: Ô nhập văn bản + Radio tròn đánh dấu đúng (`is_correct = FALSE`).
      * Phương án B: Ô nhập "Lọc và kiểm tra các HTTP request gửi đến ứng dụng" + Radio tròn checked tím (`is_correct = TRUE`).
      * Phương án C: Ô nhập văn bản + Radio (`is_correct = FALSE`).
      * Phương án D: Ô nhập văn bản + Radio (`is_correct = FALSE`).
    - Ô nhập Lời giải thích (`explanation`): "Middleware đóng vai trò như lớp lọc trung gian kiểm tra xác thực trước khi request vào controller."
  * Nút viền nét đứt: "+ Thêm câu hỏi trắc nghiệm mới".
- Footer Action Bar:
  * Nút Primary: "Lưu cấu hình đề thi Quiz" (Nền tím `#4F46E5`).

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Form đang có 2 câu hỏi mẫu đã điền dữ liệu đầy đủ.
- Realistic Dummy Data: Câu hỏi kiến thức Middleware Laravel, đáp án đúng là B.
- Key Actions / CTAs: Nút "Lưu cấu hình đề thi Quiz".

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Radio button đáp án đúng có nhãn nhỏ "(Đáp án đúng)" màu xanh lá để tránh nhầm lẫn.
```

---

### PROMPT 15 - SCR-INS-05: Quản lý Hỏi đáp & Đánh giá (Q&A & Review Management)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-INS-05: Quản lý Hỏi đáp & Đánh giá Khóa học (Q&A & Review Management)
- Role / User: Giảng viên
- Objective: Theo dõi và trả lời các thắc mắc của học viên dưới từng bài học, đồng thời phản hồi công khai đánh giá sao theo SRS F4.7, F4.8.
- Theme/Style: Support & Communication Dashboard, Nền canvas #F8FAFC, Card trắng viền mỏng #E2E8F0, Accent #4F46E5.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px.
- Structure: Left Sidebar Instructor + Topbar + 2 Tabs chính ("Hỏi & Đáp học viên" và "Đánh giá khóa học") + Danh sách thẻ tương tác.
- Visual Hierarchy: Tab Q&A hiển thị các câu hỏi chưa trả lời trên đầu để giảng viên xử lý nhanh.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Top Tab Switcher:
  * Tab 1: "[x] Hỏi & Đáp bài học (3 câu hỏi mới)" (`lesson_comments`).
  * Tab 2: "[ ] Đánh giá khóa học (12 review)" (`course_reviews`).
- Vùng nội dung Tab 1 (Q&A Management):
  * Bộ lọc nhanh: [Tất cả] [Chưa trả lời (Active)] [Đã trả lời].
  * Danh sách Thẻ câu hỏi học viên:
    - Header thẻ: Avatar học viên, Họ tên "Trần Đức Nam", Tên bài học "Bài 14: Xây dựng Middleware", Thời gian "2 giờ trước".
    - Nội dung thắc mắc: "Thầy cho em hỏi khi em khai báo middleware trong bootstrap/app.php thì bị lỗi Class not found, sửa thế nào ạ?"
    - Khung nhập phản hồi của Giảng viên ngay dưới thẻ:
      * Textarea có hỗ trợ chèn code định dạng markdown.
      * Nút "Gửi câu trả lời" (Nền tím `#4F46E5`).
- Vùng nội dung Tab 2 (Review Management):
  * Thẻ đánh giá từ học viên: Tên học viên, Khóa học, Số sao vàng Amber 5/5, Lời nhận xét: "Khóa học rất thực chiến và chi tiết!".
  * Nút "Viết phản hồi công khai" (`instructor_reply`).

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Tab Q&A đang mở, hiển thị 1 câu hỏi đang được soạn phản hồi.
- Realistic Dummy Data: Câu hỏi về lỗi Laravel Middleware, học viên Trần Đức Nam.
- Key Actions / CTAs: Nút "Gửi câu trả lời".

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Thẻ câu hỏi chưa trả lời có viền cam nhạt bên trái (`border-l-4 border-amber-500`) để gây chú ý ưu tiên.
```

---

### PROMPT 16 - SCR-INS-06: Ví Doanh thu & Yêu cầu Rút tiền (Wallet & Payout)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-INS-06: Ví Doanh thu & Yêu cầu Rút tiền (Instructor Wallet & Payout)
- Role / User: Giảng viên
- Objective: Kiểm tra số dư ví khả dụng, cấu hình số tài khoản ngân hàng và lập lệnh yêu cầu rút tiền về tài khoản theo SRS F5.1.
- Theme/Style: Modern Financial Dashboard, Nền canvas #F8FAFC, Card trắng viền #E2E8F0, Accent #10B981 (Xanh lá tài chính).

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px.
- Structure: Left Sidebar Instructor + Topbar + 2 Cột tổng quan số dư (Cột trái 60% Số dư & Rút tiền + Cột phải 40% Thông tin ngân hàng) + Bảng lịch sử rút tiền phía dưới.
- Visual Hierarchy: Thẻ Số dư khả dụng to bản nổi bật, bên cạnh là Nút "Yêu cầu rút tiền".

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Hàng trên: 2 Khối tài chính (Ánh xạ `instructor_profiles`):
  * Khối 1: Thẻ Số dư ví khả dụng (Card nền gradient xanh lục nhạt bo góc 16px):
    - Nhãn: "Số dư ví có thể rút" (`instructor_profiles.wallet_balance`).
    - Số tiền: "18,450,000 đ" (Font to 36px, bold, màu xanh đậm `#065F46`).
    - Ghi chú: "Doanh thu sau khi đã trừ 30% phí nền tảng theo chính sách."
    - Nút CTA: "Yêu cầu rút tiền" (Button nền xanh lục `#10B981`, chữ trắng) mở Modal rút tiền.
  * Khối 2: Thẻ Tài khoản ngân hàng nhận tiền (`instructor_profiles`):
    - Logo ngân hàng (VD: Vietcombank).
    - Tên ngân hàng: "Ngân hàng TMCP Ngoại thương Việt Nam (Vietcombank)".
    - Số tài khoản: `9823481923` (in đậm).
    - Tên chủ tài khoản: `NGUYEN VAN QUANG` (Viết hoa).
    - Nút text: "Thay đổi tài khoản nhận tiền".
- Hàng dưới: Lịch sử yêu cầu rút tiền (`instructor_payouts`):
  * Tiêu đề H2: "Lịch sử yêu cầu rút tiền".
  * Bảng dữ liệu giao dịch:
    - Cột 1: Mã yêu cầu (VD: `PAY-20261101-002`).
    - Cột 2: Ngày tạo (`created_at`).
    - Cột 3: Số tiền yêu cầu (`amount`: "10,000,000 đ").
    - Cột 4: Ngân hàng thụ hưởng.
    - Cột 5: Trạng thái badge:
      * `approved`: Badge xanh lá "Đã chuyển tiền" kèm nút "Xem biên lai chuyển khoản" (`receipt_image`).
      * `pending`: Badge vàng cam "Chờ duyệt".
      * `rejected`: Badge đỏ "Bị từ chối" (hover xem lý do).
- Modal Yêu cầu Rút tiền:
  * Ô nhập Số tiền muốn rút (Kiểm tra tối thiểu 500,000 đ và tối đa bằng số dư ví).
  * Nút "Xác nhận gửi yêu cầu".

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Default state có số dư 18,450,000 đ và bảng lịch sử có 2 giao dịch cũ.
- Realistic Dummy Data: Số dư ví 18.45tr, yêu cầu rút 10tr đã duyệt kèm biên lai.
- Key Actions / CTAs: Nút "Yêu cầu rút tiền".

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Số tiền căn lề phải thẳng hàng, các badge trạng thái phân màu chuẩn xác.
```

---

## III. PHÂN HỆ QUẢN TRỊ VIÊN (ADMIN PORTAL)

---

### PROMPT 17 - SCR-ADM-01: Báo cáo Tổng quan Toàn sàn (Admin Executive Dashboard)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-ADM-01: Báo cáo Tổng quan Toàn sàn (Admin Executive Dashboard)
- Role / User: Quản trị viên (`role = 'admin'`)
- Objective: Giám sát toàn bộ KPI tài chính, doanh thu thực thu 30%, tăng trưởng học viên và khóa học bán chạy theo SRS F5.4.
- Theme/Style: High-end Analytics Dashboard, Nền canvas #0F172A (Dark) hoặc #F8FAFC (Light), Card trắng viền #E2E8F0, Biểu đồ Chart.js trực quan.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px.
- Structure: Left Admin Sidebar (w=260px) + Topbar (h=64px) + Main Content (4 KPI Stat Cards + 2 Khối Biểu đồ + Bảng Top khóa học).
- Visual Hierarchy: 4 thẻ KPI đầu trang cho thấy sức khỏe tài chính toàn sàn, tiếp đến là biểu đồ đường tăng trưởng doanh thu theo tháng.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Left Admin Sidebar (w=260px, nền tối sang trọng `#1E293B`, chữ sáng):
  * Logo hệ thống "EduMaster Admin Panel".
  * Menu quản trị:
    - [x] Dashboard Tổng quan
    - [ ] Kiểm duyệt Khóa học (có badge đỏ số lượng chờ duyệt)
    - [ ] Quản lý Danh mục
    - [ ] Quản lý Mã giảm giá
    - [ ] Quản trị Đơn hàng
    - [ ] Duyệt Rút tiền Payout
    - [ ] Quản trị Người dùng
- Topbar: Tiêu đề Dashboard + Ô tìm kiếm nhanh + Profile Super Admin.
- Main Analytics Workspace:
  * Top 4 KPI Cards (Lưới 4 cột):
    - Thẻ 1: "Tổng doanh thu toàn sàn (Gross)": "285,400,000 đ" (Tăng 18% so với tháng trước).
    - Thẻ 2: "Lợi nhuận sàn 30% (Net Revenue)": "85,620,000 đ" (Màu tím đậm `#4F46E5`).
    - Thẻ 3: "Học viên mới trong tháng": "1,240 học viên" (Icon User).
    - Thẻ 4: "Khóa học chờ kiểm duyệt": "5 khóa học" (Badge cam cảnh báo).
  * Vùng Biểu đồ phân tích (Lưới 2 cột: 65% - 35%):
    - Cột 1 (Biểu đồ đường Line Chart): "Xu hướng doanh thu theo tháng (Tháng 1 -> Tháng 11)".
    - Cột 2 (Biểu đồ tròn Donut Chart): "Tỷ trọng doanh thu theo Danh mục" (Web 55%, Mobile 25%, DevOps 20%).
  * Bảng xếp hạng Top 5 Khóa học bán chạy nhất toàn sàn:
    - Cột: Tên khóa học, Giảng viên, Số lượt mua, Tổng doanh thu, Đánh giá trung bình.

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Default state có đầy đủ biểu đồ và số liệu phân tích tài chính.
- Realistic Dummy Data: Doanh thu sàn 285 triệu, lợi nhuận thực thu 85.6 triệu.
- Key Actions / CTAs: Nút chọn khoảng thời gian (7 ngày qua, 30 ngày qua, năm nay).

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Biểu đồ thể hiện dạng vector sạch sẽ với chú giải (Legend) rõ ràng.
```

---

### PROMPT 18 - SCR-ADM-02: Kiểm duyệt & Xuất bản Khóa học (Course Moderation & Preview)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-ADM-02: Kiểm duyệt & Xuất bản Khóa học (Course Moderation & Inspection)
- Role / User: Quản trị viên
- Objective: Màn hình kiểm tra nội dung khóa học chờ duyệt và đưa ra quyết định Phê duyệt (Publish) hoặc Từ chối kèm lý do theo SRS F3.6.
- Theme/Style: Inspection / Audit Screen, Nền canvas #F8FAFC, Card trắng viền #E2E8F0, Thanh hành động Bottom Bar nổi bật 2 nút Xanh/Đỏ.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px.
- Structure: Left Admin Sidebar + Topbar + Khung xem trước khóa học 2 cột (Cột trái 65% Giáo trình & Video + Cột phải 35% Thông tin khóa học) + Fixed Bottom Action Bar.
- Visual Hierarchy: Thanh cố định dưới chân trang với 2 nút to bản: Xanh lá "Phê duyệt xuất bản" và Đỏ "Từ chối xuất bản".

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Topbar: Nút quay lại danh sách + Tiêu đề: "Kiểm duyệt khóa học: #CRS-8812 - Lập trình Laravel 11 Chuyên Sâu" + Badge vàng "Chờ phê duyệt" (`courses.status = 'pending'`).
- Cột trái: Khung kiểm tra nội dung giáo trình (65%):
  * Khung phát thử video bài giảng (`lesson_videos.video_url`): Admin bấm xem trực tiếp để kiểm tra chất lượng hình ảnh/âm thanh.
  * Cây giáo trình Accordion (`chapters`, `lessons`): Liệt kê toàn bộ chương và bài học, thời lượng, xem bài đọc `lesson_articles`.
  * Khung kiểm tra bài thi trắc nghiệm (`quizzes`): Xem danh sách câu hỏi và đáp án xem có đúng chuẩn chất lượng không.
- Cột phải: Thông tin tổng quan khóa học (35%):
  * Ảnh đại diện thumbnail, Giá bán đề xuất (`courses.price`: "499,000 đ"), Giá gốc (`courses.original_price`).
  * Thông tin giảng viên gửi duyệt (`users.name`, email, chức danh).
  * Checklist tự động đạt chuẩn sàn:
    - [x] Có tối thiểu 1 chương học
    - [x] Có tối thiểu 5 bài học hoàn chỉnh
    - [x] Ảnh đại diện đạt chuẩn 16:9
    - [x] Đã cấu hình giá bán hợp lệ
- Fixed Bottom Action Bar (Thanh nổi chân trang, h=72px, nền trắng, shadow-lg, viền trên):
  * Dòng chữ nhắc nhở: "Vui lòng kiểm tra kỹ nội dung trước khi xuất bản lên trang chủ."
  * Nút Đỏ: "Từ chối duyệt (Reject)" (Mở Modal bắt buộc nhập lý do từ chối `rejection_reason`).
  * Nút Xanh lá: "Phê duyệt & Xuất bản (Approve)" (Chuyển trạng thái `published` và gửi email chúc mừng giảng viên).

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Màn hình đang kiểm duyệt 1 khóa học đầy đủ nội dung.
- Modal Từ chối: Textarea "Nhập lý do từ chối gửi giảng viên" (VD: "Âm thanh bài 3 bị rè và thiếu tài liệu thực hành đính kèm").
- Key Actions / CTAs: Nút "Phê duyệt & Xuất bản" và Nút "Từ chối duyệt".

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Thanh Action Bar dưới đáy ghim cố định toàn màn hình, nút bấm có icon rõ ràng.
```

---

### PROMPT 19 - SCR-ADM-03: Quản lý Cây Danh mục Đào tạo (Category Management)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-ADM-03: Quản lý Cây Danh mục Đào tạo (Category Tree Management)
- Role / User: Quản trị viên
- Objective: Quản lý cây phân cấp danh mục cha - con, icon hiển thị và tối ưu đường dẫn slug SEO theo SRS F2.3.
- Theme/Style: Hierarchical Tree & Form UI, Nền canvas #F8FAFC, Card trắng viền #E2E8F0, Accent #4F46E5.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px.
- Structure: Left Admin Sidebar + Topbar + 2 Cột chia đôi (Cột trái 50% Cây danh mục Tree View + Cột phải 50% Form Thêm/Sửa danh mục).
- Visual Hierarchy: Cây danh mục bên trái thể hiện trực quan quan hệ cha - con; form bên phải cập nhật tương ứng khi click vào một nhánh.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Topbar: Tiêu đề "Quản lý Danh mục Khóa học" + Nút "+ Thêm danh mục cha mới".
- Cột trái: Cây danh mục phân cấp (Tree View - Ánh xạ `categories`):
  * Nhánh Cha 1: Icon Folder - "Lập trình Web" (Slug: `lap-trinh-web`, 120 khóa học):
    - Nhánh Con 1.1: "Laravel Framework" (Slug: `laravel`, 45 khóa học).
    - Nhánh Con 1.2: "ReactJS & Next.js" (Slug: `reactjs`, 38 khóa học).
    - Nhánh Con 1.3: "Vue.js Masterclass" (Slug: `vuejs`, 20 khóa học).
  * Nhánh Cha 2: Icon Folder - "Lập trình Di động" (Slug: `lap-trinh-di-dong`, 65 khóa học):
    - Nhánh Con 2.1: "Flutter & Dart" (Slug: `flutter`).
    - Nhánh Con 2.2: "React Native" (Slug: `react-native`).
  * Thao tác trên từng nhánh: Nút icon Sửa, Nút icon Xóa.
- Cột phải: Form Thêm / Cập nhật Danh mục (Card trắng bo góc 12px, padding 24px):
  * Tiêu đề form: "Chỉnh sửa danh mục: Laravel Framework".
  * Ô nhập Tên danh mục (`categories.name`): "Laravel Framework".
  * Ô nhập Slug SEO (`categories.slug`): "laravel-framework" (Tự động sinh từ tên).
  * Dropdown Danh mục cha (`categories.parent_id`): Chọn "Lập trình Web" (Hoặc chọn "Không có - Là danh mục gốc").
  * Ô nhập Mã Icon (`categories.icon`): "fa-brands fa-laravel" (Hiển thị preview icon bên cạnh).
  * Ô nhập Thứ tự hiển thị (`categories.order`): "1".
  * Nhóm nút: Nút Primary "Lưu thay đổi", Nút Đỏ "Xóa danh mục".

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Nhánh con "Laravel Framework" đang được chọn để chỉnh sửa ở cột bên phải.
- Realistic Dummy Data: Cây danh mục gồm 2 danh mục cha và 5 danh mục con.
- Key Actions / CTAs: Nút "Lưu thay đổi".

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Nhánh con thụt đầu dòng 32px kèm đường kẻ chỉ dẫn cây phân cấp (Tree connector lines).
```

---

### PROMPT 20 - SCR-ADM-04: Quản lý Mã giảm giá (Coupon Management)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-ADM-04: Quản lý Mã giảm giá (Global Coupon Management)
- Role / User: Quản trị viên
- Objective: Cấu hình mã khuyến mãi toàn sàn, loại chiết khấu, hạn dùng và theo dõi lượt sử dụng theo SRS F2.4.
- Theme/Style: Promotion Management Table, Nền canvas #F8FAFC, Card trắng viền #E2E8F0, Accent #4F46E5.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px.
- Structure: Left Admin Sidebar + Topbar + Thanh công cụ tìm kiếm & Nút Tạo mới + Bảng dữ liệu Coupon toàn sàn.
- Visual Hierarchy: Bảng dữ liệu hiển thị rõ mã Coupon in hoa, số lượt dùng và trạng thái Còn hạn / Hết hạn.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Top Action Bar:
  * Tiêu đề: "Quản lý Mã giảm giá toàn hệ thống".
  * Nút CTA góc phải: "+ Tạo mã coupon mới" (Nền tím `#4F46E5`, mở modal tạo).
- Bảng dữ liệu Mã giảm giá (`coupons`):
  * Cột 1: Mã khuyến mãi (`code`): Badge chữ in hoa đậm nền xám `BLACKFRIDAY2026`.
  * Cột 2: Loại chiết khấu (`discount_type`): Badge "Phần trăm (%)" hoặc "Số tiền cố định (VNĐ)".
  * Cột 3: Giá trị giảm (`discount_value`): "50%" hoặc "100,000 đ".
  * Cột 4: Giới hạn sử dụng: "45 / 100 lượt" (`used_count` / `max_uses` kèm thanh progress nhỏ).
  * Cột 5: Hạn sử dụng (`expires_at`): "30/11/2026 23:59".
  * Cột 6: Trạng thái badge:
    * `Còn hiệu lực`: Badge xanh lá `#10B981`.
    * `Hết hạn / Hết lượt`: Badge xám `#64748B`.
  * Cột 7: Thao tác: Nút icon Sửa, Nút icon Xóa.
- Modal Tạo mã Coupon mới (Pop-up):
  * Ô nhập Mã Code (Chữ in hoa không dấu).
  * Radio chọn loại: Giảm theo % hay Giảm theo số tiền.
  * Ô nhập giá trị giảm.
  * Ô nhập số lượt sử dụng tối đa (`max_uses`).
  * Chọn ngày giờ hết hạn (`expires_at`).
  * Nút "Xác nhận tạo mã".

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Bảng hiển thị 4 mã coupon với các trạng thái khác nhau.
- Realistic Dummy Data: Mã `BLACKFRIDAY2026` giảm 50% (đã dùng 45/100 lượt).
- Key Actions / CTAs: Nút "+ Tạo mã coupon mới".

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Mã Code thiết kế dạng font Monospace để người nhìn dễ phân biệt ký tự.
```

---

### PROMPT 21 - SCR-ADM-05: Quản trị Đơn hàng & Đối soát (Order & Audit Management)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-ADM-05: Quản trị Đơn hàng & Đối soát Giao dịch (Order & Audit Management)
- Role / User: Quản trị viên
- Objective: Kiểm toán toàn bộ giao dịch mua bán, tra cứu mã tham chiếu ngân hàng và lưu vết mã giảm giá áp dụng theo SRS F2.7 và chuẩn toàn vẹn CSDL.
- Theme/Style: Financial Audit Table, Nền canvas #F8FAFC, Card trắng viền #E2E8F0, Chữ số căn lề chuẩn mực.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px.
- Structure: Left Admin Sidebar + Topbar + Bộ lọc đa năng (Filter Toolbar) + Bảng dữ liệu Đơn hàng đối soát + Phân trang.
- Visual Hierarchy: Bảng giao dịch rõ ràng với Mã đơn hàng, Mã VNPAY, Số tiền thực thu và Trạng thái thanh toán.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Filter Toolbar:
  * Ô tìm kiếm: Nhập Mã đơn (`order_code`) hoặc Mã tham chiếu ngân hàng (`transaction_id`).
  * Dropdown lọc theo Cổng thanh toán (`payment_method`: Tất cả, VNPAY, MoMo, Miễn phí).
  * Dropdown lọc theo Trạng thái (`payment_status`: Thành công, Chờ xử lý, Thất bại, Hoàn tiền).
  * Bộ chọn khoảng ngày giao dịch.
- Bảng Dữ liệu Đơn hàng (`orders`, `order_items`, `coupons`, `users`):
  * Cột 1: Mã đơn hàng (`orders.order_code`: `ORD-20261105-8821`).
  * Cột 2: Khách hàng: Họ tên học viên (`users.name`) + Email nhỏ bên dưới.
  * Cột 3: Khóa học mua (`courses.title`).
  * Cột 4: Tổng tiền gốc (`orders.total_amount`: "1,499,000 đ").
  * Cột 5: Mã Coupon dùng (`coupons.code`: `DISCOUNT100K` hoặc dấu gạch "-" nếu không dùng).
  * Cột 6: Thực thu sàn (`orders.final_amount`: "499,000 đ" in đậm).
  * Cột 7: Cổng & Mã giao dịch: Logo VNPAY nhỏ kèm mã `VNPAY14892011`.
  * Cột 8: Trạng thái badge:
    * `completed`: Badge xanh lá "Thành công".
    * `pending`: Badge vàng "Chờ thanh toán".
    * `refunded`: Badge tím "Đã hoàn tiền".
  * Cột 9: Thao tác: Nút "Xem chi tiết Audit Trail" (Mở modal xem nhật ký thời gian).
- Pagination Footer: "Hiển thị 1-10 của 1,450 đơn hàng".

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Bảng hiển thị danh sách các đơn hàng mới nhất trong ngày.
- Realistic Dummy Data: Đơn hàng của học viên Lê Văn Hùng, áp mã `DISCOUNT100K`, thanh toán qua VNPAY thành công.
- Key Actions / CTAs: Nút "Xuất dữ liệu Excel / CSV" và Nút xem chi tiết đơn hàng.

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Cột số tiền căn phải (Right-aligned), mã đơn có màu xanh dương liên kết.
```

---

### PROMPT 22 - SCR-ADM-06: Phê duyệt Yêu cầu Rút tiền (Payout Management)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-ADM-06: Phê duyệt Yêu cầu Rút tiền Giảng viên (Payout Management)
- Role / User: Quản trị viên
- Objective: Đối soát số dư ví giảng viên, thực hiện xác nhận giải ngân chuyển khoản kèm tải ảnh biên lai theo SRS F5.2.
- Theme/Style: Bank Disbursement Dashboard, Nền canvas #F8FAFC, Card trắng viền #E2E8F0, Accent #10B981.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px.
- Structure: Left Admin Sidebar + Topbar + Tabs lọc trạng thái duyệt + Bảng dữ liệu yêu cầu giải ngân + Modal xác nhận chuyển tiền.
- Visual Hierarchy: Tab "Chờ xử lý (Pending)" được ưu tiên hiển thị với các nút hành động "Xác nhận chuyển tiền" màu xanh lục.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Top Tab Filter:
  * Tab "[x] Chờ xử lý (Pending - 3 yêu cầu)" (Màu cam nổi bật).
  * Tab "[ ] Đã giải ngân (Approved)".
  * Tab "[ ] Đã từ chối (Rejected)".
- Bảng dữ liệu Yêu cầu Rút tiền (`instructor_payouts`, `instructor_profiles`, `users`):
  * Cột 1: Mã yêu cầu (`id`: `PAY-20261105-001`).
  * Cột 2: Giảng viên: Avatar, Tên giảng viên (`users.name`), Email.
  * Cột 3: Số tiền yêu cầu rút (`amount`: "10,000,000 đ" in đậm).
  * Cột 4: Thông tin tài khoản ngân hàng thụ hưởng (`instructor_profiles`):
    - Ngân hàng: `Vietcombank`
    - Số tài khoản: `9823481923`
    - Tên chủ tài khoản: `NGUYEN VAN QUANG`
  * Cột 5: Thời gian gửi yêu cầu (`created_at`).
  * Cột 6: Hành động:
    - Nút "Xác nhận đã chuyển" (Nền xanh lục `#10B981`, mở modal tải biên lai).
    - Nút "Từ chối" (Màu đỏ, mở modal nhập lý do từ chối).
- Modal Xác nhận Chuyển tiền (Upload Receipt Modal):
  * Tóm tắt: Chuyển 10,000,000 đ cho giảng viên NGUYEN VAN QUANG.
  * Khu vực tải lên: "Tải ảnh chụp ủy nhiệm chi / biên lai chuyển khoản ngân hàng" (`receipt_image`).
  * Ô nhập ghi chú giao dịch (`note`).
  * Nút "Hoàn tất giải ngân" (Chuyển trạng thái `approved` và trừ tiền ví giảng viên).

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Bảng hiển thị danh sách các yêu cầu đang chờ Admin duyệt chuyển tiền.
- Realistic Dummy Data: Giảng viên Nguyễn Văn Quang yêu cầu rút 10,000,000 đ về Vietcombank.
- Key Actions / CTAs: Nút "Xác nhận đã chuyển" và Modal upload biên lai.

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Thông tin số tài khoản ngân hàng có nút nhỏ "Sao chép nhanh" để Admin dễ dàng copy khi thao tác app ngân hàng.
```

---

### PROMPT 23 - SCR-ADM-07: Quản trị Người dùng & Phân quyền (User & Access Control)

```markdown
[LAYER 1: METADATA & CONTEXT]
- Screen Name: SCR-ADM-07: Quản trị Người dùng & Phân quyền (User Management & Access Control)
- Role / User: Quản trị viên cao cấp (Super Admin)
- Objective: Quản lý danh sách tài khoản học viên, giảng viên và kiểm soát trạng thái hoạt động (Khóa/Mở khóa tài khoản) theo SRS F1.6.
- Theme/Style: Security & Identity Management Table, Nền canvas #F8FAFC, Card trắng viền #E2E8F0, Accent #4F46E5.

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: Desktop 1440px.
- Structure: Left Admin Sidebar + Topbar + Bộ lọc tìm kiếm & Phân loại Role + Bảng dữ liệu người dùng + Modal khóa tài khoản.
- Visual Hierarchy: Bảng danh sách người dùng hiển thị rõ Avatar, Vai trò bằng Badge màu riêng biệt và Trạng thái tài khoản.

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Search & Filter Bar:
  * Ô tìm kiếm: Nhập Tên, Email hoặc ID người dùng.
  * Dropdown Vai trò (`users.role`): Tất cả vai trò, Học viên (`student`), Giảng viên (`instructor`), Quản trị viên (`admin`).
  * Dropdown Trạng thái (`users.status`): Hoạt động (`active`), Bị khóa (`banned`).
- Bảng dữ liệu Người dùng (`users`):
  * Cột 1: Người dùng (Avatar tròn, Họ tên `users.name`, Email `users.email`).
  * Cột 2: Vai trò badge (`role`):
    - `student`: Badge xanh dương nhạt "Học viên".
    - `instructor`: Badge tím "Giảng viên".
    - `admin`: Badge đỏ cam "Quản trị viên".
  * Cột 3: Ngày tham gia (`created_at`: "12/09/2026").
  * Cột 4: Hoạt động học tập / dạy: Số khóa đã học (nếu là student) hoặc Số khóa đã tạo (nếu là instructor).
  * Cột 5: Trạng thái (`status`):
    - `active`: Badge xanh lá "Hoạt động".
    - `banned`: Badge đỏ "Bị khóa".
  * Cột 6: Hành động:
    - Nếu đang `active`: Nút Đỏ "Khóa tài khoản" (Ban).
    - Nếu đang `banned`: Nút Xanh "Mở khóa" (Unban).
    - Nút icon "Xem chi tiết hồ sơ".
- Modal Xác nhận Khóa tài khoản (Ban User Modal):
  * Cảnh báo icon tam giác vàng: "Bạn có chắc chắn muốn khóa tài khoản của [Tên người dùng]?"
  * Nhập lý do khóa: Vi phạm điều khoản cộng đồng, phát ngôn xúc phạm, gian lận thanh toán.
  * Nút Đỏ: "Xác nhận khóa tài khoản".

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: Bảng danh sách người dùng hiển thị hỗn hợp các vai trò Student, Instructor và Admin.
- Realistic Dummy Data: Học viên "Lê Văn Hùng", Giảng viên "Nguyễn Văn Quang", Admin "Phạm Minh Hoàng".
- Key Actions / CTAs: Nút "Khóa tài khoản" và Nút "Mở khóa tài khoản".

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Bảng dữ liệu phân cách rõ ràng, avatar người dùng tròn đường kính 40px hiển thị sắc nét.
```
