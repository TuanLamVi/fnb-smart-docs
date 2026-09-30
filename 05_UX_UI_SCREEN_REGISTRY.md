# 05 — UX/UI & SCREEN REGISTRY

## Mục tiêu
Không để xảy ra tình trạng database đã có nhưng PO không biết tính năng nằm ở đâu.

## Screen Registry bắt buộc
| Screen ID | Tên | Actor | Entry Point | Feature | Work Item | Permission | Status |
|---|---|---|---|---|---|---|---|
| SCR-AUTH | Đăng nhập | All | App start | Auth | A1/A2 | Auth | ... |
| SCR-ACCOUNT | Quản lý tài khoản | Owner/Employee | Account flow | Account | A2 | Membership | ... |
| SCR-MENU | Menu | Staff/Manager | App navigation | Menu | A3+ | Menu permission | TO DEFINE |
| SCR-POS | Bán hàng | POS staff | POS navigation | POS | A3+ | POS permission | TO DEFINE |
| SCR-TABLE | Bàn | Staff | Table navigation | Tables | A5+ | Table permission | TO DEFINE |
| SCR-KDS | Bếp | Kitchen | KDS navigation | KDS | A4+ | KDS permission | TO DEFINE |
| SCR-CHECKOUT | Thanh toán | Authorized staff | Order | Payment | A6+ | Payment permission | TO DEFINE |

## Mỗi Screen phải có
- Mục đích.
- Entry point.
- Điều hướng vào/ra.
- Header/tab/drawer.
- Thành phần.
- Button/action.
- Loading.
- Empty.
- Error.
- Success.
- Permission.
- Store scope.
- Vietnamese UI text.
- PO Acceptance.

## Quy tắc Menu
Nếu Product Spec yêu cầu Menu là chức năng người dùng, phải chỉ rõ:
`Menu xuất hiện ở đâu → ai thấy → nhấn gì → màn hình nào mở → dữ liệu nào hiển thị`.

Không được để Codex tự đoán từ Firestore collections.
