# Contract: Create Item Form

**Date**: February 3, 2026  
**Feature**: Create Item  
**Spec**: `specs/001-create-feature/spec.md`

## Purpose

Define the user-facing contract for creating a new item, including inputs, validation rules, and expected outcomes.

## Inputs

- **Title** (required)
  - Trim leading/trailing whitespace
  - Length: 1-120 characters
- **Description** (optional)
  - Free text, may be empty

## Preconditions

- User is signed in.
- User has permission to create items.

## Success Outcome

- A new item is created with:
  - Title and optional description
  - Creator set to the signed-in user
  - Creation time captured
- The new item appears in the user's item list or detail view within 5 seconds.
- A confirmation message is shown.

## Validation Errors

- Missing title: show a clear, actionable validation message.
- Title exceeds 120 characters: show a length validation message.

## Cancellation

- If the user cancels before submission, no item is created and partial inputs are discarded.
