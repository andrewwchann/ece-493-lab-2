# Use Case UC-19: Make Final Paper Decision

## Goal in Context
Editor makes final accept/reject decision after 3 reviews.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Editor

## Secondary Actors
CMS Database

## Trigger
Editor receives three completed reviews for a paper.

## Success End Condition
Paper decision is recorded and author is notified.

## Failed End Condition
Decision is not recorded and editor is informed.

## Preconditions
- Editor is logged in.
- Three reviews are completed for the paper.

## Main Success Scenario
1. Editor opens the paper decision page.
2. Editor reviews the three completed reviews.
3. Editor selects Accept or Reject.
4. Editor confirms the decision.
5. System records the decision and notifies the author.

## Extensions
- **1a** Fewer than three reviews completed
  - **1a1** System blocks decision and informs the editor.

## Related Information
- **Priority**: High
- **Frequency**: Medium
