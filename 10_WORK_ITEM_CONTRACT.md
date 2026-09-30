# F&B SMART V5.1 — WORK ITEM CONTRACT

## 1. Mục tiêu

Chuẩn hóa đầu vào/đầu ra của từng Work Item.

## 2. Required Header

- Prompt ID
- Work Item ID
- Work Item Name
- Parent Phase
- Dependencies
- Scope
- Out of Scope
- PO Authorization
- Expected User-visible Result
- Expected Technical Result
- Test Plan
- Build Requirement
- Closure Requirement

## 3. Read-First

Coding Agent phải đọc:

- KIM CHỈ NAM
- Current State
- Roadmap
- Relevant Product Spec
- Database Schema
- State Machines
- Security
- Previous Work Item evidence
- Protected/Locked records

## 4. Execution

`READ-FIRST → FORENSIC → IMPLEMENT → TEST → BUILD → EVIDENCE → REPORT`

Nếu failure:

`STOP → Evidence → Root Cause → Authorization → Fix → Retest`

## 5. Final Report

Bắt buộc:

- Prompt
- Work Item
- Read-first evidence
- Scope
- Files changed
- Implementation result
- Test result
- Build result
- Device result if applicable
- Git status
- Commit
- Evidence
- Blockers
- Out-of-scope changes
- Recommended next action

## 6. No Self-Approval

Coding Agent không được tự:

- PO_VERIFIED
- PROTECTED
- LOCKED

## 7. Meaningful Commit

Commit khi đạt meaningful milestone:

- Implementation + Test + Build PASS
- PO verification
- Protection/Lock
- Governance milestone
- High-risk safety checkpoint

Không commit mỗi prompt nếu chưa đạt milestone.

## 8. User-visible requirement

Nếu Work Item có UI:

Final Report phải trả lời:

- UI nằm ở màn hình nào?
- Entry point là gì?
- PO thao tác thế nào?
- UI Acceptance Criteria nào đã được kiểm thử?

Nếu Work Item chỉ là foundation/data:

Phải ghi rõ:

`USER-VISIBLE RESULT: NOT INCLUDED IN THIS WORK ITEM`

Điều này ngăn PO hiểu nhầm foundation = hoàn thành chức năng.
