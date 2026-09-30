# F&B SMART V5.1 — UX/UI & SCREEN SPECIFICATION

## 1. Mục đích

Đây là lớp tài liệu bị thiếu nếu chỉ có Product + Database.

Nó trả lời:

> Người dùng mở app sẽ thấy gì, bấm vào đâu, và sau mỗi thao tác chuyện gì xảy ra?

## 2. Screen Registry

Mỗi màn hình phải có:

- Screen ID
- Tên tiếng Việt
- Tên kỹ thuật nếu cần
- Actor
- Feature
- Work Item
- Route
- Entry point
- Exit points
- Permission
- State dependencies

## 3. Navigation Registry

Mỗi navigation item:

- Navigation ID
- Label hiển thị
- Icon
- Vị trí
- Actor
- Điều kiện hiển thị
- Route
- Feature
- Work Item

### Quy tắc

Nếu một Feature yêu cầu người dùng truy cập từ Tab/Menu/Drawer thì phải ghi rõ **entry point**.

Không được để Codex tự suy đoán từ database.

## 4. Screen Specification

Mỗi màn hình:

### Header
- Tiêu đề
- Back
- Store context
- Actions

### Body
- Nội dung
- Component
- Data source
- Empty state
- Loading state
- Error state

### Actions
- Button
- Gesture
- Confirmation
- Success result
- Failure result

### Permission
- Ai nhìn thấy
- Ai được sửa
- Ai được xóa

## 5. User Flow

Mỗi flow:

`Entry → Action → System response → Next screen/state`

Phải mô tả cả:

- First use
- Returning user
- Empty data
- Error
- Permission denied
- Network unavailable

## 6. Localization

User-facing UI của F&B SMART phải ưu tiên tiếng Việt theo quyết định sản phẩm hiện hành.

Không dùng nhãn kỹ thuật tiếng Anh trong UI người dùng nếu chưa có lý do sản phẩm rõ ràng.

## 7. MENU — SPECIFICATION FRAMEWORK

### Entry

Phải xác định:

- Menu là Tab, Drawer, Dashboard card hay entry khác?
- Ai nhìn thấy?
- Khi nào hiển thị?
- Điều hướng tới đâu?

### Menu Home

Phải xác định:

- Category list
- Product list
- Search
- Filter
- Add/Edit/Delete nếu có
- Empty state

### Product

Phải xác định:

- Tên
- Giá
- Category
- Trạng thái bán
- Modifier Groups
- Hình ảnh nếu có
- Mô tả nếu có

### Modifier

Phải xác định:

- Group
- Item
- Required/Optional
- Single/Multiple selection
- Min/Max selection
- Giá cộng thêm

**Tất cả mục trên là specification framework. Giá trị chính thức phải được chốt trong Product Decision/UI Specification.**

## 8. PO UI Acceptance

Mỗi màn hình phải có test dạng người thật:

1. Mở app.
2. Vào entry point.
3. Nhìn thấy đúng màn hình.
4. Thực hiện thao tác.
5. Quan sát kết quả.
6. Kiểm tra trạng thái lỗi/empty nếu có.

PO không cần hiểu code để nghiệm thu UI.
