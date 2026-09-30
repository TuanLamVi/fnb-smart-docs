# 10 — REPOSITORY / SERVICE / API CONTRACTS

## Repository Contract
Mỗi repository phải định nghĩa:
- Interface/Contract.
- Entity/model.
- Store scope.
- Read operations.
- Write operations.
- Validation.
- Error contract.
- Idempotency nếu có.
- Security assumptions.
- Test.

## Menu Contract
`CleanRebuildMenuRepositoryContract`
- Category read/write.
- Product read/write.
- Modifier Group read/write.
- Modifier Item read/write.
- Store scoping.
- Serialization/deserialization.
- Error handling.

## Quy tắc
Implementation không được tự đổi canonical path.
Thay đổi contract phải có impact review.
