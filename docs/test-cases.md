# Manual Test Cases

| ID | Title | Preconditions | Steps | Expected Result |
|---|---|---|---|---|
| TC-01 | Signup - success | App running | Go to /signup_page, enter valid email + matching passwords, submit | Redirects to login page + success message |
| TC-02 | Signup - existing email | Same email already registered | Repeat signup with same email | Signup rejected + error message |
| TC-03 | Signup - password mismatch | App running | Enter password != confirm password | Signup rejected + error message |
| TC-04 | Login - success | User exists | Go to /, enter valid email/password, submit | Redirects to /dashboard |
| TC-05 | Login - invalid password | User exists | Login with wrong password | Redirects back to / with error message |
| TC-06 | Dashboard - blocked without login | Not logged in | Go directly to /dashboard | Redirects to / (login) |
| TC-07 | Dashboard - allowed after login | Logged in | Login then open /dashboard | Page loads successfully (200) |
| TC-08 | Logout | Logged in | Open /logout then try /dashboard | Session cleared + dashboard redirects to login |
