# Use Case UC-04: User Login

## Goal in Context
Log into CMS.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Registered User

## Secondary Actors
CMS Database

## Trigger
User selects the Login option and submits credentials.

## Success End Condition
User is authenticated and shown their dashboard.

## Failed End Condition
User is not authenticated and receives an error.

## Preconditions
- User has an existing CMS account.
- User is not currently logged in.

## Main Success Scenario
1. User navigates to the Login page.
2. User enters username/email and password.
3. User submits the login form.
4. System validates the credentials.
5. System creates an authenticated session.
6. System redirects the user to their dashboard.

## Extensions
- **4a** Credentials are incorrect
  - **4a1** System displays an error message and allows retry.

## Related Information
- **Priority**: High
- **Frequency**: Medium
