<!-- Sync Impact Report:
- Version change: N/A (template) -> 1.0.0
- Modified principles:
  - PRINCIPLE_1_NAME placeholder -> I. Spec-Kit Incremental Workflow
  - PRINCIPLE_2_NAME placeholder -> II. Use Case & Acceptance Test Files
  - PRINCIPLE_3_NAME placeholder -> III. Strict MVC Architecture
  - PRINCIPLE_4_NAME placeholder -> IV. Vanilla Web Stack Only
  - PRINCIPLE_5_NAME placeholder -> V. No Repository or Implementation Changes at This Stage
- Added sections: None
- Removed sections: None
- Templates requiring updates:
  - OK .specify/templates/plan-template.md
  - OK .specify/templates/spec-template.md
  - OK .specify/templates/tasks-template.md
  - PENDING .specify/templates/commands/*.md (directory not found)
- Follow-up TODOs: None
-->
# CMS Constitution

## Core Principles

### I. Spec-Kit Incremental Workflow
The CMS MUST be developed incrementally using Spec-Kit. Each use case MUST be treated as an
independent feature developed in its own Git branch. Rationale: This keeps the workflow aligned
with the Spec-Kit pipeline and isolates feature changes.

### II. Use Case & Acceptance Test Files
All use cases MUST be stored as Markdown files named `UC-XX.md`. All acceptance tests MUST be
stored as Markdown files named `UC-XX-AT.md`. Rationale: Spec-Kit expects these filenames as
inputs.

### III. Strict MVC Architecture
The CMS MUST follow a strict Model-View-Controller (MVC) architecture. Rationale: This enforces
the required separation of concerns.

### IV. Vanilla Web Stack Only
Implementation MUST use only vanilla HTML, CSS, and JavaScript. Frameworks, external libraries,
or unstated technologies MUST NOT be introduced. Rationale: This preserves the approved tech
stack.

### V. No Repository or Implementation Changes at This Stage
Do not initialize or modify the git repository. Do not generate implementation code at this
stage. Rationale: This step is limited to constitution and documentation setup only.

## Additional Constraints

No additional constraints beyond the Core Principles.

## Development Workflow

Follow the Spec-Kit incremental workflow; each use case remains an independent feature in its
own Git branch.

## Governance

- Amendments require updating this `constitution.md` file with explicit instruction and
  recording the change in the Sync Impact Report.
- Versioning follows semantic versioning: MAJOR for backward-incompatible governance or
  principle removals/redefinitions, MINOR for new principles/sections or material expansions,
  PATCH for clarifications and typo-level changes.
- Every Spec-Kit artifact (spec, plan, tasks) MUST include a Constitution Check that verifies
  compliance with the Core Principles before proceeding.

**Version**: 1.0.0 | **Ratified**: 2026-02-02 | **Last Amended**: 2026-02-02
