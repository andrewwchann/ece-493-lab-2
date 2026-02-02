# Use Case UC-06: Change Password

## Goal in Context
Change password.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Registered User

## Secondary Actors
CMS Database

## Trigger
Registered user requests a password change.

## Success End Condition
Password is updated and user is informed.

## Failed End Condition
Password is not updated and user is informed of failure.

## Preconditions
- User is logged in.

## Main Success Scenario
1. User navigates to account settings.
2. User selects the Change Password option.
3. User enters current password and new password.
4. User submits the password change request.
5. System validates current password and new password rules.
6. System updates the stored password.
7. System confirms the password change.

## Extensions
- **5a** Current password is incorrect
  - **5a1** System displays an error and does not change the password.
- **5b** New password does not meet security requirements
  - **5b1** System displays an error and requests a new password.

## Related Information
- **Priority**: High
- **Frequency**: Medium
