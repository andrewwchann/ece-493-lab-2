# Use Case UC-20: Receive Paper Decision Notification

## Goal in Context
Author receives editor decision.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Author

## Secondary Actors
CMS Database

## Trigger
Editor records a final decision for the author’s paper.

## Success End Condition
Author receives decision details via CMS notification.

## Failed End Condition
Author is not notified and system logs the failure.

## Preconditions
- Author has a submitted paper under review.

## Main Success Scenario
1. System finalizes the editor’s decision for the paper.
2. System sends a notification to the author.
3. Author views the decision in their CMS account.

## Extensions
- **2a** Notification delivery fails
  - **2a1** System retries and displays decision in account when available.

## Related Information
- **Priority**: High
- **Frequency**: Medium
