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
1. The user is logged into the application.
2. The browser (Chrome) is set to "Dark" mode at the OS level.
3. The application’s theme setting is currently set to "Auto".

## Test Data
* None (Default system settings)

## Steps
| # | Action | Expected Result |
|---| :--- | :--- |
| 1 | Navigate to the application homepage. | Homepage is open |
| 2 | Click on the Profile Icon in the header | A new object with a dropwown listinside has opened |
| 3 | Select 'Light' from the Theme dropdown menu | The theme change to light  |
| 4 | Refresh the browser page (F5) | The theme should remain the same |
| 5 | Click on the Profile Icon again to verify the current | The theme toggle should stay on 'Light'

## Actual Result

As expected

## Status
- [x] Pass
- [ ] Fail (Link to Bug Report: [Issue #XXX])

## Environment / Notes
* **Environment**: Chrome 147.0.7727.102, Windows 10
* **Notes**: None
