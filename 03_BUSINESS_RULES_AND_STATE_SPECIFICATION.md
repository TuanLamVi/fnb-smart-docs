# F&B SMART V5.1 — BUSINESS RULES & STATE SPECIFICATION

## 1. Mục đích

Tách rõ:

- Người dùng muốn gì
- Hệ thống được phép làm gì
- Trạng thái nào hợp lệ
- Trạng thái nào không hợp lệ

## 2. Business Rule ID

`BR-<DOMAIN>-<NUMBER>`

Ví dụ:

- BR-MENU-001
- BR-ORDER-001
- BR-PAYMENT-001

## 3. Rule Template

- Rule ID
- Mô tả
- Actor
- Điều kiện
- Hành động
- Kết quả
- Ngoại lệ
- Security impact
- Data impact
- Test ID

## 4. State Machine Template

- Entity
- Initial State
- States
- Allowed transitions
- Forbidden transitions
- Actor
- Trigger
- Side effects
- Recovery

## 5. State Change Rule

Mọi transition quan trọng phải trả lời:

`Ai → làm gì → từ trạng thái nào → sang trạng thái nào → điều kiện gì → hệ quả gì`

## 6. Cross-domain transaction

Khi một hành động ảnh hưởng nhiều domain, phải mô tả toàn bộ chuỗi.

Ví dụ khung:

`Payment Success → Order Paid → Table Closure → Financial Record`

Không được chỉ mô tả Payment mà bỏ qua tác động sang Table/Order.

## 7. Idempotency

Các hành động có thể gửi lại phải xác định:

- Có được chạy lại không?
- Nếu chạy lại thì kết quả có thay đổi không?
- Cách chống duplicate.

## 8. Edge Cases

Mỗi Feature phải xem xét:

- Double tap
- Retry
- Network loss
- Permission change
- Session restore
- Store switch
- Concurrent user
- Duplicate request
- Missing document
- Invalid state

## 9. Source of Truth

Mỗi entity phải có một nơi xác định là nguồn trạng thái chính.

Không cho phép hai nguồn cùng được coi là canonical nếu chưa có quy tắc đồng bộ.
