# Use Case UC-18: Collect Completed Reviews

## Goal in Context
Editor receives completed review forms.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Editor

## Secondary Actors
CMS Database

## Trigger
Editor checks the review status for a paper.

## Success End Condition
Editor can view all completed reviews for the paper.

## Failed End Condition
Editor cannot access reviews and is informed.

## Preconditions
- Editor is logged in.
- At least one review exists for a paper.

## Main Success Scenario
1. Editor opens the paper review status page.
2. System retrieves completed review forms.
3. System displays the collected reviews to the editor.

## Extensions
- **2a** No reviews are completed yet
  - **2a1** System displays a status message indicating reviews are pending.

## Related Information
- **Priority**: High
- **Frequency**: Medium
