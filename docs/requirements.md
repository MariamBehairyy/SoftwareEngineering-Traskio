# Requirements

## Overview
Authentication system (Signup/Login) with a protected Dashboard using Flask sessions.

## Actors
- Guest (not logged in)
- User (logged in)

## Functional Requirements
- FR-01: The system shall allow a guest to sign up with email and password.
- FR-02: The system shall validate that password and confirm password match during signup.
- FR-03: The system shall prevent duplicate registrations for the same email.
- FR-04: The system shall allow a user to log in with valid credentials.
- FR-05: The system shall reject login with invalid credentials.
- FR-06: The system shall restrict access to /dashboard unless the user is logged in.
- FR-07: The system shall allow a logged-in user to log out and clear the session.

## Non-Functional Requirements
- NFR-01: Passwords shall be stored hashed (not plain text).
- NFR-02: The UI shall be accessible through a browser.
- NFR-03: The system shall show clear success/error messages.
- NFR-04: Automated tests shall run in CI (GitHub Actions).
