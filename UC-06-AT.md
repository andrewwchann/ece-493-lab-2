# Acceptance Test Suite: UC-06 Change Password

## Purpose
Validate acceptance criteria for UC-06: Change Password.

---

## Acceptance Tests

### UC06-AT-01 — Main success path
**Goal:** Verify UC-06 completes successfully.

- **Given** the preconditions for UC-06 are satisfied
- **When** the primary actor performs the main success scenario
- **Then** the system completes UC-06 successfully
- **And** the success end condition is met

---

### UC06-AT-02 — Alternative path 5a
**Goal:** Verify the system handles extension 5a correctly.

- **Given** the preconditions for UC-06 are satisfied
- **When** the actor performs UC-06 and condition 5a occurs
- **Then** the system does not complete the main success scenario
- **And** displays an error/status message
- **And** the workflow does not proceed incorrectly

---

### UC06-AT-03 — Alternative path 5b
**Goal:** Verify the system handles extension 5b correctly.

- **Given** the preconditions for UC-06 are satisfied
- **When** the actor performs UC-06 and condition 5b occurs
- **Then** the system does not complete the main success scenario
- **And** displays an error/status message
- **And** the workflow does not proceed incorrectly


---

## Exit Criteria (for UC-06)
UC-06 is considered **accepted** when all tests above pass and failures do not allow the workflow to proceed incorrectly.
