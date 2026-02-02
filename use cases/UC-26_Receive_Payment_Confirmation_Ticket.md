# Use Case UC-26: Receive Payment Confirmation Ticket

## Goal in Context
Receive payment confirmation as ticket.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Attendee (Authorized User)

## Secondary Actors
Payment Gateway

## Trigger
Successful conference payment is completed.

## Success End Condition
User receives confirmation/ticket.

## Failed End Condition
Ticket is not generated and system informs user.

## Preconditions
- User has successfully paid for registration.

## Main Success Scenario
1. System confirms payment success from the gateway.
2. System generates a registration confirmation ticket.
3. System displays the ticket to the user and stores it in the user account.

## Extensions
- **2a** Ticket generation fails
  - **2a1** System displays an error and allows user to retry viewing later.

## Related Information
- **Priority**: High
- **Frequency**: Medium
