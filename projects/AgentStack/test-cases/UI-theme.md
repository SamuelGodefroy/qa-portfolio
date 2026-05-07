# Test Case ID: AS-TC-UI_THEME-001

## Metadata
* **Title**: Verify Light Theme Persistence After Refresh
* **Module**: UI Theme
* **Priority**: Low
* **Created By**: Aleksei Nikolaev
* **Date**: 2026-04-28

## Objective
Verify Light theme persists after page refresh when OS is in Dark mode.

## Preconditions
1. User logged into website
2. Browser (Chrome) set to Dark mode (OS level)  
3. Website theme set to "Auto"

## Test Data
* None

## Steps
| # | Action | Expected Result | Actual Result |
|---|--------|-----------------|---------------|
| 1 | Navigate to homepage | Homepage loads | - |
| 2 | Click Profile Icon → Theme | Dropdown opens | - |
| 3 | Select "Light" theme | UI switches to Light | - |
| 4 | Refresh page (F5) | **Light theme persists** | - |
| 5 | Verify theme toggle | Toggle shows "Light" | - |

## Status
- [x] Pass
- [ ] Fail (Link to Bug Report: [#])
- [ ] Blocked
- [ ] Skipped

## Environment
* Chrome 147.0.7727.102, Windows 10

---
---

# Test Case ID: AS-TC-UI-THEME-002

## Metadata
* **Title**: Verify Dark Theme Persistence After Refresh
* **Module**: UI Theme
* **Priority**: Low
* **Created By**: Aleksei Nikolaev
* **Date**: 2026-04-28

## Objective
Verify Dark theme persists after page refresh when OS is in Dark mode.

## Preconditions
1. User logged into website
2. Browser (Chrome) set to Dark mode (OS level)
3. Website theme set to "Auto"

## Test Data
* None

## Steps
| # | Action | Expected Result | Actual Result |
|---|--------|-----------------|---------------|
| 1 | Navigate to homepage | Homepage loads | - |
| 2 | Click Profile Icon → Theme | Dropdown opens | - |
| 3 | Select "Dark" theme | UI switches to Dark | - |
| 4 | Refresh page (F5) | **Dark theme persists** | - |
| 5 | Verify theme toggle | Toggle shows "Dark" | - |

## Status
- [x] Pass
- [ ] Fail (Link to Bug Report: [#])
- [ ] Blocked
- [ ] Skipped

## Environment
* Chrome 147.0.7727.102, Windows 10

---
---

# Test Case ID: AS-TC-UI_THEME-003

## Metadata
* **Title**: Verify Dark Theme Persistence After Logout/Login
* **Module**: UI Theme
* **Priority**: Low
* **Created By**: Aleksei Nikolaev
* **Date**: 2026-04-28

## Objective
Verify Dark theme persists after logout/login cycle.

## Preconditions
1. Valid test account exists
2. Browser set to Dark mode (OS level)
3. Website theme initially "Auto"

## Test Data
* Email: `test@example.com`
* Password: `TestPass123!`

## Steps
| # | Action | Expected Result | Actual Result |
|---|--------|-----------------|---------------|
| 1 | Login with test data | Homepage loads | - |
| 2 | Click Profile → Theme | Dropdown opens | - |
| 3 | Select "Dark" theme | UI switches to Dark | - |
| 4 | Refresh page (F5) | Dark theme persists | - |
| 5 | Click "Logout" | Login screen appears | - |
| 6 | Enter email | Email field populated | - |
| 7 | Enter password | Password field populated | - |
| 8 | Click "Login" | User logged in | - |
| 9 | Verify theme website | The website theme should be set to Dark | -
| 10 | Check theme toggle | **Toggle shows "Dark"** | **FAILED: Toggle reset to "Auto"** |

## Status
- [ ] Pass
- [x] Fail (Link to Bug Report: https://github.com/SamuelGodefroy/qa-portfolio/blob/main/projects/AgentStack/bug-reports/AS-BUG-UI_THEME-003.md)
- [ ] Blocked
- [ ] Skipped

## Environment
* Chrome 147.0.7727.102, Windows 10
---
---

# Test Case ID: AS-UI_THEME-004

## Metadata
* **Title**: Verify Light Theme Persistence After Logout/Login
* **Module**: UI Theme
* **Priority**: Low
* **Created By**: Aleksei Nikolaev
* **Date**: 2026-04-28

## Objective
Verify Light theme persists after logout/login cycle.

## Preconditions
1. Valid test account exists
2. Browser set to Light mode (OS level)
3. Website theme initially "Auto"

## Test Data
* Email: `test@example.com`
* Password: `TestPass123!`

## Steps
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

## Status
- [ ] Pass
- [x] Fail (Link to Bug Report: (https://github.com/SamuelGodefroy/qa-portfolio/blob/main/projects/AgentStack/bug-reports/AS-BUG-UI_THEME-004.md))
- [ ] Blocked
- [ ] Skipped


## Environment
* Chrome 147.0.7727.102, Windows 10
