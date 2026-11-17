[LAYER 1: METADATA & CONTEXT]
- Screen Name: [Tên màn hình chính xác]
- Role / User: [Student / Instructor / Admin / Guest]
- Objective: [Mục tiêu nghiệp vụ chính của màn hình này theo SRS]
- Theme/Style: [Ví dụ: Clean modern SaaS, neutral slate background, accent #4F46E5, Inter font, 8px border-radius]

[LAYER 2: LAYOUT ARCHITECTURE]
- Viewport: [Desktop 1440px / Responsive]
- Structure: [Ví dụ: Sticky Topbar (h=64px) + Left Sidebar (w=260px) + Main Content (12-column grid)]
- Visual Hierarchy: [Khu vực nào là trọng tâm mắt người nhìn đầu tiên]

[LAYER 3: DETAILED COMPONENT BREAKDOWN (MAP TO DB)]
- Header/Navigation:
  * [Thành phần 1, 2, ...]
- Main Section / Workspace:
  * Component A: [Tên component] -> Data fields: [Tên cột DB: ví dụ course_title, original_price, discount_price] -> Visual style: [Badge/Card/Text/Button]
  * Component B: [Tên component] -> Data fields: [...]
- Sidebar / Secondary Panel (nếu có):
  * [Các widget, sticky checkout card, hoặc curriculum navigation]

[LAYER 4: STATES & MICRO-COPY]
- Current State Rendered: [Default with data / Empty state / Editing mode]
- Realistic Dummy Data: [Cung cấp 1-2 mẫu dữ liệu cụ thể để UI không bị dùng Lorem Ipsum nhàm chán]
- Key Actions / CTAs: [Nút bấm chính: label, màu sắc, vị trí]

[LAYER 5: STITCH-SPECIFIC RENDERING HINTS]
- Bố cục khoảng cách: Tinh gọn, padding tiêu chuẩn 24px, card shadow nhẹ (`shadow-sm`).
- Không tạo các nút thừa hoặc hiệu ứng phức tạp không cần thiết cho báo cáo.