# F&B SMART V5.1 — COMPLETE PRODUCT DEVELOPMENT DOCUMENTATION
## Bộ tài liệu tham khảo hoàn chỉnh

**Mục đích:** tạo một bộ hồ sơ mà một người mới vào dự án có thể lần lượt hiểu:
Product → Feature → Screen → Flow → Business Rule → State → Data → Security → Architecture → Work Item → Test → Build → PO Verification → Protection → Lock → Operations.

> **QUAN TRỌNG:** Bộ này là bộ tham khảo/chuẩn hóa tài liệu. Nó KHÔNG thay thế KIM CHỈ NAM, Product Charter, Database Schema, State Machines hoặc các quyết định PO đã được ghi chính thức.

### Thứ tự nguồn
1. `boquytacfnb/00_KIM_CHI_NAM/*` — Governance cao nhất.
2. Các hợp đồng chuyên môn V5.1 đã được PO chấp thuận.
3. Hồ sơ trạng thái, quyết định, checkpoint, protection/evidence.
4. Product discovery/specification đã được PO xác nhận hoặc khóa.
5. Bộ tài liệu này.
6. Implementation của Coding Agent.

### Nguyên tắc
- Không suy đoán yêu cầu còn thiếu.
- Không biến `DRAFT`, `PROPOSED`, `TBD` thành quyết định chính thức.
- Không biến technical PASS thành PO_VERIFIED.
- Không để database/repository tự quyết định giao diện.
- Mọi Feature có UI phải có Screen ID, Entry Point, Flow và PO Acceptance.
- Foundation/Data-only Work Item phải ghi rõ kết quả người dùng nhìn thấy có hay chưa.

## Cấu trúc bộ tài liệu
| ID | Tài liệu | Câu hỏi trả lời |
|---|---|---|
| 01 | Product Charter & Scope | Sản phẩm là gì? |
| 02 | Product Requirements | Phải làm gì? |
| 03 | Feature Registry | Có những tính năng nào? |
| 04 | Roadmap & Work Item Map | Làm theo thứ tự nào? |
| 05 | UX/UI & Screen Registry | Người dùng nhìn thấy gì? |
| 06 | Navigation & User Flows | Người dùng đi như thế nào? |
| 07 | Business Rules | Hệ thống xử lý thế nào? |
| 08 | State Machines | Trạng thái chuyển ra sao? |
| 09 | Architecture | Hệ thống được xây thế nào? |
| 10 | Repository/API Contracts | Các lớp giao tiếp ra sao? |
| 11 | Database/Data Dictionary | Dữ liệu ở đâu? |
| 12 | Security/Permission | Ai được làm gì? |
| 13 | Test & Acceptance | Chứng minh đúng thế nào? |
| 14 | Feature Traceability | Một Feature nối toàn bộ chuỗi thế nào? |
| 15 | Build/Release | APK nào từ source nào? |
| 16 | Operations/Recovery | Sau phát hành xử lý thế nào? |
| 17 | Risk/Issue/Regression | Rủi ro và lỗi được kiểm soát thế nào? |
| 18 | Decision & Change Control | Ai quyết định thay đổi? |
| 19 | Work Item Template | Mỗi task phải cam kết gì? |
| 20 | Documentation Governance | Tài liệu được quản lý ra sao? |
| 21 | Menu Product Blueprint | Menu phải xuất hiện ở đâu và theo luồng nào? |
| 22 | PO Acceptance Handbook | Tuấn kiểm tra chức năng thế nào? |
| 23 | Glossary | Thuật ngữ thống nhất là gì? |
| 24 | New Agent Read-First | Codex/Gemini phải đọc gì trước? |

## Chuỗi truy nguyên bắt buộc

`Requirement → Feature → Screen → User Flow → Business Rule → State → Data → Permission → Repository → Work Item → Test → Build → PO Test → PO_VERIFIED → Regression → PROTECTED → LOCKED`

## Phân loại trạng thái tài liệu
- **OFFICIAL / LOCKED:** nguồn đã được bảo vệ.
- **PO CONFIRMED:** đã có xác nhận PO.
- **FINAL DRAFT / PO REVIEW REQUIRED:** chưa được coi là quyết định cuối.
- **REFERENCE:** chỉ tham khảo.
- **PROPOSED / TBD:** chưa được phép biến thành requirement.
- **HISTORICAL:** chỉ dùng để hiểu lịch sử.
