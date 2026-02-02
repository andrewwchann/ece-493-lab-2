# Use Case UC-10: Save Paper Submission Progress

## Goal in Context
Save submission progress.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Author

## Secondary Actors
CMS Database

## Trigger
Author chooses to save progress during submission.

## Success End Condition
Draft is saved and can be resumed later.

## Failed End Condition
Draft is not saved and user is informed.

## Preconditions
- Author is logged in and editing a submission.

## Main Success Scenario
1. Author enters submission information.
2. Author selects Save Draft.
3. System validates minimally required draft data.
4. System stores the draft submission.
5. System confirms the draft was saved.

## Extensions
- **3a** System cannot save due to database error
  - **3a1** System displays an error and keeps the current form data.

## Related Information
- **Priority**: High
- **Frequency**: Medium
