# Test Case ID: AS-THEME-001

## Metadata
* **Title**: Check theme 
* **Module**: UI THEME
* **Priority**: Low
* **Created By**: Aleksei Nikolaev
* **Date**: 2026-04-28

## Objective
Verify that the user can switch the interface theme from "Auto" to "Light" and that the setting persists after a page refresh.

## Preconditions
1. The user is logged into the websit.
2. The browser (Chrome) is set to "Dark" mode at the OS level.
3. The website theme setting is currently set to "Auto".

## Test Data
* None (Default system settings)

## Steps
| # | Action | Expected Result |
|---| :--- | :--- |
| 1 | Navigate to the website homepage. | Homepage is open |
| 2 | Click on the Profile Icon in the header | A new object with a dropwown listinside has opened |
| 3 | Select 'Light' from the Theme dropdown menu | The theme change to light  |
| 4 | Refresh the browser page (F5) | The theme should remain the same |
| 5 | Click on the Profile Icon again to verify the current | The theme toggle should stay on 'Light'

## Actual Result

As expected

## Status
- [x] Pass 
- [ ] Fail 

## Environment / Notes
* **Environment**: Chrome 147.0.7727.102, Windows 10
* **Notes**: None

---
---

# Test Case ID: AS-THEME-002

## Metadata
* **Title**: Check theme "Dark"
* **Module**: UI THEME
* **Priority**: Low
* **Created By**: Aleksei Nikolaev
* **Date**: 2026-04-28

## Objective
Verify that the user can switch the interface theme from "Auto" to "Dark" and that the setting persists after a page refresh.

## Preconditions
1. 1. The user is logged into the website.
2. The browser (Chrome) is set to "Dark" mode at the OS level.
3. The website theme setting is currently set to "Auto".

## Test Data
* None (Default system settings)

## Steps
| # | Action | Expected Result |
|---| :--- | :--- |
| 1 | Navigate to the website homepage. | Homepage is open |
| 2 | Click on the Profile Icon in the header | A new object with a dropwown listinside has opened |
| 3 | Select "Dark" from the Theme dropdown menu | The theme change to Dark  |
| 4 | Refresh the browser page (F5) | The theme should remain the same |
| 5 | Click on the Profile Icon again to verify the current | The theme toggle should stay on "Dark"

## Actual Result

As expected

## Status
- [x] Pass
- [ ] Fail (Link to Bug Report: [Issue #XXX])

## Environment / Notes
* **Environment**: Chrome 147.0.7727.102, Windows 10
* **Notes**: None

---
---

# Test Case ID: AS-THEME-003

## Metadata
* **Title**: Check theme presistence after login
* **Module**: UI THEME
* **Priority**: Low
* **Created By**: Aleksei Nikolaev
* **Date**: 2026-04-28

## Objective
Verify that the darktheme setting remains consistent after logging out and back in

## Preconditions
1. The user is logged into the website.
2. The browser (Chrome) is set to "Dark" mode at the OS level.
3. The website theme setting is currently set to "Auto".

## Test Data
* None (Default system settings)

## Steps
| # | Action | Expected Result |
|---| :--- | :--- |
| 1 | Navigate to the website homepage. | Homepage is open |
| 2 | Click on the Profile Icon in the header | A new object with a dropwown listinside has opened |
| 3 | Select "Dark" from the Theme dropdown menu | The theme change to Dark  |
| 4 | Refresh the browser page (F5) | The theme should remain the same |
| 5 | Click on the loggout button | The user has logged out of the system. The login or registration window appears
| 6 | In the email field, enter a valid email | The email is entered in the field
| 7 | In the password field, enter the correct password | The password is entered in the field
| 8 | Click on the loggin button | The user is logged into the website
| 9 | Follow the instruction in step 2 | The theme remained dark and toggle is set to the dark theme

## Actual Result

In step 9 the theme remains selected as auto

## Status
- [ ] Pass
- [x] Fail (Link to Bug Report: [Issue #XXX])

## Environment / Notes
* **Environment**: Chrome 147.0.7727.102, Windows 10
* **Notes**: None

---
---

# Test Case ID: AS-THEME-004

## Metadata
* **Title**: Check theme presistence after login
* **Module**: UI THEME
* **Priority**: Low
* **Created By**: Aleksei Nikolaev
* **Date**: 2026-04-28

## Objective
Verify that the light theme setting remains consistent after logging out and back in

## Preconditions
1. The user is logged into the website.
2. The browser (Chrome) is set to Light mode at the OS level.
3. The website theme setting is currently set to "Auto".

## Test Data
* None (Default system settings)

## Steps
| # | Action | Expected Result |
|---| :--- | :--- |
| 1 | Navigate to the website homepage. | Homepage is open |
| 2 | Click on the Profile Icon in the header | A new object with a dropwown listinside has opened |
| 3 | Select "Light" from the Theme dropdown menu | The theme change to Light  |
| 4 | Refresh the browser page (F5) | The theme should remain the same |
| 5 | Click on the loggout button | The user has logged out of the system. The login or registration window appears
| 6 | In the email field, enter a valid email | The email is entered in the field
| 7 | In the password field, enter the correct password | The password is entered in the field
| 8 | Click on the loggin button | The user is logged into the website
| 9 | Follow the instruction in step 2 | The theme remained light and toggle is set to the dark theme

## Actual Result

In step 9 the theme remains selected as auto

## Status
- [ ] Pass
- [x] Fail (Link to Bug Report: [Issue #XXX])

## Environment / Notes
* **Environment**: Chrome 147.0.7727.102, Windows 10
* **Notes**: None
