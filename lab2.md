# ECE 493 Software Systems Design Project

**Winter 2026**

## Laboratory #2

**Instructor:** Dr. Scott Dick
**Due Date:** Monday, Feb. 9, 2026 — 11:59:59 pm

---

## Additional Resources

Discussion

The core deliverable for this class, or any software development project, is correct and working code. In this lab we look at the code-generation process using **Spec-Kit** and **Codex**. Agentic development involves having the AI pass through several intermediate steps, each time reasoning about the model of code to be built and adding those findings to its context. This added context yields code of much higher quality, approaching or reaching release-candidate status.

As we know, however, the AI cannot simply be allowed to run free. What has become clear in the last six months is that the AI should only build software incrementally, one small piece at a time, with the intermediate artifacts it produces each being validated before it is allowed to proceed to the next step.

Our work in developing and validating detailed use cases and acceptance tests will now serve as the foundation for this incremental process; each use case will be a feature for the CMS, which will be created independently in its own branch of the source tree. As you proceed through the use cases, expect to see Codex doing a lot of rework of existing code files to accommodate each new use case. **THIS IS FINE** — it is the AI doing that work, not you.

Your job is to validate the high-level and detailed plans in each use case.

> **IMPORTANT NOTE:** When you see something that isn’t right in any validation, do **not** manually fix the generated files. Re-generate them by re-issuing the previous slash command with additional instructions. This keeps the entire context synchronized.

---

## Spec-Kit Workflow Overview

Spec-Kit introduces a multi-step workflow for each feature. These include mandatory intermediate generations and optional cross-checks. In this lab, **all optional checks will be used**. These processes follow the flowchart shown in Figure 1.

> *(Figure 1 referenced in original document)*

These commands are run within the command-line interface of your code generator. In our case:

1. Install **Codex**
2. Install **Spec-Kit**
3. Set up your **git repository**
4. Copy your use-case and acceptance-test files into the repository root
5. Launch **Codex**

Spec-Kit commands are then available as slash commands within the Codex CLI.

---

## Spec-Kit Command Sequence

### 1. `/speckit.constitution` *(run once per project)*

Defines the high-level principles for your implementation.

Example constraints:

* Use cases stored as `UC-XX.md`
* Acceptance tests stored as `UC-XX-AT.md`
* CMS implemented using MVC
* Vanilla HTML, CSS, and JavaScript only

Codex will prepare the repository (it *can* set one up for you, but this consumes tokens — avoid spending tokens on tasks you can do yourself).

**Output:** `constitution.md`

**Validation:**

* Read `constitution.md`
* Confirm it accurately repeats what you specified
* Re-generate if needed

---

### 2. `/speckit.specify`

Converts your specification into a format understood by Spec-Kit.

* Use-case flows should be copied directly
* Functional requirements should be extracted from the flows

#### a. `/speckit.clarify` *(optional validation — required for this lab)*

Raises ambiguities in `spec.md` or `constitution.md`.

**Reporting:**

* Respond to clarifications in Codex
* Record questions and your responses in your lab report

#### b. Validation

* Confirm `spec.md` repeats the use-case information (especially flows)
* No semantic changes beyond grammar or style
* Functional requirements must match the use case

---

### 3. `/speckit.plan`

Generates high-level planning documents:

* Architecture
* Tech stack
* Data model
* Interface contracts

#### a. `/speckit.checklist` *(optional validation — required)*

Compares generated plans against common quality checklists (UX, security, etc.).

**Reporting:**

* Record checklist items not completed
* Decide whether they are necessary for the CMS
* Re-run plan or spec steps if needed

#### b. Validation

* Confirm `plan.md` matches your intent from the constitution
* Confirm `data_model.md` and `./contracts/` align with `spec.md`
* **After all branches are complete:** combine all `data_model.md` files into one ER diagram

---

### 4. `/speckit.tasks`

Breaks the plan into individual AI-sized task steps.

#### a. `/speckit.analyze` *(optional validation — required)*

Checks consistency and coverage across:

* `spec.md`
* planning files
* `tasks.md`

**Reporting:**

* Save the generated table to a file
* Include it in your report
* Document actions taken to resolve issues

#### b. Validation

* Confirm there are **no blocking dependencies** in `tasks.md`

---

## Requirements

You must:

* Install **Codex CLI**, **Spec-Kit**, and **git**
* Windows users must use **WSL**
* Set up a git repository for your project
* Copy use cases and acceptance tests from **Lab #1** into the repo root
* Launch Codex and run:

```text
/speckit.init
```

---

## Submission

After completing planning and task preparation for all branches, submit:

* `constitution.md`
* All required reports and validations
* Zipped into a **single archive**

Upload via the Canvas lab page by the deadline.

> *Implementation and testing of the CMS will be examined in Lab #3.*

---

## Grading Breakdown

* Constitution file — **10%**
* `/speckit.clarify` report — **10%**
* Specification validation — **20%**
* `/speckit.checklist` report — **10%**
* Plan validation — **20%**
* `/speckit.analyze` report — **10%**
* Tasks validation — **20%**
