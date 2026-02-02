# Acceptance Test Suite: UC-11 Assign Reviewers to Paper

## Purpose
Validate acceptance criteria for UC-11: Assign Reviewers to Paper.

---

## Acceptance Tests

### UC11-AT-01 — Main success path
**Goal:** Verify UC-11 completes successfully.

- **Given** the preconditions for UC-11 are satisfied
- **When** the primary actor performs the main success scenario
- **Then** the system completes UC-11 successfully
- **And** the success end condition is met

---

### UC11-AT-02 — Alternative path 4a
**Goal:** Verify the system handles extension 4a correctly.

- **Given** the preconditions for UC-11 are satisfied
- **When** the actor performs UC-11 and condition 4a occurs
- **Then** the system does not complete the main success scenario
- **And** displays an error/status message
- **And** the workflow does not proceed incorrectly


---

## Exit Criteria (for UC-11)
UC-11 is considered **accepted** when all tests above pass and failures do not allow the workflow to proceed incorrectly.
