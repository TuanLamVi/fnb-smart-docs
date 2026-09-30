# F&B SMART V5.1 — PRODUCT REQUIREMENTS SPECIFICATION

## 1. Mục đích

Mô tả sản phẩm ở mức mà PO, Designer, Coding Agent và Tester đều hiểu giống nhau.

## 2. Product Requirement ID

Mỗi requirement có ID ổn định:

`PRD-<DOMAIN>-<NUMBER>`

Ví dụ:

- PRD-AUTH-001
- PRD-MENU-001
- PRD-POS-001
- PRD-TABLE-001

## 3. Mẫu Requirement

### Requirement
- ID:
- Tên:
- Mục đích:
- Actor:
- Tiền điều kiện:
- Trigger:
- Luồng chính:
- Luồng ngoại lệ:
- Kết quả:
- Business Rules liên quan:
- Screen liên quan:
- Data liên quan:
- Permission:
- Work Item:
- Test Cases:
- PO Acceptance:
- Trạng thái:

## 4. Functional Requirements

Functional Requirement phải mô tả **hệ thống làm gì**, không mô tả code phải viết thế nào.

Ví dụ:

`PRD-MENU-001`
Người dùng có quyền phù hợp có thể mở khu vực Menu của cửa hàng đang hoạt động.

`PRD-MENU-002`
Người dùng có thể xem Category thuộc cửa hàng hiện tại.

`PRD-MENU-003`
Người dùng có thể xem Product thuộc Category/cửa hàng theo quy định.

Lưu ý: đây là **mẫu minh họa**, không tự biến thành yêu cầu chính thức nếu chưa có trong Product Specification/PO Decision.

## 5. Non-Functional Requirements

Mỗi domain cần xem xét:

- Performance
- Reliability
- Availability
- Security
- Data isolation
- Observability
- Accessibility
- Localization
- Maintainability

## 6. Definition of Requirement

Requirement tốt phải:

- Rõ
- Có thể kiểm tra
- Không mâu thuẫn
- Có phạm vi
- Có actor
- Có kết quả mong muốn
- Có cách nghiệm thu

## 7. Requirement Change

Không sửa requirement quan trọng âm thầm.

Mỗi thay đổi phải ghi:

- Requirement cũ
- Requirement mới
- Lý do
- Người quyết định
- Ảnh hưởng
- Work Items bị ảnh hưởng
- Regression cần chạy

## 8. PO Boundary

ChatGPT/Coding Agent có thể phân tích và đề xuất.

PO quyết định các thay đổi về sản phẩm/phạm vi.

AI/Coding Agent không tự tuyên bố PO_VERIFIED.
