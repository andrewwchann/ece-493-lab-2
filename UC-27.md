# Use Case UC-27: View Attendance Price List

## Goal in Context
View attendance price list on CMS webpage.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Attendee / Guest

## Secondary Actors
CMS Database

## Trigger
User opens the pricing page.

## Success End Condition
Price list is displayed for all attendee roles.

## Failed End Condition
Price list cannot be displayed and user is informed.

## Preconditions
- CMS website is accessible.

## Main Success Scenario
1. User navigates to the conference pricing page.
2. System retrieves the current price list.
3. System displays prices for attendee categories.

## Extensions
- **2a** Pricing data unavailable
  - **2a1** System displays an error message and suggests trying later.

## Related Information
- **Priority**: High
- **Frequency**: Medium
