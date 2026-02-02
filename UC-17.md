# Use Case UC-17: Submit Review Form

## Goal in Context
Submit completed review form.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Reviewer

## Secondary Actors
CMS Database

## Trigger
Reviewer submits a completed review form.

## Success End Condition
Review is stored and made available to the editor.

## Failed End Condition
Review is not stored and reviewer is informed.

## Preconditions
- Reviewer is viewing a review form.

## Main Success Scenario
1. Reviewer completes the review form fields.
2. Reviewer submits the review form.
3. System validates required review fields.
4. System stores the completed review.
5. System confirms successful submission.

## Extensions
- **3a** Required review fields are missing
  - **3a1** System displays an error and requests completion.

## Related Information
- **Priority**: High
- **Frequency**: Medium
