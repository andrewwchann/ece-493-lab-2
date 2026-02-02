# Acceptance Test Suite: UC-13 Respond to Review Invitation

## Purpose
Validate acceptance criteria for UC-13: Respond to Review Invitation.

---

## Acceptance Tests

### UC13-AT-01 — Main success path
**Goal:** Verify UC-13 completes successfully.

- **Given** the preconditions for UC-13 are satisfied
- **When** the primary actor performs the main success scenario
- **Then** the system completes UC-13 successfully
- **And** the success end condition is met

---

### UC13-AT-02 — Alternative path 3a
**Goal:** Verify the system handles extension 3a correctly.

- **Given** the preconditions for UC-13 are satisfied
- **When** the actor performs UC-13 and condition 3a occurs
- **Then** the system does not complete the main success scenario
- **And** displays an error/status message
- **And** the workflow does not proceed incorrectly


---

## Exit Criteria (for UC-13)
UC-13 is considered **accepted** when all tests above pass and failures do not allow the workflow to proceed incorrectly.
