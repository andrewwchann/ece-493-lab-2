# Acceptance Test Suite: UC-25 Register for Conference and Pay

## Purpose
Validate acceptance criteria for UC-25: Register for Conference and Pay.

---

## Acceptance Tests

### UC25-AT-01 — Main success path
**Goal:** Verify UC-25 completes successfully.

- **Given** the preconditions for UC-25 are satisfied
- **When** the primary actor performs the main success scenario
- **Then** the system completes UC-25 successfully
- **And** the success end condition is met

---

### UC25-AT-02 — Alternative path 5a
**Goal:** Verify the system handles extension 5a correctly.

- **Given** the preconditions for UC-25 are satisfied
- **When** the actor performs UC-25 and condition 5a occurs
- **Then** the system does not complete the main success scenario
- **And** displays an error/status message
- **And** the workflow does not proceed incorrectly

---

### UC25-AT-03 — Alternative path 3a
**Goal:** Verify the system handles extension 3a correctly.

- **Given** the preconditions for UC-25 are satisfied
- **When** the actor performs UC-25 and condition 3a occurs
- **Then** the system does not complete the main success scenario
- **And** displays an error/status message
- **And** the workflow does not proceed incorrectly


---

## Exit Criteria (for UC-25)
UC-25 is considered **accepted** when all tests above pass and failures do not allow the workflow to proceed incorrectly.
