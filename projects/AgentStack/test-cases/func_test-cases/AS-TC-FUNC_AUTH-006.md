# AS-TC-FUNC_AUTH-006

## Metadata
* **Title**: Registration of a user with invalid data
* **Priority**: Critical
* **Created By**: Aleksei Nikolaev
* **Date**: 2026-05-07

## Objective

Negative scenario of entering invalid data

## Preconditions
1. Site [https://agentstack.tech/](https://agentstack.tech/) is open
2. User is not logged in
3. User is not registered

## Test Data
* Email: `[test1@example.com]`
* Password: `[1]`


## Steps

| # | Action | Expected Result | Actual Result |
|---| :--- | :--- | :--- |
| 1 | Click on the "Sign in" icon/button | The user authentication window opens with "Email", "Password" fields and "Sign in", "Registration", "Sign in via API key" icons/buttons | - |
| 2 | Click on the "Registration" icon/button | The registration window opens with "Email", "Password", "Inviter code" (for the referral system) fields | - |
| 3 | Enter valid data into the "Email" field | The entered data is displayed in the text field | - |
| 4 | Enter one character "1" into the "Password" field | The "Password" field displays "dots" hiding the entered password | - |
| 5 | Click on the "Registration" icon/button | Registration error. Password cannot contain only one character | - |

## Status
- [ ] Pass
- [x] Fail https://github.com/SamuelGodefroy/qa-portfolio/blob/main/projects/AgentStack/bug-reports/AS-BUG-FUNC_AUTH-006.md
- [ ] Blocked
- [ ] Skipped

## Environment
* **Environment**: OS: Windows 10, Browser: Chrome 147.0.7727.102, Device: Desktop
