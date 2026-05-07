# AS-TC-FUNC_AUTH-001

## Metadata
* **Title**: User registration
* **Priority**: Critical
* **Created By**: Aleksei Nikolaev
* **Date**: 2026-05-07

## Objective
Verification of new user registration in the positive scenario

## Preconditions
1. Site [https://agentstack.tech/](https://agentstack.tech/) is open
2. User is not logged in

## Test Data
* Email: `[test@example.com]`
* Password: `[TestPass123!]`


## Steps

| # | Action | Expected Result | Actual Result |
|---| :--- | :--- | :--- |
| 1 | Click on the "Sign in" icon/button | The user authentication window opens with "Email", "Password" fields and "Sign in", "Registration", "Sign in via API key" icons/buttons | - |
| 2 | Click on the "Registration" icon/button | The registration window opens with "Email", "Password", "Inviter code" (for the referral system) fields | - |
| 3 | Enter valid data into the "Email" field | The entered data is displayed in the text field | - |
| 4 | Enter valid data into the "Password" field | The "Password" field displays "dots" hiding the entered password | - |
| 5 | Click on the "Registration" icon/button | The user is registered, the dashboard opens | - |

## Status
- [x] Pass
- [ ] Fail 
- [ ] Blocked
- [ ] Skipped

## Environment
* **Environment**: OS: Windows 10, Browser: Chrome 147.0.7727.102, Device: Desktop
