# Use Case UC-03: Display Registration Error Message

## Goal in Context
See error message when registration info invalid.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
User

## Secondary Actors
CMS Database

## Trigger
User submits registration form with invalid information.

## Success End Condition
System displays a clear error message and allows correction.

## Failed End Condition
System fails to inform the user of invalid input.

## Preconditions
- User has access to CMS web interface.

## Main Success Scenario
1. User submits the registration form.
2. System validates registration fields.
3. System detects one or more invalid fields.
4. System displays an error message explaining the invalid fields.
5. System keeps the user on the registration page for correction.

## Extensions
- **3a** System cannot validate due to server/database error
  - **3a1** System displays a generic error message and asks the user to try again later.

## Related Information
- **Priority**: High
- **Frequency**: Medium
