# Use Case UC-09: Validate Submission Fields and Show Status Messages

## Goal in Context
Validate required fields and show success/error messages for submission.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Author

## Secondary Actors
CMS Database

## Trigger
Author submits the paper submission form.

## Success End Condition
System confirms submission is valid and accepted.

## Failed End Condition
System reports invalid fields and prevents submission.

## Preconditions
- Author is on the submission form.

## Main Success Scenario
1. Author submits the paper submission form.
2. System validates that all required fields are present.
3. System validates the uploaded manuscript meets constraints.
4. System displays a success message and accepts the submission.

## Extensions
- **2a** One or more required fields are missing/invalid
  - **2a1** System displays an error message and highlights invalid fields.

## Related Information
- **Priority**: High
- **Frequency**: Medium
