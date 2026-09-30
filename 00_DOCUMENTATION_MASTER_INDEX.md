# F&B SMART V5.1 — DOCUMENTATION MASTER INDEX

## 1. Mục đích

Bộ tài liệu này là **khung đặc tả sản phẩm và kỹ thuật** dùng để bảo đảm một chức năng không chỉ có code, mà còn có:

**Yêu cầu → Giao diện → Luồng → Quy tắc → Dữ liệu → Kiến trúc → Work Item → Test → Build → PO Test → PO Verified → Protected → Locked**

Tài liệu này **không thay thế KIM CHỈ NAM**.

## 2. Thứ tự ưu tiên

Khi có mâu thuẫn:

1. KIM CHỈ NAM / Governance chính thức của F&B SMART
2. Product Charter / Specification chính thức đã được PO chấp thuận
3. Database Schema / State Machines / Security Specification
4. Roadmap / Work Item Specification
5. Bộ tài liệu này
6. Quyết định triển khai của Coding Agent

Không tài liệu nào ở cấp thấp được tự ý ghi đè cấp cao hơn.

## 3. Bộ tài liệu

| ID | Tài liệu | Mục đích |
|---|---|---|
| DOC-00 | Master Index | Điều hướng toàn bộ tài liệu |
| DOC-01 | Product Requirements | Ứng dụng phải làm gì |
| DOC-02 | UX/UI & Screen Specification | Người dùng nhìn thấy và thao tác thế nào |
| DOC-03 | Business Rules & State | Hệ thống xử lý thế nào |
| DOC-04 | Architecture & Technical Specification | Hệ thống được xây thế nào |
| DOC-05 | Database & Data Contract | Dữ liệu nằm ở đâu và có cấu trúc gì |
| DOC-06 | Security & Permission | Ai được làm gì và dữ liệu được bảo vệ thế nào |
| DOC-07 | Test & PO Acceptance | Chứng minh chức năng đúng thế nào |
| DOC-08 | Release & Operations | Build, phát hành, vận hành, phục hồi |
| DOC-09 | Feature Traceability | Liên kết mọi phần thành một chuỗi |
| DOC-10 | Work Item Contract | Mỗi Work Item phải cam kết đầu ra gì |

## 4. Quy tắc bắt buộc

Một Feature có giao diện **không được bắt đầu implementation UI** nếu chưa xác định tối thiểu:

- Feature ID
- Actor
- Screen ID
- Navigation
- User Flow
- Acceptance Criteria
- Data entities
- Permission
- Work Item

Một Feature kỹ thuật không có giao diện vẫn phải xác định:

- Requirement
- Data/Architecture impact
- Test
- Work Item
- Acceptance evidence

## 5. Nguồn tham khảo ngoài

- IEEE/ISO/IEC 29148: Requirements Engineering.
- NIST SP 800-218 SSDF: Secure Software Development Framework.
- OWASP ASVS: Application Security Verification Standard.

Các nguồn ngoài chỉ là **tham khảo phương pháp**, không phải governance của F&B SMART.
