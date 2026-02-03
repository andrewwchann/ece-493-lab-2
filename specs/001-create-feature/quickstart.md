# Quickstart: Create Item

**Date**: February 3, 2026  
**Feature**: Create Item  
**Spec**: `specs/001-create-feature/spec.md`

## Prerequisites

- Modern web browser (desktop or mobile)
- A signed-in user context available in the app

## Run

1. Open the application entry point (e.g., `src/index.html`) in a browser.
2. Navigate to the Create Item view.
3. Enter a title (1-120 characters) and, optionally, a description.
4. Submit the form.
5. Confirm the new item appears in the item list or details view with creator and creation time visible.

## Validation Checks

- Submitting without a title shows a clear validation message and does not create an item.
- Submitting a title longer than 120 characters shows a length validation message.
- Cancelling creation returns to the prior view without creating an item.
