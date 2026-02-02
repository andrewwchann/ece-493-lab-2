# Use Case UC-24: View Published Conference Schedule

## Goal in Context
Publish schedule on webpage for attendees.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Attendee / Guest

## Secondary Actors
CMS Database

## Trigger
Attendee opens the CMS conference schedule page.

## Success End Condition
Schedule is displayed on the CMS website.

## Failed End Condition
Schedule cannot be displayed and user is informed.

## Preconditions
- Schedule has been published.

## Main Success Scenario
1. Attendee navigates to the schedule webpage.
2. System retrieves the published schedule.
3. System displays the schedule in HTML format.

## Extensions
- **2a** Schedule unavailable
  - **2a1** System displays a message indicating schedule is not available.

## Related Information
- **Priority**: High
- **Frequency**: Medium
