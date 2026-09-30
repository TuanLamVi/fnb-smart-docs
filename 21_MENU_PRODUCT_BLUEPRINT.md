# 21 — MENU PRODUCT BLUEPRINT
## Tài liệu tham khảo để giải quyết đúng vấn đề “Menu nằm ở đâu?”

### 1. Mục tiêu
Menu phải được mô tả trên cả 4 lớp:
`Data → Feature → Screen → PO Test`

### 2. Data layer
A3-01 đã xác nhận foundation cho:
- Category.
- Product.
- Modifier Group.
- Modifier Item.

### 3. UI layer — điều bắt buộc phải có trong Product/UI Specification
- Screen ID của Menu.
- Entry point từ navigation.
- Actor được thấy Menu.
- Category list.
- Product list.
- Product detail.
- Modifier/Option display.
- Empty state.
- Loading state.
- Error state.
- Permission.
- Store scope.
- Vietnamese labels.

### 4. POS relationship
Menu là nguồn để POS chọn sản phẩm; Product/Modifier data phải được liên kết với POS ordering contract.

### 5. Không được suy diễn
A3-01 PASS không chứng minh SCR-MENU đã tồn tại.
Nếu APK chưa có Menu, cần xác định Work Item UI tương ứng từ Product/UX/Roadmap chính thức trước khi sửa code.

### 6. PO Acceptance mẫu
- Mở app.
- Vào đúng khu vực Menu.
- Thấy Category.
- Chọn Category.
- Thấy Product.
- Mở Product.
- Thấy Modifier/Option khi có.
- Không thấy dữ liệu của store khác.
- Các trạng thái Empty/Error hiển thị đúng.
