# Acceptance Test Suite: UC-09 Validate Submission Fields and Show Status Messages

## Purpose
Validate acceptance criteria for UC-09: Validate Submission Fields and Show Status Messages.

---

## Acceptance Tests

### UC09-AT-01 — Main success path
**Goal:** Verify UC-09 completes successfully.

- **Given** the preconditions for UC-09 are satisfied
- **When** the primary actor performs the main success scenario
- **Then** the system completes UC-09 successfully
- **And** the success end condition is met

---

### UC09-AT-02 — Alternative path 2a
**Goal:** Verify the system handles extension 2a correctly.

- **Given** the preconditions for UC-09 are satisfied
- **When** the actor performs UC-09 and condition 2a occurs
- **Then** the system does not complete the main success scenario
- **And** displays an error/status message
- **And** the workflow does not proceed incorrectly


---

## Exit Criteria (for UC-09)
UC-09 is considered **accepted** when all tests above pass and failures do not allow the workflow to proceed incorrectly.
