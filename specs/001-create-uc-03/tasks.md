---

description: "Task list for Display Registration Error Message"
---

# Tasks: Display Registration Error Message

**Input**: Design documents from `/home/ajchan/ECE493/lab/lab2/ece-493-lab-2/specs/001-create-uc-03/`
**Prerequisites**: plan.md (required), spec.md (required for user stories), research.md, data-model.md, contracts/

**Tests**: Not included (no explicit test tasks requested in the feature specification).

**Organization**: Tasks are grouped by user story to enable independent implementation and testing of each story.

## Format: `[ID] [P?] [Story] Description`

- **[P]**: Can run in parallel (different files, no dependencies)
- **[Story]**: Which user story this task belongs to (e.g., US1, US2)
- All tasks include exact file paths in descriptions

## Constitution Check

- [x] Development proceeds incrementally using Spec-Kit.
- [x] Feature corresponds to a single use case, developed in its own Git branch.
- [x] Use case source files are named `UC-XX.md`.
- [x] Acceptance tests are named `UC-XX-AT.md`.
- [x] Architecture adheres to strict Model-View-Controller (MVC).
- [x] Stack is vanilla HTML/CSS/JavaScript only.
- [x] No frameworks, external libraries, or unstated technologies are introduced.
- [x] Do not initialize or modify the git repository in this stage.
- [x] Do not generate implementation code in this stage.

## Phase 1: Setup (Shared Infrastructure)

**Purpose**: Project initialization and basic structure

- [ ] T001 Create MVC directories `src/models/`, `src/views/`, `src/controllers/` and test directories `tests/contract/`, `tests/integration/`, `tests/unit/`

---

## Phase 2: Foundational (Blocking Prerequisites)

**Purpose**: Core foundations used by all user stories

- [ ] T002 [P] Define the `ValidationError` model in `src/models/validationError.js`
- [ ] T003 [P] Define the `RegistrationSubmission` model in `src/models/registrationSubmission.js`
- [ ] T004 [P] Define the `RegistrationFormField` model in `src/models/registrationFormField.js`
- [ ] T005 Implement validation utility that returns `{field, message}` errors in `src/models/registrationValidation.js`
- [ ] T006 Wire POST /registrations to registration controller with 200/400/503 handling in `src/controllers/registrationController.js`

**Checkpoint**: Validation models and utilities are ready for controller/view integration

---

## Phase 3: User Story 1 - See validation errors on registration (Priority: P1) 🎯 MVP

**Goal**: Show clear, field-level error messages for invalid registration submissions while keeping users on the registration page.

**Independent Test**: Submit invalid registration data and verify field-specific errors display and registration does not complete.

### Implementation for User Story 1

- [ ] T007 [US1] Validate submissions and produce field error lists in `src/controllers/registrationController.js`
- [ ] T008 [P] [US1] Add field-level error placeholders in `src/views/registrationForm.html`
- [ ] T009 [P] [US1] Render field-level errors and keep users on the page in `src/views/registrationForm.js`

**Checkpoint**: User Story 1 is independently functional and demonstrates clear field error messaging.

---

## Phase 4: User Story 2 - Handle validation system errors (Priority: P2)

**Goal**: Inform users when validation cannot be performed and provide a generic, plain-language error message.

**Independent Test**: Simulate a validation system failure and verify a generic error message is displayed without completing registration.

### Implementation for User Story 2

- [ ] T010 [US2] Catch validation system failures and return a generic error message in `src/controllers/registrationController.js`
- [ ] T011 [P] [US2] Add a generic error message container in `src/views/registrationForm.html`
- [ ] T012 [P] [US2] Render the generic error message in `src/views/registrationForm.js`

**Checkpoint**: User Story 2 is independently functional and handles system validation failures.

---

## Phase 5: Polish & Cross-Cutting Concerns

**Purpose**: Documentation and final validation

- [ ] T013 [P] Record quickstart validation notes in `specs/001-create-uc-03/quickstart.md`
- [ ] T014 [P] Verify SC-001–SC-004 outcomes and record results in `specs/001-create-uc-03/quickstart.md`
- [ ] T015 Review and refine error message copy in `src/views/registrationForm.html`

---

## Dependencies & Execution Order

### Phase Dependencies

- **Setup (Phase 1)**: No dependencies - can start immediately
- **Foundational (Phase 2)**: Depends on Setup completion - BLOCKS all user stories
- **User Story 1 (Phase 3)**: Depends on Foundational completion
- **User Story 2 (Phase 4)**: Depends on Foundational completion; runs after US1 due to shared files
- **Polish (Phase 5)**: Depends on all desired user stories being complete

### User Story Dependencies

- **User Story 1 (P1)**: Starts after Foundational - no dependencies on other stories
- **User Story 2 (P2)**: Starts after Foundational; recommended after US1 because it extends the same controller and view

### Parallel Opportunities

- Phase 2 tasks T002–T004 can run in parallel
- US1 view tasks T008–T009 can run in parallel after T006
- US2 view tasks T011–T012 can run in parallel after T010

---

## Parallel Example: User Story 1

```bash
Task: "Add field-level error placeholders in src/views/registrationForm.html"
Task: "Render field-level errors and keep users on the page in src/views/registrationForm.js"
```

## Parallel Example: User Story 2

```bash
Task: "Add a generic error message container in src/views/registrationForm.html"
Task: "Render the generic error message in src/views/registrationForm.js"
```

---

## Implementation Strategy

### MVP First (User Story 1 Only)

1. Complete Phase 1: Setup
2. Complete Phase 2: Foundational
3. Complete Phase 3: User Story 1
4. Validate User Story 1 independently using the quickstart steps

### Incremental Delivery

1. Setup + Foundational
2. User Story 1 → Validate
3. User Story 2 → Validate
4. Polish & documentation updates

---

## Notes

- [P] tasks = different files, no dependencies
- [Story] label maps tasks to specific user stories
- Tasks are specific and immediately executable without additional context
