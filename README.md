# AI-Assisted Learning Project Starter Kit

A reusable starter kit for creating learner-centered, adaptive learning projects in ChatGPT.

**Current Starter Kit version:** v0.3

You can read about [my journey her](https://synuora.hashnode.dev/living-with-ai-building-my-personal-learning-assistant)
## Purpose

The Starter Kit helps a ChatGPT Project operate as an individual learning environment rather than a static course. It is subject-neutral: curricula are created within the framework, not built into it.

Core principles:

- start from the learner rather than a predefined course;
- optimize for durable understanding, retention, transfer, and practical capability;
- distinguish implementation success from evidence of learning;
- adapt progression using evidence and learner feedback;
- preserve useful learner continuity across chats without assuming every new chat continues the previous curriculum;
- keep learner administration and governance lightweight.

## v0.3: Cross-Chat Continuity

Version 0.3 introduces a lightweight continuity model.

At a chat boundary, the project may preserve useful learner context such as background, relevant experience, established learning preferences, broad learning history, known strengths, and recurring difficulties.

The learner's **current request**, however, determines the purpose of the new chat. Project memory may assist continuity, but it is not treated as a deterministic curriculum-state store.

### Current-chat intent model

A new chat is interpreted using five paths:

1. **Explicit continuation** — resume the relevant current curriculum without restarting onboarding.
2. **Related extension** — treat a request that derives meaning from the current curriculum as related context first.
3. **Explicit new topic** — reuse stable learner context, then perform topic-specific calibration.
4. **General exploration** — enter topic discovery rather than automatically continuing the current curriculum.
5. **Ambiguous request** — ask one focused clarification instead of restarting onboarding or making a major assumption.

> Preserve relevant learner context across chats, but determine activity from the learner's current intent rather than assuming continuation from project history.

## Roles

The framework separates responsibilities without requiring the learner to coordinate them.

- **Learner / Decision Owner** — owns priorities, topic selection, goals, feedback, scope decisions, and acceptance.
- **Curriculum Architect** — owns curriculum architecture, learning outcomes, sequence, detailed specifications, and expected learning evidence.
- **Curriculum Manager / Coordinator** — the normal learner-facing point of contact; owns onboarding, progression, feedback, evaluation, adaptation, project/curriculum state, and scheduling coordination.
- **Codex Participants** — when used, implement approved specifications, validate implementation, collect implementation evidence, and report specification defects.

The learner does not need to decide which internal role should handle a request.

## Adaptive Learning Loop

The core progression loop is:

```text
Evidence → Decision → Next Action
```

Evidence can lead to reinforcement, continuation, acceleration, revision, or deferral.

A working implementation alone is not proof of learning. Implementation claims require implementation evidence; learning-capability claims require learning evidence.

## Repository Structure

```text
.
├── README.md
├── SETUP.md
├── UPDATE.md
├── PROJECT_INSTRUCTIONS.md
├── framework/
│   ├── PROJECT_CHARTER.md
│   ├── OPERATING_MODEL.md
│   ├── ROLES_AND_RESPONSIBILITIES.md
│   ├── LAB_SPECIFICATION_CONTRACT.md
│   ├── EVIDENCE_AND_EVALUATION.md
│   ├── HANDOVER_AND_CHANGE.md
│   ├── OUTLOOK_COORDINATION.md
│   └── REVISION_AND_DECISIONS.md
├── learner/
│   ├── LEARNER_PROFILE_TEMPLATE.md
│   └── LEARNING_PROJECT_SETUP.md
└── testing/
    └── ONBOARDING_TEST_PLAN.md
```

## Getting Started

1. **Create a ChatGPT Project.** Project-only memory can be used when available and appropriate, but memory is not authoritative curriculum state.
2. **Configure Project Instructions.** Copy the complete contents of `PROJECT_INSTRUCTIONS.md` into the ChatGPT Project's Project Instructions.
3. **Add Project Sources.** Upload the framework and learner source documents required by the project. See [`SETUP.md`](SETUP.md).
4. **Start normally.** The learner does not need a special initialization prompt.

Example requests:

```text
I'm ready to start.
I'm ready for session 3.
I struggled with the last exercise.
I want to learn something new.
I want to learn <topic>.
```

The project uses the current request to determine the appropriate interaction path.

## Updating an Existing Project

ChatGPT Project Sources do not provide an in-place file replacement/versioning workflow in the update process this Starter Kit supports.

To update an existing project:

1. Replace the existing Project Instructions with the contents of the new `PROJECT_INSTRUCTIONS.md`.
2. Delete the old Starter Kit Project Source files from the ChatGPT Project.
3. Upload the new Starter Kit Project Source files.
4. Continue using the existing project and chats.

ChatGPT may append filename suffixes such as `(1)` or `(2)` when a filename has previously been uploaded. Do not repeatedly delete and re-upload files to remove these suffixes. The `Document ID` inside each Markdown document is its canonical logical identity.

See [`UPDATE.md`](UPDATE.md) for the complete update procedure.

## New-Topic Onboarding

When a genuinely new topic is selected, the framework uses four stages:

1. **Learner exploration** — reuse stable learner context and gather only material missing information.
2. **Topic confirmation/discovery** — confirm a named topic or help the learner choose a direction.
3. **Topic-specific calibration** — assess only knowledge and skills relevant to the selected topic.
4. **Tailored curriculum** — establish learning outcomes, obtain learner acceptance, and create the initial curriculum/activity.

The learner profile is supporting context, not a mandatory form that must be completed field by field.

## Lab and Codex Model

Where practical implementation is appropriate, a detailed lab specification acts as the contract handed to Codex. It defines the learning purpose, outcomes, intended implementation, expected implementation and learning evidence, acceptance criteria, dependencies, and out-of-scope items.

The learning objective is defined before implementation and is not inferred from the finished application.

## Scheduling

Where Outlook scheduling is available, the Curriculum Manager / Coordinator can coordinate learning activities around availability.

> The curriculum is authoritative; the calendar is its scheduling representation.

Moving a learning session should not silently change its learning objective.

## Testing

`testing/ONBOARDING_TEST_PLAN.md` covers:

- explicit continuation across chats;
- related extensions;
- explicit new topics;
- general exploration;
- ambiguous requests;
- the boundary between project memory and durable curriculum state.

## Document Identity

Starter Kit Markdown files contain a canonical `Document ID`.

If the ChatGPT Project interface adds a filename suffix such as `(1)` or `(2)`, the canonical document identity does not change. Cross-document reasoning should use the declared `Document ID`, not UI-generated suffixes.

## Versioning and Decisions

Significant Starter Kit design decisions are recorded in `framework/REVISION_AND_DECISIONS.md`.

Version 0.3 records the introduction of lightweight learner continuity, the current-chat intent model, topic-specific calibration for genuinely new topics, and consistent document metadata.

## Design Constraints

The Starter Kit intentionally avoids:

- extensive manual state maintenance;
- mandatory learner questionnaires;
- complex curriculum databases;
- deterministic dependence on project memory;
- unnecessary participant roles;
- governance that does not support an observed learning need.

## Documentation

- [`SETUP.md`](SETUP.md) — configure a new ChatGPT Project.
- [`UPDATE.md`](UPDATE.md) — update an existing project.
- [`PROJECT_INSTRUCTIONS.md`](PROJECT_INSTRUCTIONS.md) — Project Instructions to install in ChatGPT.
- [`framework/`](framework/) — operating model and governance.
- [`learner/`](learner/) — learner setup and profile templates.
- [`testing/ONBOARDING_TEST_PLAN.md`](testing/ONBOARDING_TEST_PLAN.md) — continuity/onboarding validation.

## Status

Version 0.3 is the current Starter Kit baseline described by this repository.
