# AC-BUG-FUNC_MSG-002

>**Summary:** Deleting sent messages by the user
>
>**Example:** When the user attempts to delete a message, they receive a "Not found 404" error.

| Field | Value |
| :--- | :--- |
| **Status** | New|
| **Severity** | Major |
| **Priority** | Low |
| **Environment** | OS: Windows 10, Browser: Chrome 147.0.7727.102, Device: Desktop|
| **Build/Version** | Actual |
| **Author** | Aleksei Nikolaev |
| **Date Reported** | 2026-05-06|
| **Linked TC** | https://github.com/SamuelGodefroy/qa-portfolio/blob/main/projects/AgentChat/test-cases/AC-TC-FUNC_MSG-002.md |

---

## Description

When attempting to delete previously sent messages, the user receives a "Not found 404" error.

## Steps to Reproduce

| # | Action | Expected Result | Actual Result |
|---| :--- | :--- | :--- |
| 1 | Right-click on the sent message | A dropdown menu appears | - |
| 2 | Click "Delete message" | The message is deleted for the user | **FAILED: The user receives a "Not found 404" error.** |


## Actual vs Expected
**Expected:** The user's message is deleted.
**Actual:** The user's message remains in the chat.

## Impact Assessment
- [ ] Critical: System unusable (the entire project is down)
- [ ] High: Core functionality broken (main feature is not working)
- [x] Medium: User experience degraded, workaround exists (functionality works but is inconvenient)
- [ ] Low: Cosmetic issue (minor UI distortions)
- [x] Frequency: 100%
- [ ] Workaround: None

## Incident Category
- [x] Functional defect
- [ ] UI/UX issue
- [ ] Performance degradation
- [ ] Configuration problem
- [ ] Compatibility issue
- [ ] Documentation error

## Attachments
