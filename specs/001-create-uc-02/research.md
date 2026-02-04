# Research: UC-02 Validate Registration Credentials

**Date**: February 4, 2026  
**Source Spec**: `/home/ajchan/ECE493/lab/lab2/ece-493-lab-2/specs/001-create-uc-02/spec.md`

## Decisions

### Decision 1: Use vanilla HTML/CSS/JavaScript with strict MVC
**Rationale**: The CMS constitution mandates a vanilla web stack and strict MVC separation. This ensures compliance and reduces rework risk.
**Alternatives considered**: Using a web framework or external validation library (rejected by constitution).

### Decision 2: Apply explicit credential rules from the spec
**Rationale**: The feature spec defines password security standards and email normalization behaviors (case-insensitive uniqueness, trim email whitespace). Codifying these rules prevents ambiguous validation outcomes.
**Alternatives considered**: RFC-exhaustive email parsing or passphrase-only password rules (not specified in scope).

### Decision 3: Expose a single validation contract for UI/controller integration
**Rationale**: A dedicated validation endpoint with structured error details keeps UI feedback consistent and isolates validation logic for reuse in the registration flow.
**Alternatives considered**: Inline-only validation with no formal contract, or splitting into multiple endpoints (adds unnecessary complexity for this scope).
