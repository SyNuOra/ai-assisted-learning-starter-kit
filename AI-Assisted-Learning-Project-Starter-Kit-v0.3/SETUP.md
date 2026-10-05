# Learning Project Setup v0.3

**Document:** Learning Project Setup
**Document ID:** SETUP.md
**Version:** 0.3
**Status:** Starter Kit
**Owner:** Curriculum Manager / Coordinator
**Authority:** Starter Kit Baseline

## Objective

Create an individual ChatGPT Project using the reusable learning framework with
lightweight learner continuity across chats.

## Setup

1. Create a new ChatGPT Project.
2. Prefer project-only memory when available and appropriate.
3. Paste `PROJECT_INSTRUCTIONS.md` into Project Instructions.
4. Upload all files under `framework/` as Project Sources.
5. Upload learner templates under `learner/` as Project Sources.
6. Upload `testing/ONBOARDING_TEST_PLAN.md` if the project is being evaluated.
7. Start a new chat with an ordinary learner request.

Examples:

- "I'm ready to start."
- "I'm ready for session 3."
- "I struggled with the last exercise."
- "I want to learn something new."
- "I want to learn [new topic]."

The learner should not need to explain the framework, choose an internal role,
or provide a manual initialization prompt.

## New-chat initialization

At the start of a new chat:

1. Load relevant lightweight learner continuity context from available project
   context.
2. Interpret the learner's current request.
3. Determine the appropriate interaction path.
4. Use the current request to establish the purpose of the chat.
5. Use prior learner context to inform the response without assuming the learner
   wants to continue the previous curriculum.

Project memory may assist this process but must not be treated as a
deterministic curriculum-state store.

## Interaction paths

### Explicit continuation

If the learner clearly requests continuation, resume the relevant current
curriculum using available project context.

Do not restart onboarding.

### Related extension

If the request derives meaning from the current curriculum, treat it as related
context first.

Determine whether to:

- answer directly;
- adapt the current curriculum/activity;
- treat it as a related learning branch.

Do not automatically create a new curriculum.

### Explicit new topic

Retain stable learner background and preferences.

Perform topic-specific calibration for the new topic rather than assuming
knowledge transfers from the previous topic.

Do not repeat broad learner exploration unless the existing learner context is
insufficient or outdated.

### General exploration

If the learner asks to learn something new without naming a topic, enter topic
discovery.

Do not automatically continue the current curriculum.

### Ambiguous request

Ask one focused clarification when the intended path is not clear.

Do not restart full onboarding merely because intent is ambiguous.

## New-topic onboarding

For a genuinely new topic, use the existing stages as needed:

1. Learner exploration — reuse stable context and fill only material gaps.
2. Topic confirmation/discovery.
3. Topic-specific calibration.
4. Tailored curriculum.

## Design constraint

Keep continuity lightweight.

Do not introduce extensive manual state maintenance, mandatory forms, complex
curriculum databases, or deterministic dependency on project memory.
