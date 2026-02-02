# Acceptance Test Suite: UC-16 View Review Form

## Purpose
Validate acceptance criteria for UC-16: View Review Form.

---

## Acceptance Tests

### UC16-AT-01 — Main success path
**Goal:** Verify UC-16 completes successfully.

- **Given** the preconditions for UC-16 are satisfied
- **When** the primary actor performs the main success scenario
- **Then** the system completes UC-16 successfully
- **And** the success end condition is met

---

### UC16-AT-02 — Alternative path 3a
**Goal:** Verify the system handles extension 3a correctly.

- **Given** the preconditions for UC-16 are satisfied
- **When** the actor performs UC-16 and condition 3a occurs
- **Then** the system does not complete the main success scenario
- **And** displays an error/status message
- **And** the workflow does not proceed incorrectly


---

## Exit Criteria (for UC-16)
UC-16 is considered **accepted** when all tests above pass and failures do not allow the workflow to proceed incorrectly.
