# AI-Assisted Learning Project Starter Kit v0.3

**Document:** Starter Kit README
**Document ID:** README.md
**Version:** 0.3
**Status:** Starter Kit
**Owner:** Curriculum Architect
**Authority:** Starter Kit Baseline

## Purpose

Version 0.3 extends the v0.2 onboarding model with lightweight cross-chat
continuity.

The framework remains subject-neutral and learner-centered.

## v0.3 continuity principle

At a chat boundary, preserve relevant learner context, but determine activity
from the learner's current intent rather than assuming continuation from project
history.

Project memory may help with continuity, but it is not treated as a
deterministic curriculum-state store.

Durable project sources and explicit learner requests remain the basis for
important state and decisions.

## Learner continuity

Preserve lightweight, broadly reusable context where useful, such as:

- background and role;
- relevant experience;
- established learning preferences;
- broad learning history;
- known strengths;
- recurring difficulties.

Do not require the learner to maintain extensive state manually.

Do not assume the current curriculum is the purpose of every new chat.

## Current-chat intent paths

A new chat should interpret the learner's current request using these paths:

1. **Explicit continuation** — resume the relevant current curriculum.
2. **Related extension** — treat the request as related context first.
3. **Explicit new topic** — retain reusable learner context and perform
   topic-specific calibration for the new topic.
4. **General exploration** — enter topic discovery rather than automatically
   continuing the current curriculum.
5. **Ambiguous request** — ask one focused clarification.

If a request derives meaning from the current curriculum, treat it as related
context first.

If it establishes an independently meaningful learning goal, consider it a new
topic.

## Existing onboarding model

When a genuinely new topic requires onboarding, retain the v0.2 stages:

1. Learner exploration, using already-known learner context where appropriate.
2. Topic confirmation or discovery.
3. Topic-specific calibration.
4. Tailored curriculum.

Do not restart learner exploration unnecessarily when stable learner context is
already available.

## v0.3 test objective

Verify that separate chats can preserve useful learner continuity without
forcing continuation of the previous curriculum or creating manual
administration.

The test plan covers continuation, related extension, new topic, general
exploration, and ambiguity.
