# Use Case UC-25: Register for Conference and Pay

## Goal in Context
Register for conference and pay by credit card.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Attendee (Authorized User)

## Secondary Actors
Payment Gateway

## Trigger
Authorized user chooses to register and pay.

## Success End Condition
Payment succeeds and registration is confirmed.

## Failed End Condition
Payment fails and registration is not completed.

## Preconditions
- User is logged in.
- Conference registration is open.

## Main Success Scenario
1. User navigates to conference registration.
2. User selects attendee type and confirms price.
3. User enters credit card payment details.
4. User submits payment.
5. System processes payment via payment gateway.
6. System confirms registration and stores payment record.

## Extensions
- **5a** Payment is declined
  - **5a1** System displays an error and does not confirm registration.
- **3a** Payment details are invalid/missing
  - **3a1** System prompts user to correct payment fields.

## Related Information
- **Priority**: High
- **Frequency**: Medium
