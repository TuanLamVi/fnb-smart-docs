# 07 — BUSINESS RULES

## Rule template
`BR-<DOMAIN>-<NNN>`
- Rule:
- Trigger:
- Preconditions:
- Allowed:
- Forbidden:
- State transition:
- Data effect:
- Permission:
- Idempotency:
- Error:
- Evidence:
- Source:
- Status:

## Các nguyên tắc đã được thể hiện trong tài liệu dự án
- Mọi nghiệp vụ phải nằm trong store scope.
- Membership quyết định quyền truy cập store.
- `Còn phải thu` không tự động đồng nghĩa `Ghi nợ`.
- Payment collection phải có audit information.
- Physical cash và QR/debt có tác động khác nhau đến cash drawer.
- Legacy và Clean Rebuild không được trộn lẫn.

## First Failure
Khi phát hiện lỗi:
`STOP → Evidence → Root Cause → Authorized Surgical Fix → Retest → Report`
