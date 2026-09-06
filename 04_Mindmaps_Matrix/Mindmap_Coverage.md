# Mindmap: ParaBank Testing Coverage

## 1. Authentication Module
- Registration
  - Valid data (TC_001) ✅
  - Duplicate username (TC_002) ⏸️
- Login
  - Valid credentials (TC_003) ✅

## 2. Account Services Module
- Accounts Overview
  - UI Headers check (TC_007) ✅
- Transfer Funds
  - Zero dollar transfer (TC_004) ❌ (Bug Found)
  - Overdraft/Insufficient funds (TC_005) ❌ (Bug Found)
- Bill Pay
  - Payment with $0 balance (TC_006) ❌ (Bug Found)
- Request Loan
  - Rejection with no funds (TC_008) ✅

## 3. Data Validation & Security
- Boundary Value Analysis
  - Amount field ($0.00)
  - Overdraft limits
- Negative Testing
  - Insufficient funds scenarios