# Acceptance Test Suite: UC-15 Access Paper After Accepting Invitation

## Purpose
Validate acceptance criteria for UC-15: Access Paper After Accepting Invitation.

---

## Acceptance Tests

### UC15-AT-01 — Main success path
**Goal:** Verify UC-15 completes successfully.

- **Given** the preconditions for UC-15 are satisfied
- **When** the primary actor performs the main success scenario
- **Then** the system completes UC-15 successfully
- **And** the success end condition is met

---

### UC15-AT-02 — Alternative path 2a
**Goal:** Verify the system handles extension 2a correctly.

- **Given** the preconditions for UC-15 are satisfied
- **When** the actor performs UC-15 and condition 2a occurs
- **Then** the system does not complete the main success scenario
- **And** displays an error/status message
- **And** the workflow does not proceed incorrectly


---

## Exit Criteria (for UC-15)
UC-15 is considered **accepted** when all tests above pass and failures do not allow the workflow to proceed incorrectly.
