# Test Plan & Scope: ParaBank Online Banking

## 1. Project Overview
- **Application:** ParaBank (https://parabank.parasoft.com/)
- **Tester:** SAMUKELO CELE
- **Objective:** To validate the core financial functionalities of the banking system and identify critical defects before release.

## 2. Features In-Scope 
- **Authentication:** User Registration (Valid/Invalid) and Login.
- **Core Banking:** Transfer Funds (functional & negative testing).
- **Bills & Payments:** Bill Pay functionality.
- **Loan Management:** Loan request processing and validation.
- **User Interface:** Verification of dashboard elements and account overview.

## 3. Features Out-of-Scope
- **Mobile Responsiveness:** Testing on phones/tablets.
- **API/Backend Testing:** Direct database or API calls.
- **Performance/Load Testing:** How the site behaves under heavy user traffic.
- **Visual UI Design:** Checking font sizes or color contrast.

## 4. Testing Approach & Techniques
- **Equivalence Partitioning:** Testing valid vs. invalid input groups (e.g., $10 vs $-5).
- **Boundary Value Analysis:** Testing edge cases like $0.00.
- **Negative Testing:** Attempting actions that should fail (e.g., overdrafts).
- **Environment:** Windows 11, Google Chrome (Latest Version).