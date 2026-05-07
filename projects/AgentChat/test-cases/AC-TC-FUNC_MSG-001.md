# AC-TC-FUNC_MSG-001

## Metadata
* **Title**: Sending a private message to a user
* **Priority**: Critical
* **Created By**: Aleksei Nikolaev
* **Date**: 2026-05-06

## Objective
Verification of the message sending functionality

## Preconditions

1. Page https://agentstack.tech/messenger is open
2. User is authorized

## Test Data
* Email: `[test@example.com]`
* Password: `[TestPass123!]`

## Steps

| # | Action | Expected Result | Actual Result |
|---| :--- | :--- | :--- |
| 1 | Enter test message in the text field: "Test_123"| Text field displays: "Test_123" | - |
| 2 | Click on the "Send" icon/button | Message is sent, a "Delivered" checkmark is present below the message | - |

## Status
- [x] Pass
- [ ] Fail 
- [ ] Blocked
- [ ] Skipped

## Environment
* **Environment**: OS: Windows 11, Browser: Chrome 147.0.7727.102, Device: Desktop

## Attachments
