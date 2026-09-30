# 04 — ROADMAP & WORK ITEM MAP

## Roadmap Canonical hiện có
`A0 → A1 → A2 → A3 → A4 → A5 → A6 → A7 → A8 → A9 → A10 → A11`

## Quy tắc
- Child PASS không tự nâng Parent.
- Không tự crosswalk ID lịch sử với ID mới.
- Mỗi Work Item phải có dependency, scope và out-of-scope.
- Work Item mới phải READ-FIRST.
- Không đụng vùng LOCKED nếu chưa có UNLOCK.

## Bản đồ A3 hiện được chứng minh trong Clean Rebuild
### A3-01
Menu Catalog data/model/repository foundation.
Canonical entities đã xuất hiện:
- Category
- Product
- Modifier Group
- Modifier Item

Canonical paths:
- `/stores/{storeId}/categories/{categoryId}`
- `/stores/{storeId}/products/{productId}`
- `/stores/{storeId}/modifierGroups/{groupId}`
- `/stores/{storeId}/modifierItems/{itemId}`

### A3-02
Orders / Order Lines state engine là phạm vi tiếp theo đã được ghi nhận trong lịch sử Clean Rebuild.

### Cảnh báo
A3-01 là foundation/data layer. Technical PASS không đồng nghĩa Menu UI đã hoàn thành.
