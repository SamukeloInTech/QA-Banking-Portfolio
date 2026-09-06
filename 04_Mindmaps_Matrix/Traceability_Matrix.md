# Traceability Matrix (RTM): ParaBank

| Requirement ID | Business Requirement | Test Case ID | Bug ID | Status |
| :--- | :--- | :--- | :--- | :--- |
| REQ_AUTH_01 | User must register with unique credentials | TC_001 | - | PASS |
| REQ_AUTH_01 | User must register with unique credentials | TC_002 | - | Not Executed |
| REQ_AUTH_02 | User must log in with valid credentials | TC_003 | - | PASS |
| REQ_TRANS_01 | System must validate transfer amounts | TC_004 | BUG_001 | FAIL |
| REQ_TRANS_02 | System must prevent overdrafts (Balance checks) | TC_005 | BUG_002 | FAIL |
| REQ_BILL_01 | System must validate bill pay against balance | TC_006 | BUG_003 | FAIL |
| REQ_UI_01 | Account overview must display correct columns | TC_007 | - | PASS |
| REQ_LOAN_01 | Loan requests must check available funds | TC_008 | - | PASS |

**Summary:**
- **Total Requirements mapped:** 7
- **Passed:** 4
- **Failed (Bugs found):** 3
- **Not Executed:** 1
- **Coverage:** 100% of critical banking features tested.