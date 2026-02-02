# Acceptance Test Suite: UC-04 User Login

## Purpose
Validate acceptance criteria for UC-04: User Login.

---

## Acceptance Tests

### UC04-AT-01 — Main success path
**Goal:** Verify UC-04 completes successfully.

- **Given** the preconditions for UC-04 are satisfied
- **When** the primary actor performs the main success scenario
- **Then** the system completes UC-04 successfully
- **And** the success end condition is met

---

### UC04-AT-02 — Alternative path 4a
**Goal:** Verify the system handles extension 4a correctly.

- **Given** the preconditions for UC-04 are satisfied
- **When** the actor performs UC-04 and condition 4a occurs
- **Then** the system does not complete the main success scenario
- **And** displays an error/status message
- **And** the workflow does not proceed incorrectly


---

## Exit Criteria (for UC-04)
UC-04 is considered **accepted** when all tests above pass and failures do not allow the workflow to proceed incorrectly.
