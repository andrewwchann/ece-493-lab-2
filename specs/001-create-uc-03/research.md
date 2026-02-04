# Research: Display Registration Error Message

**Date**: February 4, 2026
**Feature**: Display Registration Error Message (UC-03)

## Decisions

Decision: Present validation errors adjacent to each invalid field in plain language, and show a generic message when validation cannot be performed.
Rationale: Field-level messages help users correct errors quickly, while a generic message prevents confusion during system failures.
Alternatives considered: Only a top-of-page banner; only field-level messages without a system error fallback.

Decision: Represent validation errors as a list of items containing the field identifier and a user-facing message.
Rationale: A structured list keeps the controller-to-view handoff simple and supports multiple errors per submission.
Alternatives considered: A single concatenated error string; a binary valid/invalid flag without details.

Decision: Use a single registration submission endpoint that returns explicit validation errors for invalid input.
Rationale: This matches the user action (submit form) and keeps the validation workflow in one place.
Alternatives considered: A separate validation-only endpoint; client-only validation without server feedback.
