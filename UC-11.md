# Use Case UC-11: Assign Reviewers to Paper

## Goal in Context
Assign reviewers to papers by email.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Editor

## Secondary Actors
CMS Database

## Trigger
Editor selects a submitted paper and assigns reviewers.

## Success End Condition
Review invitations are sent to selected reviewers.

## Failed End Condition
Reviewers are not assigned and error is shown.

## Preconditions
- Editor is logged in.
- Paper exists in submitted state.

## Main Success Scenario
1. Editor opens the paper details page.
2. Editor enters reviewer email addresses.
3. Editor confirms reviewer assignment.
4. System validates reviewer eligibility.
5. System creates review assignments and sends invitations.

## Extensions
- **4a** Reviewer email not found or invalid
  - **4a1** System displays an error and does not assign that reviewer.

## Related Information
- **Priority**: High
- **Frequency**: Medium
