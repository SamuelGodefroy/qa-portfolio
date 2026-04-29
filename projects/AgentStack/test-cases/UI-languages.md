# Test Case ID: AS-TC-UI_LANGUAGE-001

## Metadata
* **Title**: Verify Language Persistence After Logout/Login
* **Module**: UI Language
* **Priority**: Medium
* **Created By**: Aleksei Nikolaev
* **Date**: 2026-04-28

## Objective
Verify language setting persists after logout/login cycle.

## Preconditions
1. Browser language set to Russian (OS level).
2. Valid test account exists.

## Test Data
* Email: `test@example.com`
* Password: `TestPass123!`

## Steps
| # | Action | Expected Result | Actual Result |
|---| :--- | :--- | :--- |
| 1 | Login with test data | Homepage opens in Russian | - |
| 2 | Click Profile Icon → Language | Dropdown menu opens | - |
| 3 | Select "English (US)" | UI switches to English | - |
| 4 | Refresh page (F5) | Language remains English | - |
| 5 | Click "Logout" | Login screen appears | - |
| 6 | Enter email: `test@example.com` | Email field populated | - |
| 7 | Enter password: `TestPass123!` | Password field populated | - |
| 8 | Click "Login" | **UI in English** | **FAILED: UI remained Russian** |
| 9 | Check language toggle (Step 2) | **Toggle shows "English (US)"** | **FAILED: Toggle stayed on "Auto"** |

## Status
- [ ] Pass
- [x] Fail (Link to Bug Report: [Issue #XXX])

## Environment / Notes
* **Environment**: Chrome 147.0.7727.102, Windows 10

---
---

# Test Case ID: AS-TC-UI_LANGUAGE-002

## Metadata
* **Title**: Verify Language Persistence After Logout/Login
* **Module**: UI Language
* **Priority**: Medium
* **Created By**: Aleksei Nikolaev
* **Date**: 2026-04-28

## Objective
Verify language setting persists after logout/login cycle.

## Preconditions
1. Browser language set to Russian (OS level).
2. Valid test account exists.

## Test Data
* Email: `test@example.com`
* Password: `TestPass123!`

## Steps
| # | Action | Expected Result | Actual Result |
|---| :--- | :--- | :--- |
| 1 | Login with test data | Homepage opens in Russian | - |
| 2 | Click Profile Icon → Language | Dropdown menu opens | - |
| 3 | Select "Portuguese (PT)" | UI switches to Portuguese | - |
| 4 | Refresh page (F5) | Language remains Portuguese | - |
| 5 | Click "Logout" | Login screen appears | - |
| 6 | Enter email: `test@example.com` | Email field populated | - |
| 7 | Enter password: `TestPass123!` | Password field populated | - |
| 8 | Click "Login" | **UI in Portuguese** | **FAILED: UI remained Russian** |
| 9 | Check language toggle (Step 2) | **Toggle shows "Portuguese (PT)"** | **FAILED: Toggle stayed on "Auto"** |

## Status
- [ ] Pass
- [x] Fail (Link to Bug Report: [Issue #XXX])

## Environment / Notes
* **Environment**: Chrome 147.0.7727.102, Windows 10
* **Notes**: None

---
---

# Test Case ID: AS-TC-UI_LANGUAGE-003

## Metadata
* **Title**: Verify Language Persistence After Logout/Login
* **Module**: UI Language
* **Priority**: Medium
* **Created By**: Aleksei Nikolaev
* **Date**: 2026-04-28

## Objective
Verify language setting persists after logout/login cycle.

## Preconditions
1. Browser language set to Russian (OS level).
2. Valid test account exists.

## Test Data
* Email: `test@example.com`
* Password: `TestPass123!`

## Steps
| # | Action | Expected Result | Actual Result |
|---| :--- | :--- | :--- |
| 1 | Login with test data | Homepage opens in Russian | - |
| 2 | Click Profile Icon → Language | Dropdown menu opens | - |
| 3 | Select "Russian (RU)" | UI switches to Russian | - |
| 4 | Refresh page (F5) | Language remains Russian | - |
| 5 | Click "Logout" | Login screen appears | - |
| 6 | Enter email: `test@example.com` | Email field populated | - |
| 7 | Enter password: `TestPass123!` | Password field populated | - |
| 8 | Click "Login" | UI in Russian | - |
| 9 | Check language toggle (Step 2) | **Toggle shows "Russian (RU)"** | **FAILED: Toggle stayed on "Auto"** |

## Status
- [ ] Pass
- [x] Fail (Link to Bug Report: [Issue #XXX])

## Environment / Notes
* **Environment**: Chrome 147.0.7727.102, Windows 10
