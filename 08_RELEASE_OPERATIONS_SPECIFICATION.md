# F&B SMART V5.1 — RELEASE & OPERATIONS SPECIFICATION

## 1. Development

Ghi rõ:

- Flutter
- Dart
- Android SDK
- JDK
- Gradle
- AGP
- Kotlin
- Firebase environment

Version phải lấy từ repository/build evidence, không đoán.

## 2. Build

Mỗi build:

- Version
- Build number
- Source commit
- Branch
- Environment
- APK path
- SHA256
- Build result

## 3. Release Gate

Trước release phải xác nhận:

- Required implementation
- Unit tests
- Integration tests
- E2E
- Regression
- Security
- Build
- Device
- PO acceptance
- Governance closure

## 4. Deployment

Ghi:

- Environment
- Target
- Timestamp
- Actor
- Version
- Result
- Rollback plan

## 5. Production Safety

Không tự ý deploy production từ Work Item development.

Mọi production action phải theo governance/authorization hiện hành.

## 6. Monitoring

Theo dõi:

- Crash
- Auth errors
- Backend errors
- Firestore permission errors
- Performance
- Critical business failures

## 7. Incident

Khi phát hiện lỗi nghiêm trọng:

`STOP → Preserve Evidence → Record → Triage → Root Cause → Authorized Fix → Regression`

## 8. Recovery

Phải có:

- Recovery owner
- Backup/reference
- Rollback method
- Verification
- Post-recovery evidence

## 9. Change Log

Mỗi meaningful milestone phải có record.

Không tạo commit vô nghĩa chỉ để đáp ứng một prompt nhỏ.
