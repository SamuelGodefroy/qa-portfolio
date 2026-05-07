# AC-TC-UI_FRONT-001

## Metadata
* **Title**: Sending a private message to a user
* **Module**: UI_FRONT
* **Priority**: High
* **Created By**: Aleksei Nikolaev
* **Date**: 2026-05-03


## Objective

Verification of sending a message in a private chat

## Preconditions
1. Website https://agentstack.tech/messenger is open
2. Valid account is authorized

## Test Data
* Email: `test@example.com`
* Password: `TestPass123!`

## Steps

| # | Action | Expected Result | Actual Result
|---| :--- | :--- | :--- |
| 1 | Open website: https://agentstack.tech/ | Main page https://agentstack.tech/ loads successfully | - |
| 2 | Click on "Messenger" | Opens https://agentstack.tech/messenger | - |
| 3 | Select a chat from the "All Chats" folder | The selected chat opens |  |
| 4 | Tap on the chat input field | **Input field is active, text entry is available** | - [x] -  |
| 5 | Enter text | Text appears in the input field | - |
| 6 | Click the "Send" button | **Message is sent, new message is visible within the user's viewport** | [x] Fail |

## Status
- [ ] Pass
- [x] Fail (Link to Bug Report: (https://github.com/SamuelGodefroy/qa-portfolio/edit/main/projects/AgentChat/bug-reports/AC-BUG-UI_FRONT-001.md))
- [ ] Blocked
- [ ] Skipped

## Environment

* **Environment**: OS: iOS 26.4.2, Browser: Chrome 189.110.145.218, Device: iPhone 15 Plus

## Attachments

projects/AgentChat/assets/AC-ASSETS-UI_FRONT-001.md
