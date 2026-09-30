# F&B SMART V5.1 — SECURITY & PERMISSION SPECIFICATION

## 1. Security Objectives

- Authentication đúng người.
- Authorization đúng quyền.
- Store isolation.
- Không lộ dữ liệu tenant khác.
- Không tin dữ liệu từ client nếu server/rules phải xác minh.
- Có evidence khi xảy ra lỗi bảo mật.

## 2. Authentication

Phải xác định:

- Provider
- Identity
- Session
- Re-authentication
- Logout
- Session restore
- Account lifecycle

F&B SMART hiện dùng Firebase Phone Authentication theo baseline dự án.

## 3. Authorization

Mỗi hành động phải trả lời:

`User + Store + Membership + Role/Permission → Allowed/Denied`

## 4. Permission Matrix

| Action | Owner | Manager | Staff | Other |
|---|---|---|---|---|
| Xem dữ liệu | Theo policy | Theo policy | Theo policy | Deny |
| Tạo | Theo policy | Theo policy | Theo policy | Deny |
| Sửa | Theo policy | Theo policy | Theo policy | Deny |
| Xóa | Theo policy | Theo policy | Theo policy | Deny |

Không điền quyền cụ thể nếu chưa có Product/Security Decision chính thức.

## 5. Firestore Rules

Mỗi collection phải kiểm tra:

- Authenticated?
- Correct store?
- Correct membership?
- Correct role?
- Allowed operation?
- Field restrictions?
- Cross-store access?

## 6. App Check

Phải xác định:

- Environment
- Provider
- Enforcement state
- Debug handling
- Failure behavior

## 7. Sensitive Data

Không ghi vào log:

- OTP
- Access token
- Refresh token
- Password
- Secret key
- Sensitive personal data không cần thiết

## 8. Security Testing

Security test phải bao gồm:

- Unauthorized read
- Unauthorized write
- Cross-store read
- Cross-store write
- Revoked membership
- Wrong role
- Invalid document ownership

## 9. External Security Reference

NIST SSDF có thể dùng làm khung secure development; OWASP ASVS có thể dùng làm checklist kiểm tra technical security controls. Đây là nguồn tham khảo, không thay thế security rules riêng của F&B SMART.
