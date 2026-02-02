# Acceptance Test Suite: UC-14 Ensure Three Reviewers Assigned per Paper

## Purpose
Validate acceptance criteria for UC-14: Ensure Three Reviewers Assigned per Paper.

---

## Acceptance Tests

### UC14-AT-01 — Main success path
**Goal:** Verify UC-14 completes successfully.

- **Given** the preconditions for UC-14 are satisfied
- **When** the primary actor performs the main success scenario
- **Then** the system completes UC-14 successfully
- **And** the success end condition is met

---

### UC14-AT-02 — Alternative path 3a
**Goal:** Verify the system handles extension 3a correctly.

- **Given** the preconditions for UC-14 are satisfied
- **When** the actor performs UC-14 and condition 3a occurs
- **Then** the system does not complete the main success scenario
- **And** displays an error/status message
- **And** the workflow does not proceed incorrectly

---

### UC14-AT-03 — Alternative path 3b
**Goal:** Verify the system handles extension 3b correctly.

- **Given** the preconditions for UC-14 are satisfied
- **When** the actor performs UC-14 and condition 3b occurs
- **Then** the system does not complete the main success scenario
- **And** displays an error/status message
- **And** the workflow does not proceed incorrectly


---

## Exit Criteria (for UC-14)
UC-14 is considered **accepted** when all tests above pass and failures do not allow the workflow to proceed incorrectly.
