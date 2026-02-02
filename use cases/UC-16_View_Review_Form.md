# Use Case UC-16: View Review Form

## Goal in Context
View review form for assigned paper.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Reviewer

## Secondary Actors
CMS Database

## Trigger
Reviewer selects an assigned paper to review.

## Success End Condition
Review form is displayed for the selected paper.

## Failed End Condition
Review form cannot be displayed and error is shown.

## Preconditions
- Reviewer is logged in and has an assigned paper.

## Main Success Scenario
1. Reviewer opens the assigned paper.
2. Reviewer selects View Review Form.
3. System retrieves the review form template.
4. System displays the review form to the reviewer.

## Extensions
- **3a** Review form is unavailable
  - **3a1** System displays an error and suggests trying later.

## Related Information
- **Priority**: High
- **Frequency**: Medium
