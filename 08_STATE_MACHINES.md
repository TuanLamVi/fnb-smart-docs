# 08 — STATE MACHINES

## State machine template
- Machine ID:
- Entity:
- States:
- Initial state:
- Allowed transitions:
- Forbidden transitions:
- Trigger:
- Actor:
- Side effects:
- Idempotency:
- Failure handling:
- Test IDs:
- Source:

## Ví dụ đã được thể hiện trong product discovery
### Table
`occupied → cleaning → available`

### KDS
`queued → acknowledged → preparing → ready → served`

### Membership
`pending → active → inactive/revoked`

> Các state machine chính thức phải đối chiếu `STATE_MACHINES_V0.1.md`; file này chỉ là khung tổ chức.
