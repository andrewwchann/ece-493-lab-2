# Acceptance Test Suite: UC-17 Submit Review Form

## Purpose
Validate acceptance criteria for UC-17: Submit Review Form.

---

## Acceptance Tests

### UC17-AT-01 — Main success path
**Goal:** Verify UC-17 completes successfully.

- **Given** the preconditions for UC-17 are satisfied
- **When** the primary actor performs the main success scenario
- **Then** the system completes UC-17 successfully
- **And** the success end condition is met

---

### UC17-AT-02 — Alternative path 3a
**Goal:** Verify the system handles extension 3a correctly.

- **Given** the preconditions for UC-17 are satisfied
- **When** the actor performs UC-17 and condition 3a occurs
- **Then** the system does not complete the main success scenario
- **And** displays an error/status message
- **And** the workflow does not proceed incorrectly


---

## Exit Criteria (for UC-17)
UC-17 is considered **accepted** when all tests above pass and failures do not allow the workflow to proceed incorrectly.
