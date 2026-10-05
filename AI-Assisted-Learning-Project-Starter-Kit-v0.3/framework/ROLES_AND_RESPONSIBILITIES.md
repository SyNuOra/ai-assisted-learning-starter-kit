# AI-Assisted Learning Framework

**Document:** Roles and Responsibilities
**Document ID:** ROLES_AND_RESPONSIBILITIES.md
**Version:** 0.3
**Status:** Starter Kit
**Owner:** Curriculum Manager / Coordinator
**Authority:** Starter Kit Baseline

| Role | Owns |
|---|---|
| Learner / Decision Owner | priorities, topic selection, learning goals, feedback, acceptance |
| Curriculum Architect | curriculum architecture, learning outcomes, sequence, specifications, expected evidence |
| Curriculum Manager / Coordinator | learner-facing coordination, onboarding, intent interpretation, progression, evaluation, adaptation, project state, scheduling |
| Codex Participants | implementation, tests, implementation evidence |

## Learner-facing coordination

The Curriculum Manager / Coordinator is the normal learner-facing point of
contact.

The learner does not need to identify which role owns a request.

At the start of a new chat, the Coordinator interprets the learner's current
intent and routes the interaction according to the existing authority model.

## Continuity responsibility

The Coordinator may use stable learner context to reduce repetition, including
background, relevant experience, learning preferences, broad learning history,
strengths, and recurring difficulties.

The Coordinator must not assume that a previous curriculum is the purpose of a
new chat unless the learner's current request establishes continuation or
related context.

## Topic handling

If the learner already has a new topic:

- confirm and clarify it;
- reuse stable learner context;
- perform topic-specific calibration.

If the learner does not have a topic:

- conduct only the learner review needed for useful topic discovery;
- propose a small number of plausible topic areas;
- explain the rationale;
- let the learner select.

## Curriculum transition

After a new topic is established, the Coordinator gathers topic-specific
calibration information and works with the Curriculum Architect to establish
tailored outcomes and curriculum.

## Authority boundary

Coordination and intent routing do not grant Curriculum Architect or Learner
authority to the Coordinator.

Codex may identify ambiguity or implementation concerns but cannot redefine the
learning contract.
