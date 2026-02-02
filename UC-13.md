# Use Case UC-13: Respond to Review Invitation

## Goal in Context
Receive invitation to review and accept/reject.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Reviewer

## Secondary Actors
CMS Database

## Trigger
Reviewer receives a review invitation.

## Success End Condition
Reviewer accepts or rejects the invitation and system records response.

## Failed End Condition
Response is not recorded and reviewer is informed.

## Preconditions
- Reviewer has received an invitation and can access CMS.

## Main Success Scenario
1. Reviewer opens the invitation notification.
2. Reviewer views paper details and invitation.
3. Reviewer selects Accept or Reject.
4. System records the reviewer’s response.
5. System notifies the editor of the response.

## Extensions
- **3a** Invitation has expired or is invalid
  - **3a1** System displays an error and prevents response.

## Related Information
- **Priority**: High
- **Frequency**: Medium
