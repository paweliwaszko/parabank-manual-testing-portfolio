# ParaBank - Test Scenarios

This document contains test scenarios prepared for manual testing of the ParaBank Demo application.

The scenarios are grouped by the functional areas used in TestRail. A total of 45 test cases were created and executed.

## TS-001 - Login

**Purpose:** Check the login functionality with valid and invalid input.

| Case ID | Test Case |
|---|---|
| C46 | Login with valid credentials |
| C47 | Login with invalid password |
| C48 | Login with invalid username |
| C49 | Login with empty username |
| C50 | Login with empty password |
| C51 | Login with SQL injection attempt |
| C52 | Verify successful logout after login |
| C90 | Login with empty username and password |

**Expected result:**  
Valid users can log in successfully. Invalid or incomplete credentials do not allow access to the application.

---

## TS-002 - Registration

**Purpose:** Check user registration with valid, invalid and incomplete data.

| Case ID | Test Case |
|---|---|
| C53 | Register a new user with valid data |
| C54 | Registration with all required fields empty |
| C55 | Registration with mismatched passwords |
| C56 | Registration with an existing username |
| C57 | Registration with empty username |
| C58 | Registration with empty password |

**Expected result:**  
A user can register with valid data. Invalid or incomplete data should be rejected with appropriate validation.

---

## TS-003 - Accounts

**Purpose:** Check account information, transaction history and transaction filtering.

| Case ID | Test Case |
|---|---|
| C59 | View Accounts Overview after successful login |
| C60 | View account details |
| C61 | View transaction history for an account |
| C62 | View transaction details |
| C63 | Filter transactions by activity period |
| C64 | Filter transactions by transaction type |

**Expected result:**  
The user can view account and transaction information and use the available transaction filters.

---

## TS-004 - Fund Transfer

**Purpose:** Check fund transfers between accounts with valid and invalid amounts.

| Case ID | Test Case |
|---|---|
| C65 | Transfer funds between accounts with valid data |
| C66 | Transfer funds with empty amount |
| C67 | Transfer funds with zero amount |
| C68 | Transfer funds with negative amount |
| C69 | Transfer funds with invalid amount format |
| C70 | Transfer funds with valid decimal amount |
| C71 | Transfer funds using the same source and destination account |
| C72 | Transfer amount greater than available balance |
| C73 | Verify account balances after successful fund transfer |
| C74 | Verify transaction history after successful fund transfer |

**Expected result:**  
Valid transfers are processed correctly and reflected in account balances and transaction history. Invalid transfer data should be rejected.

---

## TS-005 - Bill Payment

**Purpose:** Check bill payment functionality with valid and invalid input.

| Case ID | Test Case |
|---|---|
| C75 | Pay a bill with valid data |
| C76 | Bill payment with all required fields empty |
| C77 | Bill payment with mismatched account numbers |
| C78 | Bill payment with zero amount |
| C79 | Bill payment with negative amount |
| C80 | Bill payment with invalid amount format |

**Expected result:**  
Valid bill payments are processed successfully. Invalid or incomplete payment data should be rejected.

---

## TS-006 - Profile & Password

**Purpose:** Check profile information and profile update functionality.

| Case ID | Test Case |
|---|---|
| C81 | Update profile information with valid data |
| C82 | Update profile with required fields empty |
| C83 | Verify current profile information is displayed correctly |
| C84 | Update profile with invalid ZIP code |
| C85 | Verify updated profile data persists after re-login |

**Expected result:**  
Profile information is displayed correctly and valid changes can be saved. Invalid profile data should not be accepted.

---

## TS-007 - Logout & Session

**Purpose:** Check logout behavior and access to protected pages after logout.

| Case ID | Test Case |
|---|---|
| C86 | Successful logout |
| C87 | Access protected page after logout |
| C88 | Access protected page using direct URL after logout |
| C89 | Verify session remains active during authenticated navigation |

**Expected result:**  
The user can log out successfully and protected functionality is not accessible after logout. The session remains active during normal authenticated navigation.

---

## Summary

| Area | Test Cases |
|---|---:|
| Login | 8 |
| Registration | 6 |
| Accounts | 6 |
| Fund Transfer | 10 |
| Bill Payment | 6 |
| Profile & Password | 5 |
| Logout & Session | 4 |
| **Total** | **45** |
