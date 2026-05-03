# AC-BUG-UI_FRONT-001

> **Summary:** Chat input field shifts to the top of the screen on iOS Chrome browser
> **Example:** *When tapping the chat input field, the entire chat interface scrolls up, leaving the input field stuck at the top edge of the screen.*

| Field | Value |
| :--- | :--- |
| **ID** | #5 |
| **Status** | `New` |
| **Severity** | `Low` |
| **Priority** | `P3 (Medium)` |
| **Environment** | OS: iOS 26.4.2, Browser: Chrome 189.110.145.218, Device: iPhone 15 Plus |
| **Build/Version** | actual |
| **Author** | Aleksei Nikolaev |
| **Date Reported** | 2026-05-02 |
| **Linked TC** | **None** 

---

## Description

In the Chrome browser on iOS, tapping the chat input field causes the entire chat interface to scroll upwards. The input field remains fixed at the top edge of the screen, causing layout issues.

## Steps to Reproduce

| # | Action | Expected Result | Actual Result |
|---| :--- | :--- | :--- |
| 1 | Open website: https://agentstack.tech/ | Main page https://agentstack.tech/ loads successfully | - |
| 2 | Click on "Messenger" | Opens https://agentstack.tech/messenger | - |
| 3 | Select a chat from the "All Chats" folder | The selected chat opens | - |
| 4 | Tap on the chat input field | **Input field is active, text entry is available** | **FAILED: The page scrolls up abruptly. The input field remains stuck at the very top of the screen. Text entry is available but UI is broken.** |
| 5 | Enter text | Text appears in the input field | - |
| 6 | Click the "Send" button | **Message is sent, new message is visible within the user's viewport** | **FAILED:** **The sent message remains outside the visible area (above the top edge). The input field also remains stuck at the top.** |

## Actual vs Expected
**Expected:** When tapping the message input field, it behaves stably. The input field remains in its original position. Messages remain readable. The sent message is visible and stays within the user's viewport.

**Actual:** When tapping the message input field, it shifts the entire chat interface upwards. The input field moves to the top edge of the device screen. Messages become unreadable. The sent message is not visible and is located outside the user's viewport.

## Impact Assessment
- [ ] Critical: System unusable  
- [ ] High: Core functionality broken
- [ ] Medium: User experience degraded, workaround exists
- [x] Low: Cosmetic issue
- [x] Frequency: 100% reproducible
- [x] Workaround: Manual scroll down to restore the interface to its original position

## Incident Category
- [x] Functional defect
- [x] UI/UX issue
- [ ] Performance degradation
- [x] Configuration problem
- [ ] Compatibility issue
- [ ] Documentation error

## Attachments

projects/AgentChat/assets/AC-ASSETS-UI_FRONT-001.md
