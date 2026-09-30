# F&B SMART V5.1 — FEATURE TRACEABILITY MATRIX

## 1. Mục tiêu

Đây là tài liệu chống "mất liên kết" giữa Product và Code.

## 2. Chuỗi truy nguyên

`Requirement`
→ `Feature`
→ `Screen`
→ `User Flow`
→ `Business Rule`
→ `State`
→ `Database`
→ `Repository`
→ `Work Item`
→ `Test`
→ `Build`
→ `PO Test`
→ `PO Verified`
→ `Protected`
→ `Locked`

## 3. Matrix

| Requirement | Feature | Screen | Rule | Data | Work Item | Test | Build | PO |
|---|---|---|---|---|---|---|---|---|

## 4. UI Gap Detection

Nếu:

- Requirement = YES
- Screen = MISSING

→ GAP.

Nếu:

- Screen = YES
- Work Item = MISSING

→ GAP.

Nếu:

- Technical implementation = PASS
- User-visible result = MISSING

→ Không được coi là Feature hoàn chỉnh.

## 5. Menu Example

| Layer | Expected record |
|---|---|
| Requirement | MENU requirement |
| Feature | MENU |
| Entry | Tab/Drawer/other documented entry |
| Screen | Menu screen |
| Category | Category screen/component |
| Product | Product screen/component |
| Modifier | Modifier UI |
| Data | Category/Product/Modifier collections |
| Repository | Menu repository |
| Work Item | A3 Work Item |
| Test | Menu tests |
| PO | Open app and operate Menu |

**Đây là khung kiểm tra, không phải tự xác nhận rằng Menu UI hiện đã được xây.**

## 6. Traceability Gate

Một Work Item có thể PASS về kỹ thuật nhưng vẫn phải báo:

- Technical PASS
- User-visible PASS/NOT APPLICABLE
- Traceability PASS/FAIL

Điều này tránh nhầm "repository foundation PASS" với "complete user feature".
