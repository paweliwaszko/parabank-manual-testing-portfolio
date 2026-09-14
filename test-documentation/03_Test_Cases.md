# ParaBank - Test Cases

This document contains an overview of the manual test cases prepared for the ParaBank Demo application.

A total of **45 test cases** were created and executed in TestRail. Detailed test cases, including preconditions, test steps and expected results, are available in the TestRail export included in this repository.

## 01 - Login

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

## 02 - Registration

| Case ID | Test Case |
|---|---|
| C53 | Register a new user with valid data |
| C54 | Registration with all required fields empty |
| C55 | Registration with mismatched passwords |
| C56 | Registration with an existing username |
| C57 | Registration with empty username |
| C58 | Registration with empty password |

## 03 - Accounts

| Case ID | Test Case |
|---|---|
| C59 | View Accounts Overview after successful login |
| C60 | View account details |
| C61 | View transaction history for an account |
| C62 | View transaction details |
| C63 | Filter transactions by activity period |
| C64 | Filter transactions by transaction type |

## 04 - Fund Transfer

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

## 05 - Bill Payment

| Case ID | Test Case |
|---|---|
| C75 | Pay a bill with valid data |
| C76 | Bill payment with all required fields empty |
| C77 | Bill payment with mismatched account numbers |
| C78 | Bill payment with zero amount |
| C79 | Bill payment with negative amount |
| C80 | Bill payment with invalid amount format |

## 06 - Profile & Password

| Case ID | Test Case |
|---|---|
| C81 | Update profile information with valid data |
| C82 | Update profile with required fields empty |
| C83 | Verify current profile information is displayed correctly |
| C84 | Update profile with invalid ZIP code |
| C85 | Verify updated profile data persists after re-login |

> Note: The TestRail section retains the name "Profile & Password", although the tested version of ParaBank does not provide password-change functionality.

## 07 - Logout & Session

| Case ID | Test Case |
|---|---|
| C86 | Successful logout |
| C87 | Access protected page after logout |
| C88 | Access protected page using direct URL after logout |
| C89 | Verify session remains active during authenticated navigation |

## Test design

The test cases include:

- positive and negative testing
- Equivalence Partitioning
- Boundary Value Analysis
- input validation
- error guessing
- exploratory testing

## Summary

| Section | Test Cases |
|---|---:|
| Login | 8 |
| Registration | 6 |
| Accounts | 6 |
| Fund Transfer | 10 |
| Bill Payment | 6 |
| Profile & Password | 5 |
| Logout & Session | 4 |
| **Total** | **45** |

Detailed test cases and execution evidence are available in the [TestRail folder](../testrail/).

Test execution results are available in the [Test Summary Report](./04_Test_Summary_Report.md).

Defects found during testing are documented in [Bug Reports](../bug-reports/).
