# AS-TC-FUNC_AUTH-004

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
* Password: `[TestPass123!]`


## Steps

| # | Action | Expected Result | Actual Result |
|---| :--- | :--- | :--- |
| 1 | Click on the "Sign in" icon/button | The user authentication window opens with "Email", "Password" fields and "Sign in", "Registration", "Sign in via API key" icons/buttons | - |
| 2 | Click on the "Registration" icon/button | The registration window opens with "Email", "Password", "Inviter code" (for the referral system) fields | - |
| 3 | Enter a valid "Email" into the "Email" field | The entered data is displayed in the text field | - |
| 4 | Leave the "Password" field empty | The "Password" field is empty | - |
| 5 | Click on the "Registration" icon/button | Registration error. The "password" field cannot be empty | - |

## Status
- [x] Pass
- [ ] Fail 
- [ ] Blocked
- [ ] Skipped

## Environment
* **Environment**: OS: Windows 10, Browser: Chrome 147.0.7727.102, Device: Desktop
