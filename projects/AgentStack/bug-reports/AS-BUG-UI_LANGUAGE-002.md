# AS-BUG-UI_LANGUAGE-002

> **Summary:** Language resets to Russian after logout/login cycle
> **Example:** *Selected "Portuguese (PT)" → after logout/login: Russian + toggle "Auto"*

| Field | Value |
| :--- | :--- |
| **Status** | `New` |
| **Severity** | `Low` |
| **Priority** | `P4 (Low)` |
| **Environment** | OS: Windows 10, Browser: Chrome 147.0.7727.102, Device: Desktop |
| **Build/Version** | actual |
| **Author** | Aleksei Nikolaev|
| **Date Reported** | 2026-04-29 |
| **Linked TC** | **AS-TC-UI_LANGUAGE-002** 

---

## 📝 Description
The interface language resets after logout/login cycle the profile and is set to the one used by the browser by default.

## 🔄 Steps to Reproduce

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

## Actual vs Expected
**Expected:** Language preference saved in user session/database 

**Actual:** Language resets to browser default on login

## Impact Assessment
- [ ] Critical: System unusable  
- [ ] High: Core functionality broken
- [ ] Medium: User settings lost, workaround exists
- [x] Low: Cosmetic issue
- [x] Frequency: 100% reproducible
- [x] Workaround: Reselect language after each login

## Incident Category
- [ ] Functional defect
- [x] UI/UX issue
- [ ] Performance degradation
- [ ] Configuration problem
- [ ] Compatibility issue
- [ ] Documentation error

## Attachments
