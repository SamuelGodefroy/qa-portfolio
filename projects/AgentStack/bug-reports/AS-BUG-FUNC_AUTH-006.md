# AS-BUG-FUNC_AUTH-006

>**Summary:** Entering a password of length one character
>
>**Example:** *When trying to register an account with a password of one character, no error occurs.*

| **Field** | **Value** |
| :--- | :--- |
| **Status** | New |
| **Severity** | Major |
| **Priority** | P2 (Medium) |
| **Environment** | OS: Windows 10, Browser: Chrome 147.0.7727.102, Device: Desktop |
| **Build/Version** | Actual |
| **Author** | Aleksei Nikolaev |
| **Date Reported** | 2026-05-07 |
| **Linked TC** | [https://github.com/SamuelGodefroy/qa-portfolio/blob/main/projects/AgentStack/test-cases/func_test-cases/AS-TC-FUNC_AUTH-006.md](https://github.com/SamuelGodefroy/qa-portfolio/blob/main/projects/AgentStack/test-cases/func_test-cases/AS-TC-FUNC_AUTH-006.md) |

---

## Description
When registering a new user, the password should contain more than eight characters. Registration is allowed with a password of one character, which makes the account vulnerable to brute‑force attacks.

## Steps to Reproduce

| # | Action | Expected Result | Actual Result |
|---| :--- | :--- | :--- |
| 1 | Click on the "Sign in" icon/button | The user authentication window opens with "Email", "Password" fields and "Sign in", "Registration", "Sign in via API key" icons/buttons | - |
| 2 | Click on the "Registration" icon/button | The registration window opens with "Email", "Password", "Inviter code" (for the referral system) fields | - |
| 3 | Enter valid data into the "Email" field | The entered data is displayed in the text field | - |
| 4 | Enter one character "1" into the "Password" field | The "Password" field displays "dots" hiding the entered password | - |
| 5 | Click on the "Registration" icon/button | Registration error. Password cannot contain only one character | User successfully registered. Dashboard opens |


## Actual vs Expected
**Expected:** User should not be registered with a password of one character.  
**Actual:** User can register with a password of one character.

## Impact Assessment
- [ ] Critical: System unusable (the entire project is down)  
- [ ] High: Core functionality broken (main feature is not working)  
- [x] Medium: User experience degraded, workaround exists (functionality works but is inconvenient)  
- [ ] Low: Cosmetic issue (minor UI distortions)  
- [x] Frequency: [100% / Often / Rarely / Once]  
- [x] Workaround: Use a strong password  

## Incident Category
- [x] Functional defect  
- [ ] UI/UX issue  
- [ ] Performance degradation  
- [ ] Configuration problem  
- [ ] Compatibility issue  
- [ ] Documentation error  

## Attachments
