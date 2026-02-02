# Use Case UC-21: Generate Conference Schedule

## Goal in Context
Generate conference schedule in HTML (time+rooms).

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Administrator

## Secondary Actors
CMS Database

## Trigger
Administrator requests schedule generation.

## Success End Condition
Schedule is generated in HTML and stored/published.

## Failed End Condition
Schedule generation fails and admin is informed.

## Preconditions
- Administrator is logged in.
- There are accepted papers.

## Main Success Scenario
1. Administrator selects Generate Schedule.
2. System gathers accepted papers and available rooms/time slots.
3. System generates an HTML schedule.
4. System saves the schedule and confirms success.

## Extensions
- **2a** No accepted papers available
  - **2a1** System displays a message and does not generate a schedule.

## Related Information
- **Priority**: High
- **Frequency**: Medium
