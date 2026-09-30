# F&B SMART V5.1 — ARCHITECTURE & TECHNICAL SPECIFICATION

## 1. Mục tiêu

Mô tả cách Feature được xây mà không biến Product Requirement thành code.

## 2. Layer

Khung tham khảo:

`View/UI → State/Controller → Repository → Data/Backend`

Mỗi Feature phải xác định layer nào được sử dụng.

## 3. Module Contract

Mỗi module:

- Purpose
- Public API
- Dependencies
- Forbidden dependencies
- Models
- Repository
- Services
- UI
- Tests

## 4. Repository Contract

Mỗi repository:

- Interface/contract
- Canonical data path
- Read methods
- Write methods
- Validation
- Error handling
- Store scope
- Authentication requirement

## 5. Error Handling

Mỗi lỗi phải phân loại:

- User input
- Permission
- Authentication
- Network
- Backend
- Data integrity
- Configuration
- Unexpected

User-facing message phải dễ hiểu và bằng tiếng Việt.

## 6. Observability

Mỗi feature quan trọng cần xác định:

- Log event
- Correlation/context
- Error evidence
- Sensitive data exclusion

Không log OTP, password, token hoặc dữ liệu nhạy cảm.

## 7. Build Provenance

Mọi build dùng cho PO test phải truy được:

`Source commit → Build configuration → APK → Device → Test evidence`

## 8. Protected Scope

Code đã PROTECTED/LOCKED không được sửa ngoài quy trình mở khóa chính thức.

## 9. First Failure Stop

Khi gặp lỗi hoặc mâu thuẫn:

`STOP → Evidence → Root Cause → Authorized Fix → Test → Evidence`

Không sửa lan sang domain khác để che lỗi.
