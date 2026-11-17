# TÀI LIỆU ĐẶC TẢ YÊU CẦU TÍNH NĂNG HỆ THỐNG LMS (MINI-UDEMY)
**Đề tài:** Xây dựng Website Quản lý Học tập Trực tuyến (Learning Management System)  
**Công nghệ:** Laravel Framework (PHP) & MySQL  
**Phạm vi:** Tài liệu cơ sở (Single Source of Truth - SSOT) phục vụ xây dựng Sơ đồ BFD, Đặc tả Use Case chi tiết, Sơ đồ Hoạt động (Activity Diagram), Sơ đồ Tuần tự (Sequence Diagram), Yêu cầu Phi chức năng và hiện thực hóa trên Cơ sở dữ liệu 22 bảng đã chuẩn hóa.

---

## MỤC LỤC
1. [CẤU TRÚC PHÂN RÃ CHỨC NĂNG TỔNG THỂ (BFD TREE)](#1-cấu-trúc-phân-rã-chức-năng-tổng-thể-bfd-tree)
2. [DANH MỤC BẢNG ĐẶC TẢ TÍNH NĂNG THEO PHÂN HỆ](#2-danh-mục-bảng-đặc-tả-tính-năng-theo-phân-hệ)
   - [Phân hệ 1 (F1): Xác thực, Người dùng & Hồ sơ Cá nhân](#phân-hệ-1-f1-xác-thực-người-dùng--hồ-sơ-cá-nhân)
   - [Phân hệ 2 (F2): Khám phá, Đơn hàng & Thanh toán Trực tuyến](#phân-hệ-2-f2-khám-phá-đơn-hàng--thanh-toán-trực-tuyến)
   - [Phân hệ 3 (F3): Quản lý & Biên soạn Nội dung Đào tạo](#phân-hệ-3-f3-quản-lý--biên-soạn-nội-dung-đào-tạo)
   - [Phân hệ 4 (F4): Không gian Học tập, Đánh giá & Tương tác (Core)](#phân-hệ-4-f4-không-gian-học-tập-đánh-giá--tương-tác-core)
   - [Phân hệ 5 (F5): Báo cáo Thống kê & Quản trị Tài chính](#phân-hệ-5-f5-báo-cáo-thống-kê--quản-trị-tài-chính)
3. [MA TRẬN TRUY VẾT TÍNH NĂNG VÀ CƠ SỞ DỮ LIỆU (TRACEABILITY MATRIX)](#3-ma-trận-truy-vết-tính-năng-và-cơ-sở-dữ-liệu-traceability-matrix)
4. [YÊU CẦU PHI CHỨC NĂNG (NON-FUNCTIONAL REQUIREMENTS - NFR)](#4-yêu-cầu-phi-chức-năng-non-functional-requirements---nfr)
   - [4.1. Hiệu năng & Khả năng Tải (Performance & Scalability)](#41-hiệu-năng--khả-năng-tải-performance--scalability)
   - [4.2. An toàn & Bảo mật Thông tin (Security & Authorization)](#42-an-toàn--bảo-mật-thông-tin-security--authorization)
   - [4.3. Tính Toàn vẹn & Độ tin cậy (Reliability & Integrity)](#43-tính-toàn-vẹn--độ-tin-cậy-reliability--integrity)
   - [4.4. Trải nghiệm & Khả năng Sử dụng (Usability & UX/UI)](#44-trải-nghiệm--khả-năng-sử-dụng-usability--uxui)
   - [4.5. Khả năng Bảo trì & Mở rộng Mã nguồn (Maintainability & Clean Architecture)](#45-khả-năng-bảo-trì--mở-rộng-mã-nguồn-maintainability--clean-architecture)
   - [4.6. Tính Tương thích Môi trường (Compatibility)](#46-tính-tương-thích-môi-trường-compatibility)
5. [HƯỚNG DẪN KẾ THỪA CHO CÁC MÔ HÌNH THIẾT KẾ TIẾP THEO](#5-hướng-dẫn-kế-thừa-cho-các-mô-hình-thiết-kế-tiếp-theo)

---

## 1. CẤU TRÚC PHÂN RÃ CHỨC NĂNG TỔNG THỂ (BFD TREE)

Cây phân rã chức năng (Business Function Diagram - BFD) được chia thành **5 Phân hệ chính** với **28 chức năng thành phần**, bao quát toàn bộ hoạt động của 4 tác nhân: **Khách (Guest)**, **Học viên (Student)**, **Giảng viên (Instructor)** và **Quản trị viên (Admin)**.

```
HỆ THỐNG QUẢN LÝ HỌC TẬP (LMS)
│
├── [F1] PHÂN HỆ XÁC THỰC & NGƯỜI DÙNG
│   ├── F1.1: Đăng ký tài khoản học viên
│   ├── F1.2: Đăng nhập & Xác thực hệ thống
│   ├── F1.3: Quản lý thông tin hồ sơ cá nhân
│   ├── F1.4: Đăng ký trở thành giảng viên
│   ├── F1.5: Cấu hình hồ sơ giảng viên & Tài khoản nhận tiền
│   └── F1.6: Quản lý & Khóa/Mở khóa tài khoản người dùng
│
├── [F2] PHÂN HỆ KHÁM PHÁ & THƯƠNG MẠI
│   ├── F2.1: Tìm kiếm & Lọc khóa học đa tiêu chí
│   ├── F2.2: Xem chi tiết khóa học & Học thử miễn phí
│   ├── F2.3: Quản lý Cây danh mục khóa học đa cấp
│   ├── F2.4: Quản lý & Kiểm tra mã giảm giá (Coupon)
│   ├── F2.5: Đặt hàng & Khởi tạo giao dịch thanh toán
│   ├── F2.6: Xử lý Webhook (IPN) & Kích hoạt ghi danh tự động
│   └── F2.7: Tra cứu đơn hàng & Lịch sử giao dịch
│
├── [F3] PHÂN HỆ BIÊN SOẠN & KIỂM DUYỆT KHÓA HỌC
│   ├── F3.1: Quản lý thông tin cơ bản & Định giá khóa học
│   ├── F3.2: Quản lý cấu trúc Chương học (Chapters)
│   ├── F3.3: Quản lý Bài giảng (Video & Bài đọc Article)
│   ├── F3.4: Xây dựng Ngân hàng câu hỏi & Đề thi trắc nghiệm (Quiz)
│   ├── F3.5: Gửi yêu cầu phê duyệt khóa học (Submit for Review)
│   └── F3.6: Kiểm duyệt nội dung & Xuất bản khóa học
│
├── [F4] PHÂN HỆ KHÔNG GIAN HỌC TẬP & TƯƠNG TÁC (CORE)
│   ├── F4.1: Quản lý danh sách khóa học của tôi (My Learning)
│   ├── F4.2: Trình phát video đa phương tiện & Resume Playback
│   ├── F4.3: Điều khiển mở khóa học tuần tự (Sequential Engine)
│   ├── F4.4: Tạo & Điều hướng ghi chú video theo Timestamp
│   ├── F4.5: Làm bài kiểm tra trắc nghiệm & Chấm điểm tự động
│   ├── F4.6: Cấp chứng chỉ điện tử PDF & Tra cứu xác thực QR
│   ├── F4.7: Thảo luận hỏi đáp đa tầng dưới bài học (Nested Q&A)
│   └── F4.8: Đánh giá số sao & Phản hồi nhận xét khóa học
│
└── [F5] PHÂN HỆ BÁO CÁO THỐNG KÊ & TÀI CHÍNH
    ├── F5.1: Quản lý ví doanh thu & Lập yêu cầu rút tiền
    ├── F5.2: Phê duyệt yêu cầu rút tiền & Đối soát tài chính
    ├── F5.3: Thống kê tiến độ học tập & Doanh thu theo khóa
    └── F5.4: Dashboard thống kê KPI & Báo cáo tổng thể hệ thống
```

---

## 2. DANH MỤC BẢNG ĐẶC TẢ TÍNH NĂNG THEO PHÂN HỆ

---

### PHÂN HỆ 1 (F1): XÁC THỰC, NGƯỜI DÙNG & HỒ SƠ CÁ NHÂN

| Mã CN | Tên Chức năng | Tác nhân | Mô tả Chi tiết Nghiệp vụ & Xử lý Hệ thống | Bảng CSDL Tác động | Ưu tiên |
| :---: | :--- | :---: | :--- | :--- | :---: |
| **F1.1** | Đăng ký tài khoản | Khách (Guest) | Tiếp nhận Họ tên, Email, Mật khẩu. Kiểm tra tính hợp lệ của định dạng email, mật khẩu tối thiểu 8 ký tự, xác nhận email chưa từng tồn tại trên hệ thống. Mã hóa mật khẩu bằng thuật toán Bcrypt và tạo tài khoản với vai trò mặc định là `student`. Gửi mail chào mừng qua Queue. | `users` (Insert) | **Must-Have** |
| **F1.2** | Đăng nhập & Đăng xuất | Khách, Người dùng | Xác thực thông tin qua Email và Mật khẩu. Hỗ trợ ghi nhớ đăng nhập (`remember_token`). Kiểm tra trạng thái tài khoản: nếu `status = 'banned'` thì chặn truy cập và thông báo lý do. Cấp Session/Token đăng nhập thành công; hỗ trợ tính năng Hủy phiên đăng xuất an toàn. | `users` (Read, Update) | **Must-Have** |
| **F1.3** | Quản lý hồ sơ cá nhân | Người dùng | Cho phép cập nhật thông tin: Họ tên, tải lên/thay đổi ảnh đại diện (`avatar`), đổi mật khẩu (yêu cầu xác minh mật khẩu cũ chính xác). | `users` (Update) | **Must-Have** |
| **F1.4** | Đăng ký làm Giảng viên | Học viên (Student) | Học viên điền thông tin xin cấp quyền giảng dạy: Tiêu đề chuyên môn, tiểu sử, số tài khoản ngân hàng. Hệ thống chuyển đổi vai trò tài khoản thành `instructor` và khởi tạo bản ghi hồ sơ chuyên môn kèm ví tài chính. | `users` (Update), `instructor_profiles` (Insert) | **Must-Have** |
| **F1.5** | Cấu hình hồ sơ Giảng viên | Giảng viên | Cập nhật chức danh nghề nghiệp (`headline`), tiểu sử kinh nghiệm (`bio`), cấu hình tài khoản thụ hưởng thanh toán gồm tên ngân hàng, số tài khoản và tên chủ thẻ phục vụ nhận tiền rút. | `instructor_profiles` (Update) | **Must-Have** |
| **F1.6** | Quản lý & Phân quyền người dùng | Quản trị viên (Admin) | Xem danh sách người dùng, lọc theo vai trò (`student`, `instructor`, `admin`) hoặc trạng thái (`active`, `banned`). Thực hiện khóa tài khoản vi phạm hoặc mở khóa tài khoản; cấp quyền quản trị viên phụ. | `users` (Read, Update) | **Must-Have** |

---

### PHÂN HỆ 2 (F2): KHÁM PHÁ, ĐƠN HÀNG & THANH TOÁN TRỰC TUYẾN

| Mã CN | Tên Chức năng | Tác nhân | Mô tả Chi tiết Nghiệp vụ & Xử lý Hệ thống | Bảng CSDL Tác động | Ưu tiên |
| :---: | :--- | :---: | :--- | :--- | :---: |
| **F2.1** | Tìm kiếm & Lọc khóa học | Khách, Học viên | Tìm kiếm theo từ khóa trong tiêu đề/mô tả khóa học; kết hợp bộ lọc đa chiều: theo Danh mục, mức giá (Miễn phí/Có phí), cấp độ (`beginner`, `intermediate`, `advanced`, `all`), sắp xếp theo mới nhất, đánh giá cao nhất hoặc bán chạy nhất. Chỉ hiển thị các khóa học có trạng thái `status = 'published'`. | `courses`, `categories` (Read) | **Must-Have** |
| **F2.2** | Xem chi tiết & Học thử miễn phí | Khách, Học viên | Hiển thị Trang giới thiệu khóa học: Mục tiêu học tập, yêu cầu, tổng thời lượng, số bài học, video trailer giới thiệu, giáo trình chi tiết và danh sách đánh giá sao. Cho phép người dùng bấm xem trực tiếp nội dung các bài học có đánh dấu `is_free_preview = TRUE` mà không cần mua khóa học. | `courses`, `chapters`, `lessons`, `lesson_videos`, `course_reviews` (Read) | **Must-Have** |
| **F2.3** | Quản lý Danh mục khóa học đa cấp | Admin | Quản lý cây danh mục đào tạo (hỗ trợ danh mục cha - con thông qua `parent_id`): Thêm mới danh mục, cập nhật tên, tự động sinh slug SEO, gán mã icon hiển thị và sắp xếp thứ tự hiển thị (`order`). | `categories` (CRUD) | **Must-Have** |
| **F2.4** | Quản lý & Kiểm tra mã giảm giá | Admin, Học viên | • Admin: Tạo mã khuyến mãi (`code`), loại chiết khấu (% hoặc số tiền cố định), giá trị giảm, hạn sử dụng và số lượt dùng tối đa.<br>• Học viên: Nhập mã tại trang Checkout. Hệ thống kiểm tra hợp lệ: còn hạn sử dụng, chưa vượt `max_uses`. Nếu thỏa mãn, áp dụng tính lại `discount_amount` và `final_amount`. | `coupons` (CRUD, Update `used_count`) | **Should-Have** |
| **F2.5** | Đặt hàng & Khởi tạo thanh toán | Học viên | Kiểm tra điều kiện: Học viên chưa từng sở hữu khóa học (`enrollments`) và không phải là tác giả khóa học. Tạo bản ghi đơn hàng (`orders`) với trạng thái `pending`, lưu mã `coupon_id` (nếu có áp dụng mã hợp lệ) và chi tiết giá khóa học vào `order_items`. Nếu đơn hàng có giá trị $0$ (khóa học miễn phí), chuyển thẳng sang trạng thái `completed`. Nếu có phí, hệ thống sinh mã chữ ký số (Checksum HMAC-SHA512) và chuyển hướng học viên sang Cổng thanh toán VNPAY/MoMo. | `orders` (Insert kèm `coupon_id`), `order_items` (Insert) | **Must-Have** |
| **F2.6** | Xử lý Webhook (IPN) & Kích hoạt ghi danh | Hệ thống, Cổng TT (VNPAY) | Tiếp nhận phản hồi ngầm (Instant Payment Notification) từ cổng thanh toán. Kiểm tra xác thực chữ ký bảo mật. Nếu giao dịch thành công: cập nhật `orders.payment_status = 'completed'`, tăng `coupons.used_count` (nếu đơn hàng có áp dụng mã `coupon_id`), lưu `transaction_id`, tự động tạo bản ghi trong bảng `enrollments` cấp quyền vào học cho học viên, cộng $70\%$ doanh thu vào ví giảng viên (`wallet_balance`), và đẩy Job gửi email hóa đơn điện tử vào Queue. | `orders` (Update), `coupons` (Update `used_count`), `enrollments` (Insert), `instructor_profiles` (Update) | **Must-Have** |
| **F2.7** | Tra cứu đơn hàng & Lịch sử giao dịch | Học viên, Admin | • Học viên: Xem danh sách các đơn hàng cá nhân đã thanh toán, ngày mua, giá tiền và trạng thái giao dịch.<br>• Admin: Xem toàn bộ giao dịch trên toàn hệ thống, lọc theo ngày/trạng thái/mã đối soát ngân hàng. | `orders`, `order_items`, `courses` (Read) | **Must-Have** |

---

### PHÂN HỆ 3 (F3): QUẢN LÝ & BIÊN SOẠN NỘI DUNG ĐÀO TẠO

| Mã CN | Tên Chức năng | Tác nhân | Mô tả Chi tiết Nghiệp vụ & Xử lý Hệ thống | Bảng CSDL Tác động | Ưu tiên |
| :---: | :--- | :---: | :--- | :--- | :---: |
| **F3.1** | Quản lý thông tin & Định giá khóa học | Giảng viên | Thêm mới hoặc chỉnh sửa khóa học: Nhập tiêu đề, tóm tắt, mô tả chi tiết (WYSIWYG/Markdown), chọn danh mục, chọn cấp độ, tải ảnh đại diện (`thumbnail`), video giới thiệu (`promo_video_url`), thiết lập giá gốc và giá bán khuyến mãi. Trạng thái khởi tạo mặc định là `draft`. | `courses` (CRUD) | **Must-Have** |
| **F3.2** | Quản lý cấu trúc Chương học | Giảng viên | Quản lý phân đoạn nội dung cấp 1 trong khóa học: Thêm chương mới, sửa tên chương, xóa chương, thiết lập chỉ số thứ tự (`order`) để bài giảng được hiển thị tuần tự. | `chapters` (CRUD) | **Must-Have** |
| **F3.3** | Quản lý Bài học (Video & Article) | Giảng viên | Thêm bài học mới trực thuộc chương: Đặt tiêu đề, chọn định dạng (`video` hoặc `article`), chỉ số thứ tự và bật/tắt cờ học thử (`is_free_preview`).<br>• Nếu là `video`: Lưu liên kết/upload video và tổng thời lượng (`duration_seconds`).<br>• Nếu là `article`: Soạn thảo nội dung văn bản kèm code, hình ảnh vào `lesson_articles`. | `lessons` (CRUD), `lesson_videos` (CRUD), `lesson_articles` (CRUD) | **Must-Have** |
| **F3.4** | Xây dựng Ngân hàng câu hỏi & Bài thi Quiz | Giảng viên | Tạo bài kiểm tra trắc nghiệm gán với bài học loại `quiz`: Cấu hình tỷ lệ % điểm đạt (`pass_percentage`), thời gian làm bài (`time_limit_minutes`). Thêm danh sách câu hỏi (`quiz_questions`), phần giải thích đáp án và các lựa chọn trả lời (`quiz_answers`) kèm cờ đánh dấu đáp án đúng (`is_correct`). | `quizzes` (CRUD), `quiz_questions` (CRUD), `quiz_answers` (CRUD) | **Must-Have** |
| **F3.5** | Gửi yêu cầu duyệt khóa học | Giảng viên | Kiểm tra danh mục kiểm tra chất lượng tối thiểu: Phải có ít nhất 1 chương, ít nhất 1 bài học hoàn chỉnh và ảnh bìa hợp lệ. Chuyển trạng thái khóa học từ `draft` hoặc `rejected` sang `pending`. Khóa quyền chỉnh sửa cấu trúc quan trọng trong thời gian chờ duyệt. | `courses` (Update `status = 'pending'`) | **Must-Have** |
| **F3.6** | Kiểm duyệt & Xuất bản khóa học | Admin | Xem danh sách các khóa học chờ duyệt. Quản trị viên có màn hình xem thử toàn bộ nội dung giáo trình, video và bài tập trắc nghiệm.<br>• Phê duyệt (Approve): Cập nhật `status = 'published'`, khóa học chính thức xuất hiện trên sàn; gửi mail chúc mừng.<br>• Từ chối (Reject): Bắt buộc nhập lý do chi tiết vào `rejection_reason` và chuyển `status = 'rejected'` để giảng viên sửa lại. | `courses` (Update `status`, `rejection_reason`) | **Must-Have** |

---

### PHÂN HỆ 4 (F4): KHÔNG GIAN HỌC TẬP, ĐÁNH GIÁ & TƯƠNG TÁC (CORE)

| Mã CN | Tên Chức năng | Tác nhân | Mô tả Chi tiết Nghiệp vụ & Xử lý Hệ thống | Bảng CSDL Tác động | Ưu tiên |
| :---: | :--- | :---: | :--- | :--- | :---: |
| **F4.1** | Quản lý khóa học của tôi (My Learning) | Học viên | Bảng điều khiển cá nhân hiển thị tất cả các khóa học đã ghi danh (`enrollments`). Hiển thị thanh tiến độ phần trăm hoàn thành, tổng số bài đã học / tổng số bài, nút bấm "Tiếp tục học" dẫn thẳng vào bài học đang học dở gần nhất. | `enrollments`, `courses`, `lesson_progress` (Read) | **Must-Have** |
| **F4.2** | Trình phát bài giảng & Resume Playback | Học viên | Trình phát video chuyên nghiệp: Cho phép chỉnh tốc độ ($0.75x, 1x, 1.25x, 1.5x, 2x$), bật toàn màn hình, chuyển bài trước/sau. Cứ mỗi 5-10 giây hoặc khi tạm dừng, JavaScript gửi beacon AJAX cập nhật số giây dừng xem (`last_watch_second`) vào database. Khi học viên quay lại học, video tự động nhảy đến đúng giây đó để phát tiếp. | `lesson_progress` (Insert/Update `last_watch_second`) | **Must-Have** |
| **F4.3** | Mở khóa học tuần tự (Sequential Engine) | Hệ thống, Học viên | Cơ chế quản lý học tập nghiêm ngặt (theo mô hình F8): Học viên chỉ được mở khóa bài học $N+1$ khi bài học $N$ đã đạt cờ `is_completed = TRUE` (xem $\ge 80\%$ thời lượng video hoặc vượt qua bài Quiz). Danh sách bài học bên thanh bên (Sidebar) hiển thị trực quan các bài đã xong (icon xanh), bài đang học và các bài chưa mở (icon ổ khóa xám). | `lesson_progress` (Read, Update `is_completed`) | **Must-Have** |
| **F4.4** | Tạo & Điều hướng ghi chú theo Timestamp | Học viên | Khi xem video, học viên bấm "Tạo ghi chú": Trình phát tự động tạm dừng, lấy mốc giây hiện tại (`timestamp_second`), học viên nhập nội dung và bấm lưu. Danh sách ghi chú hiển thị ở tab bên cạnh kèm mốc thời gian dạng `MM:SS`. Khi nhấp vào ghi chú bất kỳ, trình phát tự động tua đến đúng giây đó và phát video. | `lesson_notes` (CRUD) | **Should-Have (Điểm cộng)** |
| **F4.5** | Làm bài kiểm tra Quiz & Chấm điểm tự động | Học viên | Học viên thực hiện bài trắc nghiệm: Đếm ngược thời gian nếu có cài đặt `time_limit_minutes`. Khi bấm nộp bài, hệ thống so sánh các đáp án chọn với `quiz_answers.is_correct`, tính điểm số theo thang $100\%$. Nếu điểm $\ge pass\_percentage$, cập nhật `is_passed = TRUE` và tự động đánh dấu hoàn thành bài học để mở bài tiếp. Hiển thị giải thích chi tiết câu trả lời. | `quiz_submissions` (Insert), `lesson_progress` (Update) | **Must-Have** |
| **F4.6** | Cấp chứng chỉ PDF & Tra cứu xác thực QR | Học viên, Khách | Khi tất cả bài học trong khóa đều có `is_completed = TRUE`, hệ thống tự động sinh một mã định danh ngẫu nhiên không trùng lặp (`certificate_code` dạng UUID), kết xuất file chứng chỉ PDF chính quy bằng `dompdf` kèm mã QR code. Bất kỳ ai (nhà tuyển dụng, bạn bè) quét mã QR hoặc truy cập đường dẫn tra cứu đều xem được trang xác minh tính hợp lệ của văn bằng. | `certificates` (Insert, Read), `enrollments` (Update `completed_at`) | **Must-Have** |
| **F4.7** | Thảo luận hỏi đáp đa tầng (Nested Q&A) | Học viên, Giảng viên | Khu vực thảo luận ngay dưới bài học: Cho phép học viên đăng câu hỏi (hỗ trợ định dạng code markdown). Học viên khác hoặc giảng viên có thể nhấn "Trả lời" dưới từng bình luận cụ thể (lưu vết qua `parent_id` để tạo cây phân cấp trao đổi đa tầng). | `lesson_comments` (CRUD) | **Should-Have** |
| **F4.8** | Đánh giá & Phản hồi chất lượng khóa học | Học viên, Giảng viên | • Học viên: Đánh giá số sao từ 1 đến 5 sao và viết nhận xét chi tiết sau khi đã ghi danh và học được ít nhất $30\%$ tiến độ (ràng buộc `UNIQUE(user_id, course_id)` ngăn đánh giá nhiều lần).<br>• Giảng viên: Xem danh sách đánh giá của học viên và viết nội dung phản hồi công khai (`instructor_reply`). | `course_reviews` (CRUD) | **Must-Have** |

---

### PHÂN HỆ 5 (F5): BÁO CÁO THỐNG KÊ & TÀI CHÍNH

| Mã CN | Tên Chức năng | Tác nhân | Mô tả Chi tiết Nghiệp vụ & Xử lý Hệ thống | Bảng CSDL Tác động | Ưu tiên |
| :---: | :--- | :---: | :--- | :--- | :---: |
| **F5.1** | Quản lý ví & Yêu cầu rút tiền | Giảng viên | Xem số dư khả dụng (`wallet_balance`), số tiền đang chờ xử lý và lịch sử các lần rút tiền. Khi số dư đạt ngưỡng tối thiểu quy định (VD: $500,000$ VNĐ), giảng viên nhập số tiền muốn rút và gửi yêu cầu giải ngân (`status = 'pending'`). | `instructor_profiles` (Read), `instructor_payouts` (Insert) | **Must-Have** |
| **F5.2** | Duyệt yêu cầu rút tiền & Đối soát tài chính | Admin | Xem danh sách các yêu cầu rút tiền của giảng viên, thông tin số tài khoản và ngân hàng thụ hưởng. Sau khi chuyển khoản ngoài thực tế, Admin tải ảnh chụp biên lai giao dịch (`receipt_image`) lên hệ thống, cập nhật trạng thái `approved` và trừ số dư ví của giảng viên. Nếu từ chối, nhập lý do vào `note` và hoàn trả số dư ví. | `instructor_payouts` (Update), `instructor_profiles` (Update `wallet_balance`) | **Must-Have** |
| **F5.3** | Báo cáo hiệu suất khóa học & Học viên | Giảng viên | Thống kê số lượng học viên đã đăng ký theo từng khóa, tổng doanh thu thực nhận của từng khóa học, điểm đánh giá trung bình và danh sách học viên đang theo học kèm phần trăm tiến độ cụ thể. | `courses`, `enrollments`, `order_items`, `lesson_progress` (Read) | **Should-Have** |
| **F5.4** | Dashboard thống kê KPI & Báo cáo hệ thống | Admin | Bảng điều khiển quản trị trực quan (tích hợp biểu đồ Chart.js): Thống kê tổng doanh thu toàn sàn, lợi nhuận thực thu của sàn ($30\%$), tổng số học viên đăng ký mới, số khóa học xuất bản, biểu đồ tăng trưởng doanh thu theo tháng và danh sách Top 5 khóa học bán chạy nhất. | `orders`, `order_items`, `users`, `courses`, `enrollments` (Read) | **Must-Have** |

---

## 3. MA TRẬN TRUY VẾT TÍNH NĂNG VÀ CƠ SỞ DỮ LIỆU (TRACEABILITY MATRIX)

Bảng ma trận dưới đây chứng minh tính khả thi kỹ thuật tuyệt đối: **Toàn bộ 22 bảng CSDL đã thiết kế đều được sử dụng và bao quát trọn vẹn trong 28 chức năng hệ thống**.

| STT | Tên Bảng CSDL (22 bảng) | Các Chức năng Tác động (CRUD) | Vai trò trong Hệ thống |
| :---: | :--- | :--- | :--- |
| 1 | `users` | F1.1, F1.2, F1.3, F1.4, F1.6, F5.4 | Quản lý định danh và phân quyền người dùng |
| 2 | `instructor_profiles` | F1.4, F1.5, F2.6, F5.1, F5.2 | Hồ sơ chuyên gia, ví doanh thu và tài khoản ngân hàng |
| 3 | `categories` | F2.1, F2.3, F3.1 | Phân loại danh mục đào tạo đa cấp |
| 4 | `courses` | F2.1, F2.2, F3.1, F3.5, F3.6, F5.3, F5.4 | Thực thể trung tâm lưu trữ thông tin khóa học và vòng đời duyệt |
| 5 | `chapters` | F2.2, F3.2, F4.2, F4.3 | Phân cấp chương học |
| 6 | `lessons` | F2.2, F3.3, F4.2, F4.3 | Phân cấp bài học và cờ học thử miễn phí |
| 7 | `lesson_videos` | F2.2, F3.3, F4.2 | Lưu trữ thông tin kỹ thuật và thời lượng video |
| 8 | `lesson_articles` | F3.3, F4.2 | Lưu trữ nội dung bài học lý thuyết văn bản |
| 9 | `quizzes` | F3.4, F4.5 | Quy chế bài thi trắc nghiệm (điểm đạt, thời gian làm bài) |
| 10 | `quiz_questions` | F3.4, F4.5 | Ngân hàng đề thi trắc nghiệm |
| 11 | `quiz_answers` | F3.4, F4.5 | Các đáp án lựa chọn và cờ đáp án đúng |
| 12 | `quiz_submissions` | F4.5 | Lịch sử làm bài thi, điểm số và kết quả Đạt/Trượt |
| 13 | `enrollments` | F2.5, F2.6, F4.1, F4.6, F5.3, F5.4 | Quyền sở hữu khóa học và mốc hoàn thành khóa |
| 14 | `lesson_progress` | F4.1, F4.2, F4.3, F4.5, F5.3 | Hạt nhân điều khiển mở bài tuần tự và vị trí dừng video (Resume) |
| 15 | `lesson_notes` | F4.4 | Lưu trữ các ghi chú video gắn với mốc thời gian Timestamp |
| 16 | `certificates` | F4.6 | Chứng chỉ điện tử và mã tra cứu công khai QR |
| 17 | `coupons` | F2.4, F2.5, F2.6 | Mã khuyến mãi giảm giá, liên kết đơn hàng và theo dõi số lượt sử dụng |
| 18 | `orders` | F2.5, F2.6, F2.7, F5.4 | Hóa đơn giao dịch, lưu vết `coupon_id` và tích hợp cổng thanh toán |
| 19 | `order_items` | F2.5, F2.7, F5.3, F5.4 | Lưu giá lịch sử khóa học tại thời điểm thanh toán |
| 20 | `instructor_payouts` | F5.1, F5.2 | Yêu cầu và biên lai đối soát rút tiền của giảng viên |
| 21 | `course_reviews` | F2.2, F4.8 | Đánh giá sao và nhận xét từ học viên |
| 22 | `lesson_comments` | F4.7 | Thảo luận và hỏi đáp đa tầng lồng nhau dưới bài giảng |

---

## 4. YÊU CẦU PHI CHỨC NĂNG (NON-FUNCTIONAL REQUIREMENTS - NFR)

Các yêu cầu phi chức năng được xây dựng bám sát tiêu chuẩn chất lượng phần mềm quốc tế **ISO/IEC 25010**, xác định rõ các chỉ số định lượng và giải pháp kỹ thuật tương ứng trên nền tảng **Laravel & MySQL**:

```
                       CÁC TRỤ CỘT PHI CHỨC NĂNG (ISO/IEC 25010)
  ┌───────────────────────┬───────────────────────┬───────────────────────┐
  │ 1. HIỆU NĂNG          │ 2. AN TOÀN & BẢO MẬT  │ 3. TIN CẬY & TOÀN VẸN │
  │    (Performance)      │    (Security)         │    (Reliability)      │
  ├───────────────────────┼───────────────────────┼───────────────────────┤
  │ 4. TRẢI NGHIỆM        │ 5. BẢO TRÌ & MỞ RỘNG  │ 6. TÍNH TƯƠNG THÍCH   │
  │    (Usability & UX)   │    (Maintainability)  │    (Compatibility)    │
  └───────────────────────┴───────────────────────┴───────────────────────┘
```

---

### 4.1. Hiệu năng & Khả năng Tải (Performance & Scalability)

| Mã YC | Tiêu chí đánh giá | Chỉ số Định lượng Mục tiêu | Giải pháp Kỹ thuật Triển khai trong Laravel & MySQL |
| :---: | :--- | :--- | :--- |
| **NFR-01** | Thời gian phản hồi trang (Page Response Time) | $\le 2.0$ giây đối với các trang danh mục, trang chi tiết; $\le 1.0$ giây đối với các thao tác AJAX/API nội bộ. | • Sử dụng kỹ thuật Eager Loading (`with(['chapters.lessons'])`) trong Eloquent ORM nhằm triệt tiêu hoàn toàn vấn đề $N+1$ Query.<br>• Đánh chỉ mục (`INDEX`) trên các cột tìm kiếm và khóa ngoại thường xuyên lọc (`category_id`, `status`, `slug`, `user_id`). |
| **NFR-02** | Khả năng phát video bài giảng mượt mà | Video bắt đầu phát dưới $1.5$ giây, không giật lag khi chuyển bài. | Tận dụng CDN / lưu trữ đám mây (AWS S3, Cloudinary hoặc nhúng Vimeo/YouTube HLS) để phân tải băng thông máy chủ chính. |
| **NFR-03** | Khả năng xử lý tác vụ nền (Background Processing) | Thao tác bấm thanh toán và hoàn tất bài học phản hồi ngay lập tức cho người dùng, không bị nghẽn bởi việc gửi mail hay sinh PDF. | Đưa tác vụ gửi Email thông báo hóa đơn và Render file PDF chứng chỉ vào hàng đợi ngầm (**Laravel Queue & Worker** với Database Driver hoặc Redis Driver). |
| **NFR-04** | Tần suất lưu tiến độ học tập (Progress Beacon) | Không gây quá tải server khi hàng trăm học viên cùng xem video một lúc. | Phía client dùng JavaScript Throttle/Debounce: Chỉ gửi request lưu vị trí giây phát (`last_watch_second`) mỗi 10 giây/lần hoặc khi sự kiện `pause` / `beforeunload` diễn ra. |

---

### 4.2. An toàn & Bảo mật Thông tin (Security & Authorization)

| Mã YC | Tiêu chí đánh giá | Tiêu chuẩn Đạt được | Giải pháp Kỹ thuật Triển khai trong Laravel |
| :---: | :--- | :--- | :--- |
| **NFR-05** | Mã hóa mật khẩu người dùng | Mật khẩu không bao giờ lưu dưới dạng văn bản thô (Plain text). | Sử dụng cơ chế băm mật khẩu chuẩn công nghiệp **Bcrypt** (`Hash::make()`) với hệ số work factor mặc định của Laravel. |
| **NFR-06** | Phòng chống các lỗ hổng Web phổ biến (OWASP Top 10) | Triệt tiêu nguy cơ tấn công SQL Injection, Cross-Site Scripting (XSS), và CSRF. | • **Chống SQLi:** 100% truy vấn cơ sở dữ liệu qua Eloquent ORM và Query Builder sử dụng cơ chế Prepared Statements (PDO Parameter Binding).<br>• **Chống CSRF:** Mọi form HTML và request POST/PUT/DELETE bắt buộc phải có `@csrf` token xác thực.<br>• **Chống XSS:** Blade Template tự động escape ký tự HTML bằng thẻ `{{ $data }}`. Riêng nội dung bài giảng rich text phải qua bộ lọc HTMLPurifier. |
| **NFR-07** | Bảo mật giao dịch cổng thanh toán | Chống gian lận thay đổi số tiền hoặc giả mạo kết quả thanh toán từ cổng ngoài. | • Áp dụng mã hóa băm chữ ký điện tử **HMAC-SHA512** đối chiếu giữa dữ liệu gửi sang VNPAY và dữ liệu nhận về qua IPN Webhook.<br>• Kiểm tra số tiền trả về từ ngân hàng phải khớp đúng với `orders.final_amount` trước khi cấp quyền ghi danh. |
| **NFR-08** | Phân quyền truy cập tài nguyên (Authorization & RBAC) | Học viên không thể xem bài học chưa mua; Giảng viên chỉ sửa được khóa học của chính mình. | Sử dụng **Laravel Policies / Gates** (`CoursePolicy`, `LessonPolicy`) để kiểm tra quyền sở hữu và quyền truy cập trước khi thực thi Controller Action. |
| **NFR-09** | Giới hạn tần suất request (Rate Limiting) | Ngăn chặn tấn công Brute-Force mật khẩu và spam bình luận/đơn hàng. | Kích hoạt middleware `throttle:60,1` (tối đa 60 request/phút) và `throttle:5,1` đối với endpoint Đăng nhập. |

---

### 4.3. Tính Toàn vẹn & Độ tin cậy (Reliability & Integrity)

| Mã YC | Tiêu chí đánh giá | Mục tiêu | Giải pháp Kỹ thuật Triển khai |
| :---: | :--- | :--- | :--- |
| **NFR-10** | Tính nguyên tử trong giao dịch tài chính (ACID) | Không bao giờ xảy ra tình trạng: Trừ tiền thành công nhưng không tạo được ghi danh, hoặc ví giảng viên không nhận được tiền. | Sử dụng cơ chế Transaction cơ sở dữ liệu: `DB::transaction(function () { ... })`. Nếu có bất kỳ bước nào phát sinh lỗi, toàn bộ dữ liệu sẽ tự động Rollback về trạng thái ban đầu. |
| **NFR-11** | Tính duy nhất của việc ghi danh (Double Spending / Enrollment) | Một học viên không thể mua trùng một khóa học 2 lần. | Thiết lập chỉ mục duy nhất `UNIQUE KEY (user_id, course_id)` trên bảng `enrollments`, kết hợp kiểm tra tiền điều kiện ở tầng nghiệp vụ. |
| **NFR-12** | Xử lý lỗi mềm và Nhật ký hệ thống (Graceful Error Handling & Logging) | Không để lộ thông tin nhạy cảm của hệ thống (Database Schema, Stack Trace) ra màn hình người dùng khi gặp sự cố. | Bật chế độ `APP_DEBUG=false` trên môi trường triển khai; cấu hình trang lỗi thân thiện (`404.blade.php`, `500.blade.php`); toàn bộ ngoại lệ lỗi được ghi nhận chi tiết vào file log thông qua Monolog (`storage/logs/laravel.log`). |

---

### 4.4. Trải nghiệm & Khả năng Sử dụng (Usability & UX/UI)

| Mã YC | Tiêu chí đánh giá | Tiêu chuẩn Trải nghiệm | Giải pháp Thiết kế Giao diện |
| :---: | :--- | :--- | :--- |
| **NFR-13** | Thiết kế tương thích đa thiết bị (Responsive Web Design) | Hiển thị tối ưu và liền mạch trên các kích thước màn hình phổ biến: Màn hình máy tính (Desktop $\ge 1200px$), Máy tính bảng (Tablet $768px - 1024px$) và Điện thoại di động (Mobile $\le 767px$). | Xây dựng giao diện dựa trên hệ thống CSS hiện đại (Bootstrap 5 / Tailwind CSS), thanh bên danh sách bài học tự động thu gọn dạng Drawer trên di động. |
| **NFR-14** | Trải nghiệm phòng học tập trung (Distraction-Free Mode) | Tối đa hóa diện tích hiển thị bài giảng, không gây phân tâm cho người học. | Cung cấp nút ẩn/hiện thanh giáo trình Sidebar, phím tắt điều khiển nhanh video (Phím Space: Tạm dừng/Phát; Phím mũi tên: Tua tới/lui 5 giây). |
| **NFR-15** | Phản hồi trạng thái thao tác tức thì (Instant Feedback) | Người dùng luôn nhận được phản hồi trực quan khi hệ thống đang xử lý dữ liệu. | Tích hợp thông báo Toast popup nổi (SweetAlert2 hoặc Toastr) khi thêm khóa học, áp mã coupon thành công hoặc thông báo lỗi nhập liệu rõ ràng ngay dưới từng ô input form. |

---

### 4.5. Khả năng Bảo trì & Mở rộng Mã nguồn (Maintainability & Clean Architecture)

| Mã YC | Tiêu chí đánh giá | Chuẩn mực Kỹ thuật | Giải pháp Triển khai trong Dự án Laravel |
| :---: | :--- | :--- | :--- |
| **NFR-16** | Tuân thủ chuẩn mực lập trình (Coding Standards) | Toàn bộ mã nguồn backend tuân thủ nghiêm ngặt theo tiêu chuẩn mã nguồn PHP quốc tế **PSR-12**. | Đặt tên Class dạng `PascalCase`, method/function dạng `camelCase`, biến và bảng CSDL dạng `snake_case`. Sử dụng công cụ Laravel Pint / PHP_CodeSniffer để định dạng mã nguồn. |
| **NFR-17** | Kiến trúc phân tách tầng trách nhiệm (Separation of Concerns) | Controller thanh gọn (Skinny Controllers), không viết nghiệp vụ phức tạp trực tiếp trong Controller. | • Tách tầng kiểm tra dữ liệu đầu vào sang **Form Request Classes** (`CreateCourseRequest`, `CheckoutRequest`).<br>• Tách nghiệp vụ tính toán dòng tiền, thanh toán và xử lý tiến độ sang **Service Classes** (`PaymentService`, `CourseProgressService`). |
| **NFR-18** | Tự động hóa khởi tạo và dữ liệu mẫu (Database Seeding) | Dễ dàng cài đặt và chạy thử nghiệm hệ thống chỉ với một câu lệnh terminal. | Xây dựng đầy đủ các file `DatabaseMigrations` cho 22 bảng và `DatabaseSeeder` sinh dữ liệu mẫu hợp lý cho tài khoản Admin, Giảng viên, Học viên và các khóa học demo. |

---

### 4.6. Tính Tương thích Môi trường (Compatibility)

| Mã YC | Tiêu chí | Môi trường Hỗ trợ |
| :---: | :--- | :--- |
| **NFR-19** | Tương thích Trình duyệt (Browser Compatibility) | Hoạt động ổn định trên các trình duyệt hiện đại phổ biến nhất hiện nay: Google Chrome, Microsoft Edge, Mozilla Firefox, Apple Safari (phiên bản không quá 2 năm gần nhất). |
| **NFR-20** | Môi trường Máy chủ & Ngôn ngữ (Server Environment) | • Ngôn ngữ: PHP phiên bản $\ge 8.2$.<br>• Hệ quản trị CSDL: MySQL phiên bản $\ge 8.0$ hoặc MariaDB phiên bản $\ge 10.5$ (hỗ trợ đầy đủ kiểu JSON, Regex và khóa ngoại InnoDB).<br>• Web Server: Nginx hoặc Apache có bật module `mod_rewrite`. |

---

## 5. HƯỚNG DẪN KẾ THỪA CHO CÁC MÔ HÌNH THIẾT KẾ TIẾP THEO

Tài liệu này được định dạng để bạn sử dụng trực tiếp làm đầu vào chuẩn cho các giai đoạn thiết kế tiếp theo trong báo cáo:

1. **Vẽ Sơ đồ Phân rã Chức năng (BFD):**  
   Sao chép trực tiếp cây phân cấp tại **Mục 1** vào công cụ vẽ (như Visual Paradigm, Draw.io hoặc StarUML). Cây đã được phân rã đúng 3 cấp chuẩn khoa học.
2. **Viết Đặc tả Use Case chi tiết:**  
   Mỗi mã chức năng (`F1.1` đến `F5.4`) tương ứng với một Use Case. Cột *"Mô tả Chi tiết Nghiệp vụ & Xử lý Hệ thống"* cung cấp sẵn Tiền điều kiện, Luồng sự kiện chính và Hậu điều kiện của Use Case đó.
3. **Vẽ Sơ đồ Hoạt động (Activity Diagram) & Tuần tự (Sequence Diagram):**  
   Nên chọn **4 luồng nghiệp vụ đinh** sau đây để vẽ nhằm đạt điểm số tối đa khi phản biện:
   * **Luồng 1:** Đặt hàng, Thanh toán qua Cổng VNPAY và Kích hoạt ghi danh tự động (`F2.5`, `F2.6`).
   * **Luồng 2:** Học bài giảng video, Lưu vị trí dừng và Mở khóa bài tuần tự (`F4.2`, `F4.3`).
   * **Luồng 3:** Làm bài thi Quiz và Tự động cấp Chứng chỉ điện tử PDF (`F4.5`, `F4.6`).
   * **Luồng 4:** Giảng viên gửi duyệt và Admin kiểm duyệt/xuất bản khóa học (`F3.5`, `F3.6`).
4. **Đưa Yêu cầu Phi chức năng vào Báo cáo:**  
   Toàn bộ nội dung tại **Mục 4** có thể sao chép trực tiếp vào chương *"Yêu cầu phi chức năng của hệ thống"* trong báo cáo Word, giúp thuyết phục hội đồng về tính chuyên nghiệp, an toàn thông tin và tính thực tế của phần mềm.
