# AS-BUG-UI_THEME-004

> **Summary:** After the logout-login cycle, the theme resets to the browser theme.
> **Example:** *Selected "Light" → after logout/login: browser theme + toggle "Auto"*

| Field | Value |
| :--- | :--- |
| **Status** | `New` |
| **Severity** | `Low` |
| **Priority** | `P4 (Low)` |
| **Environment** | OS: Windows 10, Browser: Chrome 147.0.7727.102, Device: Desktop |
| **Build/Version** | actual |
| **Author** | Aleksei Nikolaev |
| **Date Reported** | 2026-04-29 |
| **Linked TC** | **AS-TC-UI_LANGUAGE-004** 

---

## Description
After the logout-login cycle, the theme resets to the browser's default theme. In the profile menu, the selection resets to "System".

## Steps to Reproduce

| # | Action | Expected Result | Actual Result |
|---|--------|-----------------|---------------|
| 1 | Login with test data | Homepage loads | - |
| 2 | Click Profile → Theme | Dropdown opens | - |
| 3 | Select "Light" theme | UI switches to Light | - |
| 4 | Refresh page (F5) | Light theme persists | - |
| 5 | Click "Logout" | Login screen appears | - |
| 6 | Enter email | Email field populated | - |
| 7 | Enter password | Password field populated | - |
| 8 | Click "Login" | User logged in | - |
| 9 | Verify theme website | **The website theme should be set to Light** | **FAILED: The website reset on the dark theme**
| 10 | Check theme toggle | **Toggle shows "Light"** | **FAILED: Toggle reset to "Auto"** |

## Actual vs Expected
**Expected:** The theme is preserved as selected by the user in the profile after the logout-login cycle. 

**Actual:** The theme resets to browser default on login

## Impact Assessment
- [ ] Critical: System unusable  
- [ ] High: Core functionality broken
- [ ] Medium: User settings lost, workaround exists
- [x] Low: Cosmetic issue
- [x] Frequency: 100% reproducible
- [x] Workaround: Reselect theme after each login

## Incident Category
- [ ] Functional defect
- [x] UI/UX issue
- [ ] Performance degradation
- [ ] Configuration problem
- [ ] Compatibility issue
- [ ] Documentation error

## Attachments
