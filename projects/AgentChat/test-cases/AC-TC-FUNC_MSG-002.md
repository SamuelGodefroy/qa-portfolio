# AC-TC-FUNC_MSG-002

## Metadata
* **Title**: Delete messages
* **Priority**: Critical
* **Created By**: Aleksei Nikolaev
* **Date**: 2026-05-06

## Objective
Verification of deleting sent messages

## Preconditions

1. Page https://agentstack.tech/messenger is open
2. User is authorized
3. Есть отправленные сообщения пользователю

## Test Data
* Email: `[test@example.com]`
* Password: `[TestPass123!]`

## Steps

| # | Action | Expected Result | Actual Result |
|---| :--- | :--- | :--- |
| 1 | Right-click on the sent message | A dropdown menu appears | - |
| 2 |Click "Delete message" | The message is deleted for the user | **Fail** |

## Status
- [ ] Pass
- [x] Fail 
- [ ] Blocked
- [ ] Skipped

## Environment
* **Environment**: OS: Windows 11, Browser: Chrome 147.0.7727.102, Device: Desktop

## Attachments
