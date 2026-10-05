# Starter Kit v0.3 — Continuity and Onboarding Test Plan

**Document:** Continuity and Onboarding Test Plan
**Document ID:** ONBOARDING_TEST_PLAN.md
**Version:** 0.3
**Status:** Starter Kit
**Owner:** Curriculum Manager / Coordinator
**Authority:** Starter Kit Baseline

## Goal

Determine whether the Starter Kit preserves useful learner continuity across
chats while allowing each new chat to establish its purpose from the learner's
current intent.

## Preconditions

Complete enough initial onboarding and at least one learning session so the
project has:

- learner background/context;
- an accepted current curriculum;
- some learning history or evidence.

## Test A — Explicit continuation

Complete a session in Chat A.

Open Chat B and say:

> I'm ready for the next session.

Observe whether the Coordinator:

- recognizes explicit continuation;
- uses available current curriculum context;
- does not restart onboarding;
- does not ask the learner to restate stable background unnecessarily.

## Test B — Related extension

Open another chat and ask a question whose meaning derives from the current
curriculum.

Example:

> I'm learning JavaScript, but I want to understand the standard versions of
> JavaScript and how they differ from what I've been learning.

Observe whether the Coordinator:

- recognizes related context;
- does not automatically create a new curriculum;
- determines whether to answer directly, adapt the curriculum/activity, or
  establish a related learning branch.

## Test C — Explicit new topic

Open another chat and say:

> I want to learn [new topic].

Observe whether the Coordinator:

- treats the request as a new topic;
- reuses stable learner background and preferences;
- does not assume topic-specific knowledge from the previous curriculum;
- performs proportionate topic-specific calibration;
- avoids repeating broad onboarding unnecessarily.

## Test D — General exploration

Open another chat and say:

> I'm ready to learn something new.

Observe whether the Coordinator:

- enters topic discovery;
- uses stable learner context to make discovery useful;
- does not automatically continue the current curriculum;
- proposes a small, plausible set of directions rather than a large catalogue.

## Test E — Ambiguous request

Open another chat with a request that could reasonably mean continuation or a
new direction.

Observe whether the Coordinator:

- asks one focused clarification;
- does not restart onboarding;
- does not make a major unsupported assumption.

## Test F — Memory/state boundary

Where project memory is available, repeat one of the tests after changing chats.

Observe whether:

- useful learner context reduces repetition;
- memory is not treated as authoritative curriculum state;
- the current learner request remains decisive for chat purpose;
- material curriculum state is taken from available durable project context
  rather than inferred solely from memory.

## Measures

Record:

- whether the interaction path was identified correctly;
- whether stable learner context was reused appropriately;
- whether unnecessary onboarding was repeated;
- whether prior curriculum was incorrectly assumed;
- number and relevance of clarification questions;
- whether new-topic calibration was topic-specific;
- whether the learner experienced avoidable administrative burden.

## Acceptance target

The Starter Kit passes when all five intent paths behave as specified and useful
continuity is preserved without deterministic dependence on project memory or
manual learner state maintenance.
