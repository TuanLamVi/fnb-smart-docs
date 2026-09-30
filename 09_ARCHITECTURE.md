# 09 — ARCHITECTURE & TECHNICAL SPECIFICATION

## Layer
UI
→ Controller/State
→ Service
→ Repository Contract
→ Repository Implementation
→ Firebase/Backend

## Nguyên tắc
- UI không tự truy cập Firestore tùy ý.
- Repository phải có canonical scope.
- Business rules không bị giấu trong UI.
- Error phải có lớp xử lý rõ.
- Store isolation là invariant.
- Locked scope phải được bảo vệ.

## Clean Rebuild
Official application source:
`TuanLamVi/fnb-smart-v5-clean-rebuild`

Governance source:
`TuanLamVi/boquytacfnb`

Legacy:
`TuanLamVi/fnb-smart-source` — forensic reference only.

## Build baseline hiện có
Flutter 3.41.0 / Dart 3.11.0 / JDK 17 / compileSdk 36 / targetSdk 36 / minSdk 24.
Các giá trị chính thức phải đọc từ BUILD_BASELINE mới nhất trước mỗi release.
