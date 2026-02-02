# Use Case UC-15: Access Paper After Accepting Invitation

## Goal in Context
Accepted invitations place paper in reviewer account.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Reviewer

## Secondary Actors
CMS Database

## Trigger
Reviewer accepts an invitation to review.

## Success End Condition
Paper appears in reviewer account for review.

## Failed End Condition
Paper does not appear and reviewer is informed.

## Preconditions
- Reviewer accepted an invitation.

## Main Success Scenario
1. Reviewer accepts the review invitation.
2. System adds the paper to the reviewer’s assigned papers list.
3. Reviewer opens the assigned paper from their dashboard.

## Extensions
- **2a** Paper assignment creation fails
  - **2a1** System displays an error and does not add the paper.

## Related Information
- **Priority**: High
- **Frequency**: Medium
