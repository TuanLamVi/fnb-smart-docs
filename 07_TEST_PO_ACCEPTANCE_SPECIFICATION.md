# F&B SMART V5.1 — TEST & PO ACCEPTANCE SPECIFICATION

## 1. Mục tiêu

Một báo cáo `PASS` phải có bằng chứng tương ứng.

## 2. Test Layers

### Unit
Kiểm tra logic nhỏ.

### Integration
Kiểm tra các thành phần làm việc cùng nhau.

### E2E
Kiểm tra luồng thực tế.

### Regression
Bảo đảm thay đổi mới không phá phần đã khóa.

### PO Test
Người dùng/PO thao tác thực tế trên build được xác định.

## 3. Test Case Template

- Test ID
- Requirement ID
- Preconditions
- Steps
- Expected Result
- Actual Result
- Evidence
- Build identity
- Result

## 4. PO Test Template

PO Test phải viết bằng ngôn ngữ thao tác:

`Mở → bấm → nhập → chọn → quan sát`

Không bắt PO kiểm tra code.

## 5. Evidence

Evidence có thể gồm:

- Screenshot
- Screen recording
- Log
- Test output
- APK hash
- Device
- Timestamp
- Firestore evidence khi cần

## 6. Build Identity

PO test chỉ hợp lệ khi xác định được:

- Commit
- APK
- SHA256
- Device
- Install time/version

## 7. First Failure Stop

Nếu test thất bại:

1. Dừng.
2. Ghi lỗi đầu tiên.
3. Không bỏ qua để test tiếp như thể PASS.
4. Cô lập nguyên nhân.
5. Sửa đúng phạm vi được phép.
6. Chạy lại test.
7. Ghi evidence mới.

## 8. PO Verification

Chỉ PO xác nhận:

`PO_VERIFIED`

AI/Codex chỉ được báo:

- Technical PASS
- Test PASS
- Ready for PO Verification

## 9. Closure Chain

Theo governance hiện hành:

`PASS → PO_VERIFIED → REGRESSION CHECK → PROTECTED → LOCKED`

Không bỏ qua bước.

## 10. Definition of Test Complete

Không chỉ có "tests passed".

Phải biết:

- Test cái gì?
- Theo requirement nào?
- Build nào?
- Bằng chứng nào?
- Ai xác nhận?
