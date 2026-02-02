# Use Case UC-22: Edit Conference Schedule

## Goal in Context
Edit/update generated schedule.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Editor

## Secondary Actors
CMS Database

## Trigger
Editor opens the schedule editor.

## Success End Condition
Schedule updates are saved and reflected in the published schedule.

## Failed End Condition
Schedule updates are not saved and error is shown.

## Preconditions
- Editor is logged in.
- A schedule exists.

## Main Success Scenario
1. Editor opens the schedule management page.
2. Editor selects a session/time slot to edit.
3. Editor updates time/room assignments.
4. Editor saves the schedule changes.
5. System validates and stores the updated schedule.

## Extensions
- **4a** Update conflicts with existing schedule constraints
  - **4a1** System displays an error and prevents saving.

## Related Information
- **Priority**: High
- **Frequency**: Medium
