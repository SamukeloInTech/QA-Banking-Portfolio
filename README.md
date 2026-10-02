# 🏦 QA Portfolio: ParaBank Banking Application Testing

**Tester:** Samukelo Cele
**Project type:** Manual functional testing
**Application under test:** [ParaBank](https://parabank.parasoft.com/) (demo online banking app)
**Contact:** [LinkedIn](https://www.linkedin.com/in/samukelo-cele) · [Email](mailto:samkeloacele@gmail.com)

---

## 📝 Project Overview

This project is a complete manual testing cycle on ParaBank, a demo banking application. The goal was to validate core financial features (account overview, fund transfers and bill payments), find defects, and document everything the way a QA team would: scope, test cases, bug reports, traceability and a final summary.

> **Note:** ParaBank is a demo application built for testing practice, so some of its behaviour may be simplified compared with a real banking system. Findings below are reported as I observed them during my test sessions.

---

## 🧪 Test Environment

| Item | Detail |
| --- | --- |
| Application | ParaBank (https://parabank.parasoft.com/) |
| Browser | [e.g. Chrome, version ___] |
| Operating system | [e.g. Windows 11] |
| Test dates | [e.g. Month Year] |
| Tools | [e.g. Jira for bug tracking, Excel/Markdown for test cases, XMind for mindmap] |

---

## 📊 Testing Summary

| Metric | Result |
| --- | --- |
| Test cases written | 8 |
| Test cases executed | 7 |
| Passed | 4 |
| Failed | 3 |
| Not executed | 1 — [reason, e.g. blocked by BUG_00X / out of scope] |

**Defects found:** 3 in total
- 2 Critical
- 1 Major

---

## 🐛 Defects Found

| ID | Title | Severity | Feature |
| --- | --- | --- | --- |
| BUG_002 | Funds transfer is allowed when the account balance is $0.00 | Critical | Transfer Funds |
| BUG_003 | Bill payment is allowed when the account balance is $0.00 | Critical | Bill Pay |
| BUG_001 | $0.00 transfer to the same account is accepted | Major | Transfer Funds |

Each bug report includes steps to reproduce, expected vs actual result, severity/priority, and screenshot evidence.

**Why these severity ratings?**
- BUG_002 and BUG_003 are rated **Critical** because the system lets a transaction go through with no available funds, which is a core financial-integrity failure in a real banking system.
- BUG_001 is rated **Major** because the system accepts a meaningless transaction with no validation, but there is no loss of funds. [Adjust this explanation to match your own reasoning.]

---

## 📂 Project Structure

| Folder | Contents |
| --- | --- |
| `01_Test_Plan_Scope` | Test scope (plan) and Test Summary Report |
| `02_Test_Cases` | 8 detailed test cases with pass/fail status |
| `03_Bug_Reports` | 3 Jira-style bug reports with screenshots |
| `04_Mindmaps_Matrix` | Coverage mindmap and Requirements Traceability Matrix (RTM) |
| `05_Screenshot` | Visual evidence for the bugs found |

---

## 🎯 How to Navigate This Portfolio

1. Start with **`Test_Summary.md`** in `01_Test_Plan_Scope` for the final verdict.
2. Read the **bug reports** in `03_Bug_Reports` to see the critical issues and evidence.
3. Open the **Traceability Matrix** in `04_Mindmaps_Matrix` to see how each test maps to a requirement.

---

## 💡 Skills Demonstrated

- Test case design using Equivalence Partitioning and Boundary Value Analysis
- Functional and negative testing
- Defect reporting with severity and priority
- Requirements traceability (RTM)
- Test planning, scoping and summary reporting
- Clear QA documentation in an Agile-style workflow

---

## 🚀 What I Would Do Next

- Add **API testing** of the ParaBank REST services using Postman (with assertions and an exported collection)
- **Automate** the regression suite for the transfer and bill-pay flows with Playwright or Selenium
- Add **non-functional checks** such as basic performance and security testing of the login and transaction flows
- Retest all defects after fixes and update the traceability matrix

---

## 📬 Contact

- **LinkedIn:** [linkedin.com/in/samukelo-cele](https://www.linkedin.com/in/samukelo-cele)
- **Email:** samkeloacele@gmail.com
