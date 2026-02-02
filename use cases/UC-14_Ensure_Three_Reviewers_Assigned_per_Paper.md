# Use Case UC-14: Ensure Three Reviewers Assigned per Paper

## Goal in Context
Ensure each paper has exactly 3 reviewers assigned.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Editor

## Secondary Actors
CMS Database

## Trigger
Editor finalizes reviewer assignments for a paper.

## Success End Condition
System confirms exactly three reviewers are assigned.

## Failed End Condition
System blocks finalization and informs editor.

## Preconditions
- Editor is assigning reviewers for a submitted paper.

## Main Success Scenario
1. Editor selects reviewers for the paper.
2. System counts the number of assigned reviewers.
3. System confirms there are exactly three reviewers.
4. System finalizes assignments and enables reviewing.

## Extensions
- **3a** Fewer than three reviewers assigned
  - **3a1** System blocks finalization and prompts editor to add reviewers.
- **3b** More than three reviewers assigned
  - **3b1** System blocks finalization and prompts editor to remove reviewers.

## Related Information
- **Priority**: High
- **Frequency**: Medium
