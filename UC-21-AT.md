# Acceptance Test Suite: UC-21 Generate Conference Schedule

## Purpose
Validate acceptance criteria for UC-21: Generate Conference Schedule.

---

## Acceptance Tests

### UC21-AT-01 — Main success path
**Goal:** Verify UC-21 completes successfully.

- **Given** the preconditions for UC-21 are satisfied
- **When** the primary actor performs the main success scenario
- **Then** the system completes UC-21 successfully
- **And** the success end condition is met

---

### UC21-AT-02 — Alternative path 2a
**Goal:** Verify the system handles extension 2a correctly.

- **Given** the preconditions for UC-21 are satisfied
- **When** the actor performs UC-21 and condition 2a occurs
- **Then** the system does not complete the main success scenario
- **And** displays an error/status message
- **And** the workflow does not proceed incorrectly


---

## Exit Criteria (for UC-21)
UC-21 is considered **accepted** when all tests above pass and failures do not allow the workflow to proceed incorrectly.
