---

description: "Task list for Create Item implementation"
---

# Tasks: Create Item

**Input**: Design documents from `/specs/001-create-feature/`
**Prerequisites**: plan.md (required), spec.md (required for user stories), research.md, data-model.md, contracts/

**Tests**: Tests are OPTIONAL and only included when explicitly requested. No explicit test tasks are required for this feature.

**Organization**: Tasks are grouped by user story to enable independent implementation and testing of each story.

## Format: `[ID] [P?] [Story] Description`

- **[P]**: Can run in parallel (different files, no dependencies)
- **[Story]**: Which user story this task belongs to (e.g., US1)
- Include exact file paths in descriptions

## Path Conventions

- **Single project**: `src/`, `tests/` at repository root (MVC under `src/`)
- Paths below follow the single project structure from `plan.md`

## Phase 1: Setup (Shared Infrastructure)

**Purpose**: Project initialization and basic structure

- [ ] T001 Create MVC and test directories: `src/models/`, `src/views/`, `src/controllers/`, `tests/contract/`, `tests/integration/`, `tests/unit/`
- [ ] T002 Create base entry file `src/index.html` with shell layout and script includes for MVC files
- [ ] T003 [P] Create view scaffolds in `src/views/create-item.html` and `src/views/item-list.html`

---

## Phase 2: Foundational (Blocking Prerequisites)

**Purpose**: Core structure shared by all stories

- [ ] T004 Define shared validation helpers (required title, trim, max length) in `src/controllers/item-controller.js`
- [ ] T005 Define localStorage key conventions and persistence helpers in `src/models/item.js`
- [ ] T006 Define current-user accessor and minimal user shape in `src/models/user.js`

**Checkpoint**: Foundation ready - user story implementation can now begin

---

## Phase 3: User Story 1 - Create a New Item (Priority: P1) 🎯 MVP

**Goal**: Allow a signed-in user to create an item with a required title and optional description, receive validation feedback, and see the item immediately with creator and creation time visible.

**Independent Test**: Submit a valid item and confirm it appears with creator/time; submit without a title and see validation; cancel and confirm no item is created.

### Implementation for User Story 1

- [ ] T007 [P] [US1] Implement item creation and storage in `src/models/item.js` (fields: title, description, createdBy, createdAt, itemId)
- [ ] T008 [P] [US1] Implement user lookup for the signed-in user in `src/models/user.js`
- [ ] T009 [P] [US1] Implement create-item form markup and validation message containers in `src/views/create-item.html`
- [ ] T010 [P] [US1] Implement item list/detail display markup (title, description, creator, createdAt) in `src/views/item-list.html`
- [ ] T011 [US1] Implement submit and cancel handlers in `src/controllers/item-controller.js` (validate, save, show confirmation, reset)
- [ ] T012 [US1] Wire controller initialization in `src/index.html` to bind the create form and list views
- [ ] T013 [US1] Implement list refresh after creation in `src/controllers/item-controller.js` to surface the new item within 5 seconds

**Checkpoint**: User Story 1 is fully functional and testable independently

---

## Phase 4: Polish & Cross-Cutting Concerns

**Purpose**: Refinements that touch multiple parts of the story

- [ ] T014 Review `UC-01.md` and `UC-01-AT.md` against implemented flow; update `specs/001-create-feature/quickstart.md` if steps differ

---

## Dependencies & Execution Order

### Phase Dependencies

- **Setup (Phase 1)**: No dependencies - can start immediately
- **Foundational (Phase 2)**: Depends on Setup completion - BLOCKS all user stories
- **User Story 1 (Phase 3)**: Depends on Foundational completion
- **Polish (Phase 4)**: Depends on User Story 1 completion

### User Story Dependencies

- **User Story 1 (P1)**: Can start after Foundational (Phase 2) - no dependencies on other stories

### Dependency Graph

Setup → Foundational → US1 (MVP) → Polish

---

## Parallel Example: User Story 1

Tasks that can run in parallel after Foundational:

T007, T008, T009, T010

---

## Implementation Strategy

### MVP First (User Story 1 Only)

1. Complete Phase 1: Setup
2. Complete Phase 2: Foundational
3. Complete Phase 3: User Story 1
4. Validate the independent test for User Story 1

### Incremental Delivery

1. Complete Setup + Foundational → Foundation ready
2. Implement User Story 1 → Validate independently → Demo
3. Polish cross-cutting details

---

## Notes

- [P] tasks = different files, no dependencies
- Each user story should be independently completable and testable
- Avoid cross-story dependencies that break independence
