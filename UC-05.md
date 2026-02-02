# Use Case UC-05: Display Login Error Message

## Goal in Context
See error when login credentials incorrect.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Registered User

## Secondary Actors
CMS Database

## Trigger
User submits login form with incorrect credentials.

## Success End Condition
System displays an error message and login is denied.

## Failed End Condition
System allows access or fails to respond appropriately.

## Preconditions
- User is on the Login page.

## Main Success Scenario
1. User enters username/email and password.
2. User submits the login form.
3. System checks credentials against stored user records.
4. System rejects invalid credentials.
5. System displays an error message indicating login failed.

## Extensions
- None

## Related Information
- **Priority**: High
- **Frequency**: Medium
