# 19 — WORK ITEM CONTRACT

## Header
- Prompt ID
- Work Item ID
- Name
- Parent Phase
- Build Mode
- Dependencies
- Protected Scope
- Objective
- Scope
- Out of Scope
- PO Authorization
- Expected User-visible Result
- Expected Technical Result
- Test Plan
- Build Requirement
- Evidence Requirement
- Closure Requirement

## Execution
`READ-FIRST → FORENSIC → IMPLEMENT → TEST → BUILD → EVIDENCE → REPORT`

## Nếu failure
`STOP → Evidence → Root Cause → Authorization → Surgical Fix → Retest`

## Final Report
- Read-first evidence.
- Scope.
- Files changed.
- Implementation.
- Test.
- Build.
- Device.
- Git.
- Commit.
- Evidence.
- Blockers.
- Out-of-scope.
- Next action.

## User-visible Result
Nếu data/foundation only:
`USER-VISIBLE RESULT: NOT INCLUDED IN THIS WORK ITEM`

Nếu có UI:
phải chỉ rõ Screen + Entry Point + thao tác + Acceptance Criteria.
