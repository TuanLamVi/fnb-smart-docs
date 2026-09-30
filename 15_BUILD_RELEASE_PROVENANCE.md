# 15 — BUILD / RELEASE / PROVENANCE

## Chuỗi provenance
`Source Commit → Build Environment → Build Command → APK Hash → Device Install → Runtime Test → PO Test`

## Release gate
- Scope correct.
- Tests PASS.
- Build PASS.
- Build identity verified.
- Real device test where required.
- Regression PASS.
- PO_VERIFIED.
- Protection/Lock.
- Release record synchronized.

## Không được
- dùng APK không biết source commit;
- gọi Build SUCCESS là Feature PASS;
- production deploy khi governance chưa cho phép;
- bỏ qua regression.
