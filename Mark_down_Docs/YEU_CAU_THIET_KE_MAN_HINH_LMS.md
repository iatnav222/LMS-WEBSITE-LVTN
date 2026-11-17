# TÀI LIỆU YÊU CẦU THIẾT KẾ MÀN HÌNH HỆ THỐNG LMS (MINI-UDEMY)
**Đề tài:** Xây dựng Website Quản lý Học tập Trực tuyến (Learning Management System)  
**Công nghệ triển khai:** Laravel Framework (PHP) & MySQL  
**Mục đích tài liệu:** Quy định chuẩn mực toàn bộ danh mục, cấu trúc và yêu cầu dữ liệu của 23 màn hình cốt lõi. Đây là tài liệu đầu vào (Input Spec) để chuyển đổi thành các Prompt Google Stitch sinh giao diện Artboard báo cáo Giảng viên Hướng dẫn.

---

## MỤC LỤC
1. [QUY CHUẨN DESIGN SYSTEM CHUNG](#1-quy-chuẩn-design-system-chung)
2. [PHÂN HỆ HỌC VIÊN & CÔNG CỘNG - STUDENT & PUBLIC (10 MÀN HÌNH)](#2-phân-hệ-học-viên--công-cộng---student--public-10-màn-hình)
   - [SCR-STU-01: Trang chủ (Homepage / Landing Page)](#scr-stu-01-trang-chủ-homepage--landing-page)
   - [SCR-STU-02: Khám phá & Bộ lọc Khóa học (Search & Course Catalog)](#scr-stu-02-khám-phá--bộ-lọc-khóa-học-search--course-catalog)
   - [SCR-STU-03: Chi tiết Khóa học (Course Landing Page)](#scr-stu-03-chi-tiết-khóa-học-course-landing-page)
   - [SCR-STU-04: Giỏ hàng & Thanh toán (Checkout Page)](#scr-stu-04-giỏ-hàng--thanh-toán-checkout-page)
   - [SCR-STU-05: Thông báo Kết quả Thanh toán (Payment Status / IPN Result)](#scr-stu-05-thông-báo-kết-quả-thanh-toán-payment-status--ipn-result)
   - [SCR-STU-06: Bảng điều khiển Học tập (My Learning Dashboard)](#scr-stu-06-bảng-điều-khiển-học-tập-my-learning-dashboard)
   - [SCR-STU-07: Phòng học / Trình phát Bài giảng (Core Learning Player)](#scr-stu-07-phòng-học--trình-phát-bài-giảng-core-learning-player)
   - [SCR-STU-08: Làm bài kiểm tra Trắc nghiệm (Quiz Assessment)](#scr-stu-08-làm-bài-kiểm-tra-trắc-nghiệm-quiz-assessment)
   - [SCR-STU-09: Chứng chỉ Điện tử & Xác thực QR (Certificate Verification)](#scr-stu-09-chứng-chỉ-điện-tử--xác-thực-qr-certificate-verification)
   - [SCR-STU-10: Hồ sơ Cá nhân & Lịch sử Đơn hàng (Profile & Orders)](#scr-stu-10-hồ-sơ-cá-nhân--lịch-sử-đơn-hàng-profile--orders)
3. [PHÂN HỆ GIẢNG VIÊN - INSTRUCTOR BACKOFFICE (6 MÀN HÌNH)](#3-phân-hệ-giảng-viên---instructor-backoffice-6-màn-hình)
   - [SCR-INS-01: Bảng điều khiển Giảng viên (Instructor Dashboard)](#scr-ins-01-bảng-điều-khiển-giảng-viên-instructor-dashboard)
   - [SCR-INS-02: Thông tin Cơ bản & Định giá Khóa học (Course Info & Pricing)](#scr-ins-02-thông-tin-cơ-bản--định-giá-khóa-học-course-info--pricing)
   - [SCR-INS-03: Trình soạn thảo Giáo trình (Curriculum Builder)](#scr-ins-03-trình-soạn-thảo-giáo-trình-curriculum-builder)
   - [SCR-INS-04: Trình tạo Đề thi Trắc nghiệm (Quiz Builder)](#scr-ins-04-trình-tạo-đề-thi-trắc-nghiệm-quiz-builder)
   - [SCR-INS-05: Quản lý Hỏi đáp & Đánh giá (Q&A & Review Management)](#scr-ins-05-quản-lý-hỏi-đáp--đánh-giá-qa--review-management)
   - [SCR-INS-06: Ví Doanh thu & Yêu cầu Rút tiền (Wallet & Payout)](#scr-ins-06-ví-doanh-thu--yêu-cầu-rút-tiền-wallet--payout)
4. [PHÂN HỆ QUẢN TRỊ VIÊN - ADMIN PORTAL (7 MÀN HÌNH)](#4-phân-hệ-quản-trị-viên---admin-portal-7-màn-hình)
   - [SCR-ADM-01: Báo cáo Tổng quan Toàn sàn (Admin Executive Dashboard)](#scr-adm-01-báo-cáo-tổng-quan-toàn-sàn-admin-executive-dashboard)
   - [SCR-ADM-02: Kiểm duyệt & Xuất bản Khóa học (Course Moderation & Preview)](#scr-adm-02-kiểm-duyệt--xuất-bản-khóa-học-course-moderation--preview)
   - [SCR-ADM-03: Quản lý Cây Danh mục Đào tạo (Category Management)](#scr-adm-03-quản-lý-cây-danh-mục-đào-tạo-category-management)
   - [SCR-ADM-04: Quản lý Mã giảm giá (Coupon Management)](#scr-adm-04-quản-lý-mã-giảm-giá-coupon-management)
   - [SCR-ADM-05: Quản trị Đơn hàng & Đối soát (Order & Audit Management)](#scr-adm-05-quản-trị-đơn-hàng--đối-soát-order--audit-management)
   - [SCR-ADM-06: Phê duyệt Yêu cầu Rút tiền (Payout Management)](#scr-adm-06-phê-duyệt-yêu-cầu-rút-tiền-payout-management)
   - [SCR-ADM-07: Quản trị Người dùng & Phân quyền (User & Access Control)](#scr-adm-07-quản-trị-người-dùng--phân-quyền-user--access-control)
5. [BẢNG TỔNG HỢP ÁNH XẠ MÀN HÌNH - TÍNH NĂNG - DATABASE](#5-bảng-tổng-hợp-ánh-xạ-màn-hình---tính-năng---database)

---

## 1. QUY CHUẨN DESIGN SYSTEM CHUNG
* **Phong cách:** Hiện đại, Tinh gọn (Clean Modern EdTech / SaaS), đường nét trực quan, không chi tiết thừa.
* **Bảng màu:**
  * Primary: `#4F46E5` (Indigo 600) — Nhận diện thương hiệu, nút CTA hành động, đường dẫn active.
  * Secondary / Accent: `#F59E0B` (Amber 500) — Đánh giá sao, huy hiệu nổi bật, nút mua hàng.
  * Dark Mode rạp chiếu: `#0B0F19` (Slate 950) — Dành riêng cho màn hình phòng học `SCR-STU-07` để chống mỏi mắt.
  * Neutral Background: `#F8FAFC` (Slate 50), Card `#FFFFFF`, Border `#E2E8F0`.
  * Semantic: Success `#10B981`, Warning `#F59E0B`, Danger `#EF4444`, Info `#3B82F6`.
* **Typography:** Font **Inter** hoặc **Plus Jakarta Sans**, chuẩn tỷ lệ 8pt spacing (8px, 16px, 24px, 32px).
* **Viewport:** Desktop 1440px, bố cục 12-column grid.

---

## 2. PHÂN HỆ HỌC VIÊN & CÔNG CỘNG - STUDENT & PUBLIC (10 MÀN HÌNH)

---

### SCR-STU-01: Trang chủ (Homepage / Landing Page)
* **Vai trò:** Khách vãng lai (Guest), Học viên (Student).
* **Mục tiêu nghiệp vụ:** Giới thiệu nền tảng, thúc đẩy tìm kiếm và điều hướng người dùng đăng ký/mua khóa học (`F1.1`, `F2.1`).
* **Ánh xạ CSDL:** `categories` (danh mục nổi bật), `courses` (khóa học thịnh hành/mới nhất, filter `status = 'published'`), `users` (tên tác giả), `course_reviews` (tính rating sao trung bình).
* **Bố cục & Thành phần cốt lõi:**
  * Top Navigation Bar: Logo, Menu danh mục đa cấp (Dropdown `categories`), Thanh tìm kiếm nhanh, Nút "Giỏ hàng", Nút "Đăng nhập / Đăng ký" (hoặc Avatar nếu đã login).
  * Hero Section: Headline truyền cảm hứng, ô tìm kiếm từ khóa to bản, badge thống kê số lượng học viên & khóa học.
  * Featured Categories Section: Lưới 6-8 thẻ danh mục (`categories.name`, `icon`, số lượng khóa học).
  * Trending Courses Section: Lưới 4 cột hiển thị Course Cards (`thumbnail`, `title`, tên giảng viên, rating sao trung bình, giá bán `price` và giá gốc gạch ngang `original_price`).
  * Learning Paths Banner (Cảm hứng F8): Lộ trình học bài bản (Frontend, Backend Laravel).
  * Footer: Liên kết điều khoản, thông tin bản quyền và liên hệ.
* **Trạng thái yêu cầu:**
  * Default: Đầy đủ dữ liệu khóa học và banner.
  * Empty: Khi danh mục chưa có khóa học (hiển thị thông báo "Đang cập nhật").

---

### SCR-STU-02: Khám phá & Bộ lọc Khóa học (Search & Course Catalog)
* **Vai trò:** Khách vãng lai, Học viên.
* **Mục tiêu nghiệp vụ:** Tìm kiếm, lọc và phân loại khóa học đa tiêu chí để chọn lựa chính xác (`F2.1`).
* **Ánh xạ CSDL:** `courses`, `categories`, `course_reviews`.
* **Bố cục & Thành phần cốt lõi:**
  * Breadcrumb: Trang chủ / Danh mục khóa học.
  * Left Filter Sidebar (w=280px):
    * Lọc theo Danh mục (Checklist đa cấp `categories`).
    * Lọc theo Cấp độ (Checkboxes: Mọi cấp độ, Người mới, Trung cấp, Nâng cao tương ứng `courses.level`).
    * Lọc theo Mức giá (Radio buttons: Tất cả, Miễn phí `price = 0`, Có phí `price > 0`).
    * Lọc theo Đánh giá sao (Từ 4.5 sao, từ 4.0 sao).
  * Main Content (Catalog Grid):
    * Header bar: Tổng số kết quả tìm thấy (`X khóa học`), Bộ sắp xếp (Mới nhất, Đánh giá cao nhất, Bán chạy nhất).
    * Lưới Course Cards (3 cột): Ảnh bìa, Nhãn cấp độ, Tiêu đề, Giảng viên, Đánh giá sao & lượt review, Giá tiền nổi bật.
    * Pagination: Phân trang chuẩn 12 khóa học/trang.
* **Trạng thái yêu cầu:**
  * Default: Danh sách khóa học thỏa mãn bộ lọc.
  * Empty State: "Không tìm thấy khóa học nào phù hợp với bộ lọc của bạn" kèm nút "Đặt lại bộ lọc".

---

### SCR-STU-03: Chi tiết Khóa học (Course Landing Page)
* **Vai trò:** Khách vãng lai, Học viên.
* **Mục tiêu nghiệp vụ:** Thuyết phục người học mua khóa học qua thông tin đầy đủ, video xem thử và minh chứng xã hội (`F2.2`).
* **Ánh xạ CSDL:** `courses`, `chapters`, `lessons`, `lesson_videos`, `users` (Instructor), `course_reviews`.
* **Bố cục & Thành phần cốt lõi:**
  * Hero Header tối màu: Tiêu đề khóa học (`courses.title`), tóm tắt ngắn (`summary`), badge cấp độ (`level`), tên giảng viên (`users.name`), ngày cập nhật cuối.
  * Cột trái (Main Content - 68%):
    * Khối "Bạn sẽ học được gì?" (What you will learn - viền highlight).
    * Khối "Nội dung khóa học" (Curriculum Accordion): Danh sách các Chương (`chapters.title`), mở ra các Bài học (`lessons.title`, thời lượng `duration_seconds`). Bài học nào có `is_free_preview = TRUE` sẽ có badge "Học thử" màu xanh và nút bấm mở video xem ngay.
    * Khối "Mô tả chi tiết" (Rich text markdown).
    * Khối "Thông tin giảng viên": Avatar, Headline, Bio tóm tắt.
    * Khối "Đánh giá từ học viên": Điểm sao trung bình tổng quan, thanh biểu đồ % phân bổ 5 sao - 1 sao, danh sách review chi tiết kèm bình luận và phản hồi giảng viên.
  * Cột phải (Sticky Sidebar Card - 32%):
    * Khung phát Video giới thiệu (`promo_video_url`).
    * Giá bán hiện tại (`price`), giá gốc (`original_price`), nhãn giảm giá %.
    * Nút CTA chính: "Mua ngay" (Màu cam nổi bật) và nút "Thêm vào giỏ hàng".
    * Cam kết hoàn tiền 7 ngày, quyền truy cập trọn đời, cấp chứng chỉ hoàn thành.
* **Trạng thái yêu cầu:**
  * Default: Khách chưa mua (hiển thị nút Mua ngay/Thêm giỏ).
  * Enrolled State: Học viên đã mua khóa học (nút đổi thành "Tiếp tục học" dẫn vào `SCR-STU-07`).

---

### SCR-STU-04: Giỏ hàng & Thanh toán (Checkout Page)
* **Vai trò:** Học viên (Bắt buộc đăng nhập).
* **Mục tiêu nghiệp vụ:** Rà soát đơn hàng, áp dụng coupon giảm giá và chọn cổng thanh toán trực tuyến (`F2.4`, `F2.5`).
* **Ánh xạ CSDL:** `orders`, `order_items`, `coupons`, `courses`.
* **Bố cục & Thành phần cốt lõi:**
  * Bố cục 2 cột (60% - 40%):
  * Cột trái (Order Review & Payment Method):
    * Danh sách khóa học thanh toán: Thumbnail nhỏ, tên khóa học, giá tiền.
    * Phương thức thanh toán (Radio options có logo): Cổng VNPAY (Quét QR / ATM nội địa), Ví MoMo.
  * Cột phải (Order Summary Card):
    * Tạm tính gốc (`total_amount`).
    * Khung nhập mã giảm giá (`coupons.code`) + nút "Áp dụng".
    * Dòng chiết khấu coupon (`discount_amount`) hiển thị chữ xanh âm tiền (nếu áp dụng thành công).
    * Tổng thanh toán cuối cùng (`final_amount`) in đậm to bản.
    * Nút CTA: "Xác nhận thanh toán VNPAY".
* **Trạng thái yêu cầu:**
  * Default: Đơn hàng nguyên giá.
  * Coupon Success: Hiển thị tag mã đã dùng, trừ tiền trực tiếp.
  * Coupon Error: Thông báo đỏ "Mã giảm giá không hợp lệ hoặc đã hết lượt dùng".
  * Free Course: Đơn hàng 0đ, nút đổi thành "Kích hoạt vào học ngay" (không gọi VNPAY).

---

### SCR-STU-05: Thông báo Kết quả Thanh toán (Payment Status / IPN Result)
* **Vai trò:** Học viên.
* **Mục tiêu nghiệp vụ:** Xác nhận trạng thái xử lý đơn hàng từ Webhook ngân hàng và dẫn dắt học viên vào học (`F2.6`).
* **Ánh xạ CSDL:** `orders` (`order_code`, `final_amount`, `payment_status`, `transaction_id`), `enrollments`.
* **Bố cục & Thành phần cốt lõi:**
  * Khung Card trung tâm (Center Modal Card, w=640px):
    * Trường hợp Thành công: Icon tích xanh lớn hoạt họa, Tiêu đề "Thanh toán thành công!", Mã đơn hàng (`order_code`), Mã giao dịch ngân hàng (`transaction_id`), Số tiền thanh toán, Tên khóa học đã ghi danh.
    * Nút CTA chính: "Bắt đầu học ngay" (dẫn vào phòng học), Nút phụ: "Xem hóa đơn / Lịch sử đơn hàng".
    * Trường hợp Thất bại: Icon dấu X đỏ, lý do lỗi ("Giao dịch bị hủy bởi người dùng hoặc số dư không đủ"), nút "Thử thanh toán lại".
* **Trạng thái yêu cầu:** Success State / Failed State.

---

### SCR-STU-06: Bảng điều khiển Học tập (My Learning Dashboard)
* **Vai trò:** Học viên.
* **Mục tiêu nghiệp vụ:** Quản trị các khóa học cá nhân đã ghi danh và theo dõi tiến độ hoàn thành (`F4.1`).
* **Ánh xạ CSDL:** `enrollments`, `courses`, `lesson_progress`.
* **Bố cục & Thành phần cốt lõi:**
  * Top Bar: Tiêu đề "Khóa học của tôi", tab chuyển đổi ("Tất cả khóa học", "Đang học", "Đã hoàn thành").
  * Lưới khóa học cá nhân (3 cột):
    * Thẻ khóa học sở hữu: Ảnh bìa, Tiêu đề, Tên giảng viên.
    * Thanh Progress Bar trực quan (% hoàn thành tính từ `lesson_progress`).
    * Số bài đã học / Tổng số bài (VD: `18/24 bài học`).
    * Nút CTA: "Tiếp tục học" (tự động link đến bài học dở gần nhất qua `last_watch_second`).
    * Nếu đã đạt 100%: Xuất hiện nút "Xem chứng chỉ" có icon cúp vàng.
* **Trạng thái yêu cầu:**
  * Default: Danh sách các khóa đang theo học.
  * Empty State: "Bạn chưa đăng ký khóa học nào" kèm nút "Khám phá khóa học ngay".

---

### SCR-STU-07: Phòng học / Trình phát Bài giảng (Core Learning Player)
> **MÀN HÌNH ĐINH CỦA ĐỒ ÁN - ĐƯỢC CHẤM ĐIỂM CAO NHẤT**
* **Vai trò:** Học viên đã ghi danh (`enrollments`).
* **Mục tiêu nghiệp vụ:** Trải nghiệm xem video học tập, tự động lưu vị trí, học tuần tự, ghi chú timestamp và hỏi đáp (`F4.2`, `F4.3`, `F4.4`, `F4.7`).
* **Ánh xạ CSDL:** `lessons`, `chapters`, `lesson_videos`, `lesson_articles`, `lesson_progress`, `lesson_notes`, `lesson_comments`.
* **Bố cục & Thành phần cốt lõi:**
  * Giao diện Full-screen Theater Mode nền tối (`#0B0F19`):
  * Cột trái (Workspace - 75%):
    * Khung Video Player HTML5: Thanh điều khiển tiến độ phát, nút Play/Pause, thời lượng, nút chỉnh tốc độ phát ($0.75x - 2x$), nút toàn màn hình.
    * Bên dưới Video: Tiêu đề bài học, nút "Bài trước", nút "Bài tiếp theo" (bị vô hiệu hóa nếu chưa đủ điều kiện tuần tự).
    * Khu vực Tab tương tác đa chức năng:
      * **Tab 1: Tổng quan & Bài đọc:** Nội dung lý thuyết văn bản (`lesson_articles`) nếu bài giảng là dạng đọc.
      * **Tab 2: Ghi chú (Timestamp Notes):** Nút "Thêm ghi chú tại 02:45". Danh sách các ghi chú đã lưu (`timestamp_second`, nội dung). Bấm vào ghi chú thì video lập tức tua đến giây tương ứng.
      * **Tab 3: Hỏi đáp (Q&A):** Form nhập câu hỏi (hỗ trợ markdown/code). Cây bình luận đa tầng lồng nhau (`lesson_comments.parent_id`), nút Trả lời dưới từng bình luận.
  * Cột phải (Sidebar Giáo trình - 25%):
    * Header: Tiến độ khóa học (% hoàn thành).
    * Danh sách Accordion các Chương: Liệt kê các bài học.
    * Trạng thái bài học:
      * Icon Tích xanh lá: Đã hoàn thành (`is_completed = TRUE`).
      * Icon Đang phát (màu tím Indigo): Bài học đang mở xem.
      * Icon Ổ khóa xám: Chưa được mở (phải học xong bài trước mới mở khóa).
* **Trạng thái yêu cầu:**
  * Video Playing State: Đang phát video và định kỳ lưu `last_watch_second`.
  * Article Lesson State: Hiển thị bài đọc thay cho khung video.
  * Completed Lesson Trigger: Đạt $\ge 80\%$ thời lượng $\rightarrow$ Tự động tích xanh và mở khóa bài tiếp theo.

---

### SCR-STU-08: Làm bài kiểm tra Trắc nghiệm (Quiz Assessment)
* **Vai trò:** Học viên.
* **Mục tiêu nghiệp vụ:** Đánh giá năng lực tiếp thu, chấm điểm tự động và quyết định mở khóa bài học kế tiếp (`F4.5`).
* **Ánh xạ CSDL:** `quizzes`, `quiz_questions`, `quiz_answers`, `quiz_submissions`, `lesson_progress`.
* **Bố cục & Thành phần cốt lõi:**
  * Bố cục tập trung (Single-focus container, w=900px):
  * Header: Tên bài Quiz, Đồng hồ đếm ngược thời gian (`time_limit_minutes`), Thanh đếm số câu (VD: `Câu 3 / 10`).
  * Vùng câu hỏi:
    * Tiêu đề câu hỏi (`question_text`).
    * Danh sách các phương án trả lời dạng thẻ bấm chọn (`quiz_answers.answer_text`).
  * Footer: Nút "Câu trước", nút "Câu tiếp theo", nút "Nộp bài thi" (màu tím nổi bật).
  * Màn hình Kết quả (Result Screen sau khi nộp):
    * Vòng tròn điểm số % đạt được (`quiz_submissions.score`).
    * Badge kết quả to: "XUẤT SẮC - ĐẠT" (Xanh lá) hoặc "CHƯA ĐẠT" (Đỏ).
    * Danh sách giải thích chi tiết: Hiển thị câu nào đúng, câu nào sai kèm lời giải thích (`explanation`).
    * Nút CTA: "Học bài tiếp theo" (nếu Đạt) hoặc "Làm lại bài thi" (nếu Trượt).
* **Trạng thái yêu cầu:** In-progress State (đang đếm giờ) / Result Review State.

---

### SCR-STU-09: Chứng chỉ Điện tử & Xác thực QR (Certificate Verification)
* **Vai trò:** Học viên, Nhà tuyển dụng / Khách ngoài tra cứu công khai.
* **Mục tiêu nghiệp vụ:** Vinh danh học viên hoàn thành 100% khóa học và cung cấp trang xác minh văn bằng chống làm giả (`F4.6`).
* **Ánh xạ CSDL:** `certificates`, `courses`, `users`.
* **Bố cục & Thành phần cốt lõi:**
  * Trang công khai (Public Verification Layout):
  * Khung hiển thị Chứng chỉ chính thức (Bản mô phỏng PDF):
    * Logo sàn LMS, Con dấu bảo chứng, Chữ ký số Ban giám đốc.
    * Dòng chữ vinh danh: "Chứng nhận học viên [Họ và tên] đã hoàn thành xuất sắc khóa học [Tên khóa học]".
    * Ngày cấp chính thức (`issued_at`), Mã định danh UUID (`certificate_code`).
  * Bảng điều khiển hành động:
    * Nút "Tải xuống chứng chỉ PDF" (gọi Laravel DomPDF).
    * Mã QR Code chứa URL tra cứu công khai trực tiếp.
    * Nút "Sao chép liên kết chia sẻ lên LinkedIn / CV".
* **Trạng thái yêu cầu:** Verified Valid State (Chứng chỉ hợp lệ, tích xanh) / Invalid Code State (Báo mã không tồn tại nếu nhập sai code).

---

### SCR-STU-10: Hồ sơ Cá nhân & Lịch sử Đơn hàng (Profile & Orders)
* **Vai trò:** Học viên.
* **Mục tiêu nghiệp vụ:** Cập nhật thông tin cá nhân, đổi mật khẩu và tra cứu lịch sử hóa đơn đơn hàng (`F1.3`, `F1.4`, `F2.7`).
* **Ánh xạ CSDL:** `users`, `orders`, `order_items`, `instructor_profiles`.
* **Bố cục & Thành phần cốt lõi:**
  * Bố cục 2 cột (Sidebar menu cá nhân + Nội dung tab):
  * Tab 1: Thông tin cá nhân:
    * Form cập nhật Họ tên, tải lên Avatar, đổi mật khẩu (yêu cầu mật khẩu cũ).
    * Nút banner nổi bật: "Đăng ký trở thành Giảng viên" (chuyển hướng sang modal nộp đơn `F1.4`).
  * Tab 2: Lịch sử đơn hàng:
    * Bảng danh sách giao dịch: Mã đơn (`order_code`), Ngày mua, Tên khóa học, Phương thức (VNPAY/MoMo), Số tiền thanh toán (`final_amount`), Trạng thái (`completed`/`refunded`).
    * Nút xem biên lai thanh toán chi tiết.
* **Trạng thái yêu cầu:** Default Profile / Order History Table.

---

## 3. PHÂN HỆ GIẢNG VIÊN - INSTRUCTOR BACKOFFICE (6 MÀN HÌNH)

---

### SCR-INS-01: Bảng điều khiển Giảng viên (Instructor Dashboard)
* **Vai trò:** Giảng viên (`role = 'instructor'`).
* **Mục tiêu nghiệp vụ:** Thống kê tổng quan kết quả giảng dạy và quản lý danh sách các khóa học của mình (`F5.1`, `F5.3`).
* **Ánh xạ CSDL:** `courses`, `enrollments`, `instructor_profiles`, `course_reviews`.
* **Bố cục & Thành phần cốt lõi:**
  * Top Metric Cards (4 thẻ KPI):
    * Thẻ 1: Tổng doanh thu thực nhận ví (`wallet_balance`).
    * Thẻ 2: Tổng học viên ghi danh toàn bộ khóa học.
    * Thẻ 3: Đánh giá trung bình sàn (VD: `4.8 ★`).
    * Thẻ 4: Số khóa học đã xuất bản (`published`).
  * Bảng "Danh sách khóa học của tôi":
    * Cột: Ảnh bìa, Tên khóa học, Giá bán, Số học viên, Doanh thu, Trạng thái badge (`draft` - Xám, `pending` - Vàng, `published` - Xanh lá, `rejected` - Đỏ).
    * Cột Thao tác: Nút "Chỉnh sửa nội dung", Nút "Xem thống kê".
  * Nút CTA chính góc phải: "+ Tạo khóa học mới" (Màu tím).
* **Trạng thái yêu cầu:** Default with Courses / Empty State (Khi giảng viên mới đăng ký, chưa có khóa học).

---

### SCR-INS-02: Thông tin Cơ bản & Định giá Khóa học (Course Info & Pricing)
* **Vai trò:** Giảng viên.
* **Mục tiêu nghiệp vụ:** Nhập liệu thông tin quảng bá khóa học và chính sách giá bán (`F3.1`).
* **Ánh xạ CSDL:** `courses`, `categories`.
* **Bố cục & Thành phần cốt lõi:**
  * Form dạng bước (Stepper Navigation): 1. Thông tin cơ bản -> 2. Giáo trình -> 3. Định giá -> 4. Gửi duyệt.
  * Vùng nhập liệu chi tiết:
    * Tiêu đề khóa học (`courses.title`), Tự động sinh `slug`.
    * Tóm tắt ngắn (`summary`), Trình soạn thảo mô tả chi tiết Rich Text (`description`).
    * Dropdown chọn Danh mục (`category_id`), Dropdown chọn Cấp độ (`level`).
    * Upload vùng kéo thả ảnh bìa Thumbnail (`thumbnail`) và Video giới thiệu Trailer.
    * Cấu hình giá: Ô nhập Giá gốc (`original_price`), Ô nhập Giá khuyến mãi thực bán (`price`).
  * Nút "Lưu bản nháp" (Save Draft) và "Tiếp tục sang Giáo trình".
* **Trạng thái yêu cầu:** Form nhập mới / Form chỉnh sửa khóa học hiện có kèm Validation Error (báo đỏ nếu bỏ trống trường bắt buộc).

---

### SCR-INS-03: Trình soạn thảo Giáo trình (Curriculum Builder)
> **MÀN HÌNH ĐINH CỦA GIẢNG VIÊN - THỂ HIỆN TRÌNH ĐỘ XỬ LÝ CẤU TRÚC PHỨC TẠP**
* **Vai trò:** Giảng viên.
* **Mục tiêu nghiệp vụ:** Xây dựng cây phân cấp Chương - Bài học, đăng tải video và tài liệu học tập (`F3.2`, `F3.3`, `F3.5`).
* **Ánh xạ CSDL:** `chapters`, `lessons`, `lesson_videos`, `lesson_articles`, `quizzes`.
* **Bố cục & Thành phần cốt lõi:**
  * Top Bar: Nút "+ Thêm chương học mới", Nút "Gửi yêu cầu phê duyệt khóa học" (Submit for Review).
  * Vùng danh sách Chương Accordion (Kéo thả sắp xếp thứ tự `order`):
    * Tiêu đề Chương (Cho phép sửa tên nhanh inline).
    * Bên trong Chương là danh sách các Bài học (`lessons`):
      * Thẻ bài học: Icon loại bài (Video/Bài đọc/Quiz), Tiêu đề bài học, Thời lượng, Badge "Học thử" (Toggle switch `is_free_preview`).
      * Khối thêm bài học mới:
        * Chọn tab **Video:** Ô tải file video lên hoặc nhập link Cloud, tự động hiển thị thời lượng `duration_seconds`.
        * Chọn tab **Bài đọc:** Mở khung soạn thảo nội dung văn bản `lesson_articles`.
        * Chọn tab **Bài thi Quiz:** Nút liên kết mở trình tạo câu hỏi trắc nghiệm `SCR-INS-04`.
      * Nút thao tác: Sửa, Xóa bài học.
* **Trạng thái yêu cầu:**
  * Empty Chapter State: Chương chưa có bài học.
  * Full Curriculum State: Có nhiều chương và bài học hoàn chỉnh.
  * Pending Lock State: Khi khóa học đang ở trạng thái `pending` chờ Admin duyệt, toàn bộ nút sửa/xóa bị khóa (Read-only).

---

### SCR-INS-04: Trình tạo Đề thi Trắc nghiệm (Quiz Builder)
* **Vai trò:** Giảng viên.
* **Mục tiêu nghiệp vụ:** Thiết lập quy chế bài kiểm tra và nhập ngân hàng câu hỏi đáp án (`F3.4`).
* **Ánh xạ CSDL:** `quizzes`, `quiz_questions`, `quiz_answers`.
* **Bố cục & Thành phần cốt lõi:**
  * Khối cấu hình chung:
    * Nhập tỷ lệ % điểm đỗ (`pass_percentage`, mặc định 80%).
    * Nhập thời gian làm bài đếm ngược (`time_limit_minutes`, để trống nếu không giới hạn).
  * Danh sách Câu hỏi trắc nghiệm:
    * Ô nhập nội dung câu hỏi (`question_text`).
    * Danh sách 4 đáp án lựa chọn (`quiz_answers`): Ô nhập văn bản kèm Radio button bên cạnh để đánh dấu phương án đúng (`is_correct = TRUE`).
    * Ô nhập lời giải thích đáp án (`explanation`): Hiển thị cho học viên sau khi nộp bài.
    * Nút "+ Thêm câu hỏi tiếp theo".
  * Nút CTA: "Lưu cấu hình Quiz".
* **Trạng thái yêu cầu:** Form builder tương tác, có thể thêm/xóa bớt đáp án linh hoạt.

---

### SCR-INS-05: Quản lý Hỏi đáp & Đánh giá (Q&A & Review Management)
* **Vai trò:** Giảng viên.
* **Mục tiêu nghiệp vụ:** Tương tác, hỗ trợ học viên giải đáp thắc mắc và phản hồi nhận xét khóa học (`F4.7`, `F4.8`).
* **Ánh xạ CSDL:** `lesson_comments`, `course_reviews`, `lessons`, `courses`.
* **Bố cục & Thành phần cốt lõi:**
  * Chuyển đổi 2 tab chính:
  * **Tab 1: Quản lý Hỏi đáp (Q&A):**
    * Bộ lọc câu hỏi: Tất cả, Chưa trả lời, Đã trả lời.
    * Danh sách thẻ câu hỏi: Tên học viên, Tên bài học liên quan, Thời gian, Nội dung câu hỏi.
    * Khung nhập phản hồi của giảng viên (gửi câu trả lời lồng nhau qua `parent_id`).
  * **Tab 2: Đánh giá khóa học (Reviews):**
    * Danh sách đánh giá từ học viên: Số sao rating, Tên khóa học, Nội dung nhận xét.
    * Khung phản hồi công khai của giảng viên (`instructor_reply`).
* **Trạng thái yêu cầu:** Default with comments / Empty Q&A State.

---

### SCR-INS-06: Ví Doanh thu & Yêu cầu Rút tiền (Wallet & Payout)
* **Vai trò:** Giảng viên.
* **Mục tiêu nghiệp vụ:** Theo dõi số dư ví doanh thu bán khóa học và lập lệnh rút tiền về tài khoản ngân hàng (`F5.1`).
* **Ánh xạ CSDL:** `instructor_profiles`, `instructor_payouts`.
* **Bố cục & Thành phần cốt lõi:**
  * Bố cục 2 khối:
  * Khối 1: Thông tin số dư & Tài khoản nhận tiền:
    * Thẻ số dư ví khả dụng (`wallet_balance`, ví dụ: `15,450,000 đ`).
    * Thẻ thông tin ngân hàng đã liên kết: Tên ngân hàng (`bank_name`), Số tài khoản (`bank_account_number`), Chủ tài khoản (`bank_account_name`).
    * Nút mở Modal "Rút tiền về tài khoản".
  * Khối 2: Lịch sử yêu cầu rút tiền:
    * Bảng danh sách giao dịch giải ngân: Mã yêu cầu, Ngày tạo, Số tiền rút, Trạng thái badge (`pending` - Chờ xử lý, `approved` - Đã chuyển tiền, `rejected` - Bị từ chối).
    * Cột xem biên lai: Bấm xem ảnh chụp ủy nhiệm chi (`receipt_image`) do Admin tải lên.
* **Trạng thái yêu cầu:**
  * Modal Rút tiền: Nhập số tiền muốn rút (kiểm tra điều kiện: Số tiền $\ge 500,000$đ và $\le wallet\_balance$).

---

## 4. PHÂN HỆ QUẢN TRỊ VIÊN - ADMIN PORTAL (7 MÀN HÌNH)

---

### SCR-ADM-01: Báo cáo Tổng quan Toàn sàn (Admin Executive Dashboard)
* **Vai trò:** Quản trị viên (`role = 'admin'`).
* **Mục tiêu nghiệp vụ:** Giám sát chỉ số tài chính, doanh thu thực thu $30\%$ của sàn và nhịp độ tăng trưởng hệ thống (`F5.4`).
* **Ánh xạ CSDL:** `orders`, `order_items`, `users`, `courses`, `enrollments`.
* **Bố cục & Thành phần cốt lõi:**
  * Top KPI Stat Cards (4 thẻ):
    * Tổng doanh thu toàn sàn (Gross Revenue).
    * Lợi nhuận sàn thực thu ($30\%$ Net Platform Revenue).
    * Tổng số học viên mới trong tháng.
    * Số khóa học đang chờ duyệt (`pending_approval`).
  * Vùng Biểu đồ tương tác (Chart.js / ApexCharts):
    * Biểu đồ đường (Line chart): Doanh thu theo tháng trong năm.
    * Biểu đồ tròn (Donut chart): Doanh thu phân bổ theo danh mục đào tạo (`categories`).
  * Bảng xếp hạng Top 5 Khóa học bán chạy nhất (Doanh thu, số lượt mua).
* **Trạng thái yêu cầu:** Biểu đồ hiển thị dữ liệu trực quan sinh động.

---

### SCR-ADM-02: Kiểm duyệt & Xuất bản Khóa học (Course Moderation & Preview)
> **MÀN HÌNH ĐINH CỦA ADMIN - THỂ HIỆN VÒNG ĐỜI NGHIỆP VỤ DUYỆT BÀI BẢN**
* **Vai trò:** Quản trị viên.
* **Mục tiêu nghiệp vụ:** Đảm bảo chất lượng khóa học trước khi xuất bản công khai ra ngoài sàn (`F3.6`).
* **Ánh xạ CSDL:** `courses`, `chapters`, `lessons`, `lesson_videos`, `quizzes`.
* **Bố cục & Thành phần cốt lõi:**
  * Danh sách khóa học chờ duyệt (Bảng lọc trạng thái `pending`).
  * Màn hình Duyệt chi tiết (Inspection Screen khi bấm vào 1 khóa học):
    * Cột trái: Xem trước toàn bộ giáo trình, bấm phát thử các video bài giảng của giảng viên, xem bài thi trắc nghiệm.
    * Cột phải: Thông tin tóm tắt giảng viên, giá bán, cam kết chất lượng.
    * Thanh hành động cố định bên dưới (Action Bottom Bar):
      * Nút **"Phê duyệt xuất bản" (Approve - Màu xanh lá):** Đổi status thành `published`, khóa học lập tức lên trang chủ.
      * Nút **"Từ chối xuất bản" (Reject - Màu đỏ):** Mở Modal bắt buộc nhập lý do từ chối (`rejection_reason`) để gửi mail cho giảng viên sửa lại.
* **Trạng thái yêu cầu:**
  * Approval Confirmation Modal: Xác nhận xuất bản.
  * Rejection Modal: Nhập lý do (TextArea có kiểm tra không để trống).

---

### SCR-ADM-03: Quản lý Cây Danh mục Đào tạo (Category Management)
* **Vai trò:** Quản trị viên.
* **Mục tiêu nghiệp vụ:** Quản lý danh mục khóa học phân cấp cha - con và tối ưu SEO menu (`F2.3`).
* **Ánh xạ CSDL:** `categories`.
* **Bố cục & Thành phần cốt lõi:**
  * Bố cục 2 phần (Cây danh mục bên trái + Form thêm/sửa bên phải):
    * Bên trái: Cây danh mục phân cấp lồng nhau (Tree view: Danh mục cha $\rightarrow$ Danh mục con kèm icon và số lượng khóa học).
    * Bên phải: Form Thêm / Cập nhật danh mục:
      * Tên danh mục (`name`).
      * Đường dẫn thân thiện (`slug`).
      * Chọn danh mục cha (`parent_id`, nếu là danh mục cấp 1 thì để trống).
      * Mã Icon (`icon`, class FontAwesome / SVG).
      * Thứ tự sắp xếp hiển thị (`order`).
      * Nút "Lưu danh mục" và "Xóa".
* **Trạng thái yêu cầu:** Tree View tương tác, hỗ trợ kéo thả hoặc click chọn danh mục để sửa.

---

### SCR-ADM-04: Quản lý Mã giảm giá (Coupon Management)
* **Vai trò:** Quản trị viên.
* **Mục tiêu nghiệp vụ:** Cấu hình và quản lý các chương trình khuyến mãi toàn hệ thống (`F2.4`).
* **Ánh xạ CSDL:** `coupons`.
* **Bố cục & Thành phần cốt lõi:**
  * Top Bar: Nút "+ Tạo mã coupon mới".
  * Bảng danh sách mã khuyến mãi:
    * Cột: Mã code (Badge in hoa nổi bật), Loại chiết khấu (% hoặc số tiền cố định), Giá trị giảm, Giới hạn sử dụng (`max_uses`), Số lượt đã dùng (`used_count`), Hạn sử dụng (`expires_at`), Trạng thái (Còn hạn / Hết hạn).
    * Thao tác: Sửa, Xóa mã.
  * Modal Tạo/Sửa Coupon: Form nhập thông tin kiểm tra ngày hết hạn phải sau ngày hiện tại.
* **Trạng thái yêu cầu:** Bảng danh sách coupon kèm filter trạng thái Còn hạn / Hết hạn.

---

### SCR-ADM-05: Quản trị Đơn hàng & Đối soát (Order & Audit Management)
* **Vai trò:** Quản trị viên.
* **Mục tiêu nghiệp vụ:** Kiểm tra lịch sử toàn bộ các giao dịch, tra cứu mã ngân hàng và lưu vết mã giảm giá áp dụng (`F2.7`).
* **Ánh xạ CSDL:** `orders`, `order_items`, `coupons`, `users`.
* **Bố cục & Thành phần cốt lõi:**
  * Bộ lọc tìm kiếm: Tìm theo Mã đơn (`order_code`), Mã tham chiếu VNPAY (`transaction_id`), Tên học viên, Lọc theo trạng thái thanh toán.
  * Bảng danh sách Đơn hàng toàn sàn:
    * Cột: Mã đơn hàng, Tên học viên & Email, Khóa học mua, Tổng tiền gốc, Mã coupon đã dùng (`coupons.code`), Số tiền thực thu (`final_amount`), Cổng thanh toán (VNPAY/MoMo), Trạng thái (`completed`, `pending`, `failed`, `refunded`), Ngày giao dịch.
    * Thao tác: Bấm xem chi tiết đơn hàng (Modal Audit Trail).
* **Trạng thái yêu cầu:** Bảng dữ liệu có phân trang và bộ lọc chính xác.

---

### SCR-ADM-06: Phê duyệt Yêu cầu Rút tiền (Payout Management)
* **Vai trò:** Quản trị viên.
* **Mục tiêu nghiệp vụ:** Đối soát tài chính, xác nhận chuyển khoản ngân hàng và cập nhật số dư ví giảng viên (`F5.2`).
* **Ánh xạ CSDL:** `instructor_payouts`, `instructor_profiles`, `users`.
* **Bố cục & Thành phần cốt lõi:**
  * Bộ lọc tab: Chờ xử lý (`pending`), Đã giải ngân (`approved`), Từ chối (`rejected`).
  * Bảng danh sách yêu cầu rút tiền:
    * Cột: Mã yêu cầu, Giảng viên yêu cầu, Số tiền muốn rút, Thông tin ngân hàng thụ hưởng (Tên NH, Số TK, Tên chủ TK), Ngày gửi đơn.
    * Cột Thao tác:
      * Nút "Xác nhận chuyển tiền": Mở Modal tải ảnh chụp ủy nhiệm chi / biên lai chuyển khoản ngân hàng (`receipt_image`), bấm hoàn tất chuyển trạng thái `approved`.
      * Nút "Từ chối": Mở Modal nhập lý do từ chối (sai thông tin tài khoản) và hoàn tiền lại vào ví giảng viên.
* **Trạng thái yêu cầu:** Payout Processing Modal kèm khu vực upload ảnh biên lai.

---

### SCR-ADM-07: Quản trị Người dùng & Phân quyền (User & Access Control)
* **Vai trò:** Quản trị viên cao cấp (Super Admin).
* **Mục tiêu nghiệp vụ:** Quản lý danh sách tài khoản học viên, giảng viên và kiểm soát trạng thái hoạt động (`F1.6`).
* **Ánh xạ CSDL:** `users`, `instructor_profiles`.
* **Bố cục & Thành phần cốt lõi:**
  * Bộ lọc: Tìm theo Tên / Email, Lọc theo Vai trò (`student`, `instructor`, `admin`), Lọc theo Trạng thái (`active`, `banned`).
  * Bảng dữ liệu người dùng:
    * Cột: Avatar, Họ tên, Email, Vai trò (Badge màu riêng biệt), Ngày tham gia, Trạng thái (Xanh: Hoạt động / Đỏ: Bị khóa).
    * Cột Thao tác: Nút "Khóa tài khoản" (Ban) hoặc "Mở khóa", Nút xem chi tiết hoạt động học tập / giảng dạy.
* **Trạng thái yêu cầu:** Bảng danh sách người dùng kèm Modal xác nhận khóa tài khoản có cảnh báo đỏ.

---

## 5. BẢNG TỔNG HỢP ÁNH XẠ MÀN HÌNH - TÍNH NĂNG - DATABASE

Bảng ma trận này xác nhận **sự đồng bộ tuyệt đối giữa Giao diện - Nghiệp vụ SRS - Cơ sở dữ liệu 22 bảng**:

| STT | Mã Màn hình | Tên Màn hình | Vai trò | Chức năng (SRS) | Bảng CSDL Tác động |
| :---: | :--- | :--- | :---: | :---: | :--- |
| 1 | `SCR-STU-01` | Trang chủ (Homepage) | Public | F1.1, F2.1 | `categories`, `courses`, `users`, `course_reviews` |
| 2 | `SCR-STU-02` | Khám phá & Bộ lọc | Public | F2.1 | `courses`, `categories`, `course_reviews` |
| 3 | `SCR-STU-03` | Chi tiết khóa học | Public | F2.2 | `courses`, `chapters`, `lessons`, `lesson_videos`, `course_reviews` |
| 4 | `SCR-STU-04` | Giỏ hàng & Thanh toán | Student | F2.4, F2.5 | `orders`, `order_items`, `coupons` |
| 5 | `SCR-STU-05` | Kết quả thanh toán | Student | F2.6 | `orders`, `enrollments` |
| 6 | `SCR-STU-06` | Khóa học của tôi | Student | F4.1 | `enrollments`, `courses`, `lesson_progress` |
| 7 | `SCR-STU-07` | Phòng học bài giảng Player | Student | F4.2, F4.3, F4.4, F4.7 | `lessons`, `chapters`, `lesson_videos`, `lesson_progress`, `lesson_notes`, `lesson_comments` |
| 8 | `SCR-STU-08` | Làm bài trắc nghiệm Quiz | Student | F4.5 | `quizzes`, `quiz_questions`, `quiz_answers`, `quiz_submissions` |
| 9 | `SCR-STU-09` | Chứng chỉ & Tra cứu QR | Public | F4.6 | `certificates`, `courses`, `users` |
| 10 | `SCR-STU-10` | Hồ sơ cá nhân & Đơn hàng | Student | F1.3, F1.4, F2.7 | `users`, `orders`, `order_items` |
| 11 | `SCR-INS-01` | Dashboard Giảng viên | Instructor | F5.1, F5.3 | `courses`, `enrollments`, `instructor_profiles` |
| 12 | `SCR-INS-02` | Thông tin & Giá khóa học | Instructor | F3.1 | `courses`, `categories` |
| 13 | `SCR-INS-03` | Trình soạn thảo Giáo trình | Instructor | F3.2, F3.3, F3.5 | `chapters`, `lessons`, `lesson_videos`, `lesson_articles` |
| 14 | `SCR-INS-04` | Trình tạo Đề thi Quiz | Instructor | F3.4 | `quizzes`, `quiz_questions`, `quiz_answers` |
| 15 | `SCR-INS-05` | Quản lý Hỏi đáp & Đánh giá | Instructor | F4.7, F4.8 | `lesson_comments`, `course_reviews` |
| 16 | `SCR-INS-06` | Ví Doanh thu & Rút tiền | Instructor | F5.1 | `instructor_profiles`, `instructor_payouts` |
| 17 | `SCR-ADM-01` | Dashboard Tổng quan Sàn | Admin | F5.4 | `orders`, `order_items`, `users`, `courses` |
| 18 | `SCR-ADM-02` | Kiểm duyệt Khóa học | Admin | F3.6 | `courses`, `chapters`, `lessons`, `lesson_videos` |
| 19 | `SCR-ADM-03` | Quản lý Cây Danh mục | Admin | F2.3 | `categories` |
| 20 | `SCR-ADM-04` | Quản lý Mã giảm giá | Admin | F2.4 | `coupons` |
| 21 | `SCR-ADM-05` | Quản trị Đơn hàng & Audit | Admin | F2.7 | `orders`, `order_items`, `coupons` |
| 22 | `SCR-ADM-06` | Phê duyệt Yêu cầu Rút tiền | Admin | F5.2 | `instructor_payouts`, `instructor_profiles` |
| 23 | `SCR-ADM-07` | Quản trị Người dùng & Khóa | Admin | F1.6 | `users` |
