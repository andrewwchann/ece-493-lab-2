# Use Case UC-12: Enforce Reviewer Assignment Limit

## Goal in Context
Prevent assigning more than 5 papers to a reviewer.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Editor

## Secondary Actors
CMS Database

## Trigger
Editor attempts to assign a reviewer who already has 5 papers.

## Success End Condition
System prevents exceeding the limit and informs the editor.

## Failed End Condition
System assigns too many papers to a reviewer.

## Preconditions
- Editor is assigning reviewers.

## Main Success Scenario
1. Editor selects a reviewer for assignment.
2. System checks the reviewer’s current assignment count.
3. System detects the reviewer already has 5 assigned papers.
4. System blocks the assignment and shows an error message.

## Extensions
- **2a** System cannot retrieve assignment count
  - **2a1** System shows an error and prevents assignment until resolved.

## Related Information
- **Priority**: High
- **Frequency**: Medium
