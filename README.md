# LMS Website — Đồ án khóa luận tốt nghiệp

Hệ thống quản lý học tập trực tuyến (Learning Management System — LMS), định hướng xây dựng nền tảng học tập theo mô hình marketplace: học viên tham gia khóa học, giảng viên biên soạn nội dung và quản trị viên kiểm duyệt, vận hành hệ thống.

> **Trạng thái hiện tại:** Repository đang lưu tài liệu phân tích yêu cầu, ghi chú chức năng và thiết kế cơ sở dữ liệu. Mã nguồn ứng dụng chưa được đưa vào repository; hướng công nghệ dự kiến được mô tả trong tài liệu là Laravel (PHP) và MySQL.

## Mục tiêu

- Mô hình hóa các nghiệp vụ chính của một nền tảng học trực tuyến.
- Thiết kế cơ sở dữ liệu phục vụ người dùng, khóa học, bài học, tiến độ, kiểm tra và giao dịch.
- Làm cơ sở cho các bước triển khai, kiểm thử và hoàn thiện đồ án.

## Vai trò và phạm vi chức năng

- **Học viên:** khám phá khóa học, ghi danh, học video/bài đọc, lưu tiến độ và ghi chú, làm quiz, thảo luận, đánh giá và nhận chứng chỉ.
- **Giảng viên:** quản lý hồ sơ, xây dựng chương/bài học và quiz, gửi khóa học để duyệt, theo dõi học viên/doanh thu và yêu cầu rút tiền.
- **Quản trị viên:** quản lý người dùng và danh mục, kiểm duyệt khóa học, theo dõi đơn hàng, xử lý yêu cầu rút tiền và xem báo cáo tổng quan.

Các chức năng được phân rã thành 5 phân hệ: người dùng; khám phá và thương mại; biên soạn khóa học; học tập và tương tác; báo cáo và tài chính. Đây là phạm vi thiết kế, không khẳng định các tính năng đã được triển khai trong ứng dụng.

## Công nghệ định hướng

- **Backend:** Laravel / PHP 8.2 trở lên
- **Cơ sở dữ liệu:** MySQL 8.0 trở lên hoặc MariaDB 10.5 trở lên
- **Storage engine và mã hóa:** InnoDB, `utf8mb4`
- **Thanh toán dự kiến:** VNPAY (một số tài liệu có đề cập các cổng khác)

## Tài liệu trong repository

- [Đặc tả yêu cầu tính năng hệ thống LMS](DAC_TA_YEU_CAU_TINH_NANG_HE_THONG_LMS.md) — phân hệ, chức năng, yêu cầu phi chức năng và ma trận truy vết.
- [Ghi chú chức năng hệ thống LMS](GHI_CHU_TINH_NANG_HE_THONG_LMS.md) — ghi chú tham khảo và ý tưởng tính năng cho học viên, giảng viên, quản trị viên.
- [Thiết kế cơ sở dữ liệu LMS](database/THIET_KE_CO_SO_DU_LIEU_LMS.md) — thuyết minh thiết kế dữ liệu.
- [Database schema SQL](database/database_schema.sql) — script tạo cấu trúc cơ sở dữ liệu.

Schema hiện mô hình hóa các nhóm dữ liệu như người dùng và hồ sơ giảng viên, danh mục/khóa học/chương/bài học, quiz, ghi danh và tiến độ, ghi chú/chứng chỉ, đơn hàng/mã giảm giá/yêu cầu rút tiền, đánh giá và bình luận.

## Khởi tạo cơ sở dữ liệu thiết kế

Yêu cầu MySQL 8.0+ hoặc MariaDB 10.5+. Tạo một database phát triển trống, ví dụ `lms_website`, sau đó nạp schema:

```bash
mysql -u <username> -p -e "CREATE DATABASE lms_website CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;"
mysql -u <username> -p lms_website < database/database_schema.sql
```

> **Cảnh báo:** `database/database_schema.sql` có các lệnh `DROP TABLE IF EXISTS` để dựng lại schema. Chỉ chạy trên database thử nghiệm/phát triển phù hợp; không chạy trên database có dữ liệu cần giữ hoặc môi trường production.

## Cấu trúc hiện tại

```text
.
├── README.md
├── DAC_TA_YEU_CAU_TINH_NANG_HE_THONG_LMS.md
├── GHI_CHU_TINH_NANG_HE_THONG_LMS.md
└── database/
    ├── THIET_KE_CO_SO_DU_LIEU_LMS.md
    └── database_schema.sql
```

## Tác giả

- **Sinh viên:** Trần Văn Tài
- **MSSV:** DH52201396
- **Lớp:** D22-TH05

---

*Tài liệu và thiết kế sẽ được cập nhật theo tiến độ thực hiện đồ án.*
