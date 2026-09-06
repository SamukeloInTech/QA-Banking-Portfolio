# ParaBank Test Cases

## Test Case ID: TC_Bank_Reg_001
**Title:** Verify successful registration with valid data
**Preconditions:** Browser is open on ParaBank homepage
**Steps:** 1. Click "Register". 2. Fill all fields with valid data. 3. Use unique username (e.g., TesterQA_2026). 4. Click "Register".
**Expected Result:** "Your account was created successfully" message appears.
**Actual Result:** User registered successfully. "Your account was created successfully" message appeared.
**Status:** PASS.

---

## Test Case ID: TC_Bank_Reg_002
**Title:** Verify registration fails with duplicate username
**Preconditions:** User "TesterQA_2026" already exists
**Steps:** 1. Click "Register". 2. Enter same username as TC_001. 3. Click "Register".
**Expected Result:** Error message: "This username already exists."
**Actual Result:** Not Executed (Due to time constraints / focus on high-risk transaction areas)
**Status:** Not Executed

---

## Test Case ID: TC_Bank_Login_003
**Title:** Verify successful login with valid credentials
**Preconditions:** User is already registered (from TC_001)
**Steps:** 1. Go to ParaBank homepage. 2. Enter the registered username. 3. Enter the correct password. 4. Click "Login".
**Expected Result:** User is successfully logged in and redirected to the Accounts Overview page. Welcome message displays the username.
**Actual Result:** User logged in successfully. Welcome message displayed.
**Status:** PASS

---

## Test Case ID: TC_Bank_Transfer_004
**Title:** Verify system blocks a transfer of $0.00
**Preconditions:** Logged in with at least two accounts
**Steps:** 1. Go to "Transfer Funds". 2. Enter $0.00. 3. Select accounts and click "Transfer".
**Expected Result:** Error: "Please enter a valid amount greater than zero."
**Actual Result:** System allowed the transfer. "Transfer Complete! $0.00 has been transferred from account #21780 to account #21780.
**Status:** FAIL.

---

## Test Case ID: TC_Bank_Transfer_005
**Title:** Verify system blocks transfer exceeding balance
**Preconditions:** Logged in. Checking has money.
**Steps:** 1. Go to "Transfer Funds". 2. Enter $100.00. 3. Select Checking to Savings. 4. Click "Transfer".
**Expected Result:** Error: "Insufficient funds in your account."
**Actual Result:** System allowed the transfer. "Transfer Complete!" message appeared for $100.00 even though the balance was $0.00.
**Status:** FAIL.

---

## Test Case ID: TC_Bank_BillPay_006
**Title:** Verify successful bill payment to a merchant
**Preconditions:** Logged in, account has balance > $20
**Steps:** 1. Click "Bill Pay". 2. Enter "Electric Company". 3. Enter address. 4. Enter $20. 5. Click "Send Payment".
**Expected Result:** Success: "Bill Payment Complete". Balance decreases by $20.
**Actual Result:**  System allowed bill payment of $10.00 even though account balance was $0.00. "Bill Payment Complete" message appeared.
**Status:** FAIL.

---

## Test Case ID: TC_Bank_UI_007
**Title:** Verify Accounts Overview table displays correct headers
**Preconditions:** Logged in
**Steps:** 1. Click on "Accounts Overview".
**Expected Result:** Table shows: Account ID, Balance, Available Balance, and Type.
**Actual Result:** Table correctly displays: Account, Balance, Available Amount.
**Status:** PASS.

---

## Test Case ID: TC_Bank_Loan_008
**Title:** Verify loan request is denied when account has $0.00 balance and no payment history
**Preconditions:** Logged in. Account balance is $0.00.
**Steps:** 
1. Click on "Request Loan" in the left-hand menu.
2. Enter Loan Amount: $1000.00
3. Enter Down Payment: $0.00
4. Select "From Account" (Checking account #21780).
5. Click the "Apply Now" button.

**Expected Result:** Loan is rejected. Error message appears: "You do not have sufficient funds" OR "Loan cannot be processed due to insufficient funds." The loan should NOT be approved.

**Actual Result:**  Loan was rejected. Error message appeared: "We cannot grant a loan in that amount with your available funds."
**Status:** PASS.