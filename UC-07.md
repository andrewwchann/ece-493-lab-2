# Use Case UC-07: Submit Paper Manuscript

## Goal in Context
Submit paper manuscript.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Author

## Secondary Actors
CMS Database

## Trigger
Author selects the Submit Paper option.

## Success End Condition
Submission is recorded and visible to the author.

## Failed End Condition
Submission is not recorded and an error is shown.

## Preconditions
- Author is logged in.

## Main Success Scenario
1. Author navigates to the paper submission page.
2. Author enters required paper metadata.
3. Author uploads the manuscript file.
4. Author submits the paper.
5. System validates the submission and stores it.
6. System shows a success confirmation to the author.

## Extensions
- **4a** Required fields are missing
  - **4a1** System displays an error and requests completion.
- **4b** File upload fails
  - **4b1** System displays an error and allows retry.

## Related Information
- **Priority**: High
- **Frequency**: Medium
