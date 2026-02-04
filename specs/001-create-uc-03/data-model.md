# Data Model: Display Registration Error Message

**Date**: February 4, 2026
**Feature**: Display Registration Error Message (UC-03)

## Entities

### Registration Submission
Represents a user's attempted registration at the moment of form submission.

Fields:
- Submission ID (unique identifier)
- Submitted field values (keyed by field name)
- Submission timestamp

### Registration Form Field
Represents a single input on the registration form.

Fields:
- Field name
- Field label
- Required flag
- Validation rules (format, allowed characters, min/max length)

### Validation Error
Represents a failed validation for a specific field.

Fields:
- Field name
- Issue type (missing, format, length, invalid characters)
- User-facing message

## Relationships

- A Registration Submission can have zero or more Validation Errors.
- Each Validation Error references one Registration Form Field.

## Validation Rules

- Missing required fields generate a Validation Error for that field.
- Fields that exceed allowed length generate a Validation Error for that field.
- Fields containing invalid characters generate a Validation Error for that field.
- Multiple validation errors may be returned for a single submission.

## State Transitions

- Submitted -> Validated (no errors) -> Registration continues in existing flow.
- Submitted -> Validated (errors found) -> Errors displayed, user remains on registration page.
- Submitted -> Validation Failed (system error) -> Generic error displayed, user remains on registration page.
