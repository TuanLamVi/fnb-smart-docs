# 13 — TEST & PO ACCEPTANCE

## Test layers
1. Unit.
2. Widget/UI.
3. Integration.
4. E2E.
5. Security/rules.
6. Regression.
7. Real-device.
8. PO Acceptance.

## Test case template
`TEST-<ID>`
- Feature:
- Requirement:
- Preconditions:
- Device/environment:
- Steps:
- Expected:
- Actual:
- Evidence:
- Result:
- PO verification:

## PO Acceptance
PO phải có thể thao tác bằng ngôn ngữ người dùng thật.
Không chấp nhận:
- chỉ xem log;
- chỉ xem unit test;
- chỉ xem build success;
- chỉ xem database.

## Closure
`PASS → PO_VERIFIED → REGRESSION CHECK → PROTECTED → LOCKED`
