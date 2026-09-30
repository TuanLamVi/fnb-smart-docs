# 12 — SECURITY & PERMISSION MATRIX

## Security layers
1. Firebase Authentication.
2. Membership.
3. Role.
4. Permission.
5. Store boundary.
6. Firestore Security Rules.
7. App Check.
8. Device binding/revocation where applicable.
9. Audit trail for sensitive actions.

## Permission matrix template
| Permission | Owner | Manager | Staff | Kitchen | Scope | Sensitive? |
|---|---|---|---|---|---|---|
| Menu view | TBD | TBD | TBD | TBD | Store | No |
| Menu edit | TBD | TBD | TBD | TBD | Store | Yes |
| POS order | TBD | TBD | TBD | TBD | Store | Yes |
| Payment | TBD | TBD | TBD | TBD | Store | High |
| Reports | TBD | TBD | TBD | TBD | Store | High |

`TBD` phải được giữ nguyên cho đến khi có nguồn chính thức.
