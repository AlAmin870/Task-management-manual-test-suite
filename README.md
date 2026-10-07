# Manual Test Suite — Task Management Module

A complete manual test suite for an enterprise task-management web application. It has **513 test cases** across 3 sub-modules and 23 test categories, each with preconditions, steps, test data, expected and actual results, priority, severity, environment and execution date.

📄 **[Open the test cases (Excel)](test-cases/Task_Management_TestCases.xlsx)**: the `Task Management_TestCases` sheet holds the cases, and `Test Coverage Summary` is a pivot by sub-module and status.

## Execution results

| Metric | Value |
|---|---|
| Test cases designed | 513 |
| Executed | 507 |
| Passed | 507 (100% of executed) |
| Failed | 0 |
| Not applicable | 6: bulk import/export and bulk-selection features not yet built, kept as ready-made cases for a future release |

## Coverage

| Sub-module | Test cases |
|---|---|
| Basic Setup (developers, support teams, priorities, task types) | 323 |
| Regular Activities (creating, assigning and tracking tasks) | 130 |
| Reports | 60 |
| **Total** | **513** |

**By test category** (top 10 of 23)

| Category | Cases | Category | Cases |
|---|---|---|---|
| Functional | 207 | Performance | 20 |
| UI/UX | 69 | Usability | 19 |
| Validation | 41 | Negative | 16 |
| Security | 35 | Compatibility | 14 |
| Integration | 27 | Data Integrity | 10 |

The other categories are Audit, Edge Case, Concurrency, API Testing, System, Boundary, Error Handling, Business Rule, Business Logic, Privacy, API Security, Calculation and Enhancement.

**By risk**

| Priority | Cases | Severity | Cases |
|---|---|---|---|
| High | 205 | Critical | 17 |
| Medium | 244 | High | 161 |
| Low | 64 | Medium | 205 |
| | | Low | 130 |

## Test design techniques used

- **Boundary and limit testing:** character limits, long inputs and empty results.
- **Negative testing:** invalid formats, missing required fields, duplicate codes.
- **Security checks:** role-based access, unauthorised actions, input sanitisation.
- **Cross-browser and mobile checks:** layout and behaviour on several browsers and on mobile.
- **Traceability:** every case is linked to a module and sub-module, so coverage gaps are visible in the pivot summary.

## Test case template

| Field | Purpose |
|---|---|
| Test Case ID | Unique ID per sub-module (e.g. `TC_DEV_001`) |
| Title, Module, Sub-Module, Category | What is tested and where |
| Description, Preconditions | Context and required starting state |
| Test Steps, Test Data | Exact steps and input values |
| Expected Result, Actual Result | Pass/fail evidence |
| Postconditions | State after the test |
| Priority, Severity | Business importance and impact if it fails |
| Status, Execution Date, Environment | Execution record |
| Comments | Notes, e.g. why a case is not applicable |
