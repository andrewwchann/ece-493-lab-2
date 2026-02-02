# Acceptance Test Suite: UC-18 Collect Completed Reviews

## Purpose
Validate acceptance criteria for UC-18: Collect Completed Reviews.

---

## Acceptance Tests

### UC18-AT-01 — Main success path
**Goal:** Verify UC-18 completes successfully.

- **Given** the preconditions for UC-18 are satisfied
- **When** the primary actor performs the main success scenario
- **Then** the system completes UC-18 successfully
- **And** the success end condition is met

---

### UC18-AT-02 — Alternative path 2a
**Goal:** Verify the system handles extension 2a correctly.

- **Given** the preconditions for UC-18 are satisfied
- **When** the actor performs UC-18 and condition 2a occurs
- **Then** the system does not complete the main success scenario
- **And** displays an error/status message
- **And** the workflow does not proceed incorrectly


---

## Exit Criteria (for UC-18)
UC-18 is considered **accepted** when all tests above pass and failures do not allow the workflow to proceed incorrectly.
