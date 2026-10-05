# AI-Assisted Learning Framework

**Document:** Revision and Decisions
**Document ID:** REVISION_AND_DECISIONS.md
**Version:** 0.3
**Status:** Starter Kit
**Owner:** Curriculum Architect
**Authority:** Starter Kit Baseline

## Purpose

Record significant Starter Kit design decisions and the rationale for changes
between accepted baselines.

## ADR-001 — v0.3 Learner Continuity and Current-Chat Intent

**Status:** Accepted for v0.3 candidate

**Decision:** Introduce lightweight learner continuity across chats while making
the learner's current request the primary determinant of each chat's purpose.

At the start of a new chat:

1. load relevant lightweight learner continuity context;
2. interpret the learner's current request;
3. determine the appropriate interaction path;
4. establish the purpose of the chat from the current request;
5. use prior learner context to inform the response without assuming
   continuation.

The supported interaction paths are:

- explicit continuation;
- related extension;
- explicit new topic;
- general exploration;
- ambiguous request requiring one focused clarification.

Project memory may assist continuity but is not a deterministic curriculum-state
store.

**Rationale:** v0.2 improved initial onboarding but did not explicitly define how
separate chats should preserve useful learner context without automatically
continuing the previous curriculum. The v0.3 model reduces repeated onboarding
while preserving learner intent and low administration.

**Consequences:**

- stable learner background and preferences may be reused across chats;
- current-chat intent determines whether to continue, extend, explore, clarify,
  or start a new topic;
- genuinely new topics receive topic-specific calibration;
- learners are not required to maintain extensive state manually;
- project memory remains supportive rather than authoritative curriculum state.

**Affected documents:**

- `README.md`
- `SETUP.md`
- `PROJECT_INSTRUCTIONS.md`
- `PROJECT_CHARTER.md`
- `OPERATING_MODEL.md`
- `ROLES_AND_RESPONSIBILITIES.md`
- `LEARNER_PROFILE_TEMPLATE.md`
- `LEARNING_PROJECT_SETUP.md`
- `ONBOARDING_TEST_PLAN.md`
- `REVISION_AND_DECISIONS.md`

**Implementation status:** Complete in the v0.3 candidate.

## ADR-002 — Consistent Starter Kit Metadata

**Status:** Accepted for v0.3 candidate

**Decision:** Apply a consistent metadata block to every Markdown document in the
Starter Kit.

Each document declares:

- Document
- Document ID
- Version
- Status
- Owner
- Authority

`Document ID` is the canonical logical identity of the document and is
independent of any filename suffix that a hosting interface may add.

**Rationale:** v0.2 used consistent metadata on framework documents but not on
all root, learner, and testing documents. A consistent block improves
maintainability and makes document identity explicit.

**Consequences:** All v0.3 Markdown files use Version `0.3`, Status `Starter Kit`,
and Authority `Starter Kit Baseline`.

**Affected documents:** All v0.3 Markdown documents.

**Implementation status:** Complete in the v0.3 candidate.
