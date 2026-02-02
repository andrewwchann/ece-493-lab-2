# Use Case UC-23: View Final Schedule for Accepted Paper

## Goal in Context
Author receives final schedule for accepted paper.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Author

## Secondary Actors
CMS Database

## Trigger
Schedule is published for an accepted paper.

## Success End Condition
Author can see when/where their paper is scheduled.

## Failed End Condition
Author cannot access schedule and is informed.

## Preconditions
- Author has an accepted paper.
- Schedule is published.

## Main Success Scenario
1. Author logs into CMS.
2. Author navigates to My Papers.
3. Author selects the accepted paper.
4. System displays the scheduled time and room details.

## Extensions
- **4a** Schedule not yet published
  - **4a1** System displays a message indicating schedule is pending.

## Related Information
- **Priority**: High
- **Frequency**: Medium
