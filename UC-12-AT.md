# Acceptance Test Suite: UC-12 Enforce Reviewer Assignment Limit

## Purpose
Validate acceptance criteria for UC-12: Enforce Reviewer Assignment Limit.

---

## Acceptance Tests

### UC12-AT-01 — Main success path
**Goal:** Verify UC-12 completes successfully.

- **Given** the preconditions for UC-12 are satisfied
- **When** the primary actor performs the main success scenario
- **Then** the system completes UC-12 successfully
- **And** the success end condition is met

---

### UC12-AT-02 — Alternative path 2a
**Goal:** Verify the system handles extension 2a correctly.

- **Given** the preconditions for UC-12 are satisfied
- **When** the actor performs UC-12 and condition 2a occurs
- **Then** the system does not complete the main success scenario
- **And** displays an error/status message
- **And** the workflow does not proceed incorrectly


---

## Exit Criteria (for UC-12)
UC-12 is considered **accepted** when all tests above pass and failures do not allow the workflow to proceed incorrectly.
