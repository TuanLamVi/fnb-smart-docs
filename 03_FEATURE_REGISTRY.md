# 03 — FEATURE REGISTRY

## Mục đích
Danh mục trung tâm của toàn bộ Feature.

| Feature ID | Feature | Actor | Screen | Work Item | Test | PO Status |
|---|---|---|---|---|---|---|
| F-A1 | Account / Store | Owner/Employee | Account flow | A1/A2 | ... | ... |
| F-A3-MENU | Menu Catalog | Owner/Manager/Staff | TBD/Defined by UX | A3-01+ | ... | ... |
| F-A3-POS | POS Ordering | Staff | POS | A3-02+ | ... | ... |
| F-A4-KDS | Kitchen/KDS | Kitchen Staff | KDS | A4+ | ... | ... |
| F-A5-TABLE | Tables | Staff | Table Map | A5+ | ... | ... |
| F-A6-PAY | Checkout/Payment | Authorized Staff | Checkout | A6+ | ... | ... |

> Các dòng trên là registry khung, không tự biến thành lịch triển khai chính thức nếu Roadmap/PO chưa xác nhận.

## Trạng thái
NOT_STARTED → IN_PROGRESS → READY_FOR_PO_VERIFICATION → PO_VERIFIED → PROTECTED → LOCKED

Failure states: FAILED / BLOCKED / REGRESSION / UNPROVEN.
