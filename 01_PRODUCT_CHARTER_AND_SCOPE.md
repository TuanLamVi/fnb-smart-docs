# 01 — PRODUCT CHARTER & SCOPE

## 1. Mục tiêu
Mô tả sản phẩm ở cấp cao trước khi đi vào code.

## 2. F&B SMART V5.1
Theo các tài liệu hiện có, đây là hệ thống POS & quản lý F&B theo mô hình SaaS Multi-Tenant/Cửa hàng.

## 3. Các miền chức năng đã xuất hiện trong tài liệu
- Tài khoản / xác thực.
- Store / membership / nhân viên / thiết bị.
- Menu / Category / Product / Modifier.
- POS / Cart / Order / Order Lines.
- Bàn / Table Management.
- Kitchen / KDS.
- Checkout / Payment.
- Shift / Cash Drawer.
- Customer / Debt.
- Reports / Analytics.

## 4. Ranh giới
Clean Rebuild và Legacy là hai hệ thống riêng.
Legacy được coi là FROZEN / Read-Only Forensic Reference theo Governance hiện hành.

## 5. Quy tắc phạm vi
Mọi chức năng chưa có nguồn chính thức phải đánh dấu:
`UNPROVEN / TBD / PO DECISION REQUIRED`.

Không tự mở rộng MVP từ discovery thành implementation.
