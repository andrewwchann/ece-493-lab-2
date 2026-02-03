# Data Model: Create Item

**Date**: February 3, 2026  
**Feature**: Create Item  
**Spec**: `specs/001-create-feature/spec.md`

## Entities

### User

- **Purpose**: Represents a signed-in person who can create items.
- **Key Attributes**:
  - `userId` (unique identifier)
  - `displayName`

### Item

- **Purpose**: Represents a user-owned item created through the feature.
- **Key Attributes**:
  - `itemId` (unique identifier)
  - `title` (required, 1-120 characters after trimming)
  - `description` (optional)
  - `createdAt` (timestamp)
  - `createdBy` (User `userId`)

## Relationships

- **User 1 ── * Item**: A user can create multiple items; each item belongs to exactly one user.

## Constraints

- Title is required and must not exceed 120 characters.
- Description is optional and can be empty.
- Items must be scoped to the creating user by default.

## Lifecycle Notes

- Only creation is in scope for this feature.
- Editing, deletion, and sharing are out of scope.
