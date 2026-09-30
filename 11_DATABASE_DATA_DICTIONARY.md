# 11 — DATABASE & DATA DICTIONARY

## Canonical Menu paths
`/stores/{storeId}/categories/{categoryId}`
`/stores/{storeId}/products/{productId}`
`/stores/{storeId}/modifierGroups/{groupId}`
`/stores/{storeId}/modifierItems/{itemId}`

## Field registry
Mỗi field phải ghi:
- name
- type
- required
- default
- immutable
- writable by
- readable by
- validation
- meaning

## Store isolation
Mọi read/write nghiệp vụ phải có:
`storeId + membership + permission + canonical path`

## Index registry
Mỗi query cần index phải ghi:
query → collection → fields → direction → scope → reason → deployment status.

## Migration
`Current → Target → Migration → Verification → Rollback/Recovery`
