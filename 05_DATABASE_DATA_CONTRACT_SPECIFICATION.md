# F&B SMART V5.1 — DATABASE & DATA CONTRACT SPECIFICATION

## 1. Collection Registry

Mỗi collection:

- Collection ID
- Canonical path
- Owner domain
- Tenant/store scope
- Document ID
- Parent relationship
- Security owner
- Index requirements

## 2. Field Registry

Mỗi field:

- Name
- Type
- Required
- Default
- Immutable?
- Writable by whom
- Readable by whom
- Validation
- Meaning

## 3. Canonical Path Rule

Một entity phải có **canonical path** duy nhất.

Ví dụ theo A3 hiện hành:

`/stores/{storeId}/categories/{categoryId}`

`/stores/{storeId}/products/{productId}`

`/stores/{storeId}/modifierGroups/{groupId}`

`/stores/{storeId}/modifierItems/{itemId}`

Đây là các path đã xuất hiện trong A3-01 implementation report; mọi thay đổi phải đối chiếu Database Schema chính thức.

## 4. Store Isolation

Mọi read/write nghiệp vụ phải xác định:

- Current store
- Membership
- Permission
- Canonical store path

Không dùng path Legacy chỉ vì code cũ đang có sẵn.

## 5. Index Registry

Mỗi query cần index phải ghi:

- Query
- Collection
- Fields
- Direction
- Scope
- Reason
- Deployment status

## 6. Data Lifecycle

Mỗi entity cần quy định:

- Create
- Read
- Update
- Archive/Delete
- Restore
- Retention

## 7. Migration

Mọi schema change:

`Current → Target → Migration → Verification → Rollback/Recovery`

Không tự migration production khi chưa có authorization.

## 8. Data Integrity

Các invariant quan trọng phải được ghi rõ.

Ví dụ:

- Entity không được vượt store scope.
- Reference không được trỏ sang store khác nếu business rule cấm.
- State phải thuộc danh sách hợp lệ.
