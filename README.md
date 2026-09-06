# 🏦 QA Portfolio: ParaBank Banking Application Testing

**Tester:** SAMUKELO CELE
**Project Type:** Manual Functional Testing  
**Application URL:** https://parabank.parasoft.com/

---

## 📝 Project Overview
This project demonstrates a complete manual testing cycle on the ParaBank online banking demo application. The goal was to validate core financial features, identify critical defects, and document them in a structured, professional manner suitable for an internship or junior QA role.

---

## 📊 Testing Summary
- **Total Test Cases Written:** 8
- **Test Cases Executed:** 7
- **Passed:** 4
- **Failed:** 3 (Critical/Major Bugs found)
- **Critical Bugs Found:** 2 (Overdraft/Zero balance fraud)
- **Major Bugs Found:** 1 ($0.00 transfer logic)

---

## 🐛 Top 3 Bugs Discovered
1. **BUG_002 (Critical):** System allows transfer of money with a $0.00 balance (Creates money out of thin air).
2. **BUG_003 (Critical):** System allows Bill Payment with a $0.00 balance.
3. **BUG_001 (Major):** System allows $0.00 transfers to the same account.

---

## 📂 Project Structure (What's inside?)
| Folder | Contents |
| :--- | :--- |
| **01_Test_Plan_Scope** | Test Scope (Plan) and Test Summary Report (Final Verdict) |
| **02_Test_Cases** | 8 detailed test cases with Pass/Fail statuses |
| **03_Bug_Reports** | 3 professional JIRA-style bug reports with screenshots |
| **04_Mindmaps_Matrix** | Coverage mindmap and Traceability Matrix (RTM) |
| **05_Screenshots** | Visual evidence of all bugs found |

---

## 🎯 How to Navigate This Portfolio
1. Start with the **`Test_Summary.md`** in the `01_Test_Plan_Scope` folder to see the final verdict.
2. Review the **Bug Reports** in the `03_Bug_Reports` folder to understand the critical issues found.
3. Check the **Traceability Matrix** in `04_Mindmaps_Matrix` to see how tests map to requirements.

---

## 💡 Skills Demonstrated
- Test Case Design (Equivalence Partitioning & Boundary Value Analysis)
- Functional & Negative Testing
- Defect Reporting (Severity/Priority)
- Requirement Traceability
- Agile/QA Documentation