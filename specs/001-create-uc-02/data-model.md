# Data Model: UC-02 Validate Registration Credentials

**Date**: February 4, 2026  
**Source Spec**: `/home/ajchan/ECE493/lab/lab2/ece-493-lab-2/specs/001-create-uc-02/spec.md`

## Entities

### RegistrationCredential (transient input)
Represents the email and password submitted during registration for validation.

- **email**: string
  - Trim leading/trailing whitespace before validation
  - Must include `@` and a domain
  - Accepts dots and plus tags in the local part
  - Compared case-insensitively for uniqueness
- **password**: string
  - Evaluated exactly as entered
  - Minimum 8 characters
  - Must include at least one letter, one number, and one special character

### UserAccount (existing record)
Represents a registered user account used to check email uniqueness.

- **email**: string
  - Unique (case-insensitive)
  - Compared against `RegistrationCredential.email` to detect duplicates

## Relationships

- `RegistrationCredential.email` MUST NOT match any existing `UserAccount.email` when normalized for case.

## State Transitions

- **Submitted** → **Validated (Pass)**: email format valid, email unique, password meets security rules.
- **Submitted** → **Validated (Fail)**: one or more validation rules fail; errors returned for each invalid field.

## Validation Rules Summary

- Email format: contains `@` and a domain; supports dots/plus tags in local part.
- Email uniqueness: case-insensitive match against existing user accounts.
- Password strength: min 8 characters with at least one letter, one number, and one special character.
