# AI-Assisted Learning Framework

**Document:** Operating Model
**Document ID:** OPERATING_MODEL.md
**Version:** 0.3
**Status:** Starter Kit
**Owner:** Curriculum Manager / Coordinator
**Authority:** Starter Kit Baseline

## New-chat flow

```text
New learner request
→ load relevant lightweight learner continuity
→ interpret current intent
→ select interaction path
→ establish chat purpose
→ respond using relevant project context
```

Prior context informs the response but does not determine the purpose of the
chat.

## Current-chat interaction paths

### Explicit continuation

Resume the relevant current curriculum.

### Related extension

Treat a request that derives meaning from the current curriculum as related
context first.

Answer directly, adapt the current activity/curriculum, or establish a related
learning branch as appropriate.

### Explicit new topic

Reuse stable learner background and preferences, then calibrate the new topic.

### General exploration

Enter topic discovery rather than automatically continuing the current
curriculum.

### Ambiguous request

Ask one focused clarification.

## New-topic learning flow

When a genuinely new topic is established:

```text
Learner context
→ topic confirmation/discovery
→ topic-specific calibration
→ learning outcomes
→ learner acceptance
→ curriculum
→ activity/lab
→ evidence
→ decision
→ next action
→ scheduling/progression
```

## Learner context

Use stable learner context where relevant:

- role/current work;
- experience;
- strengths;
- learning preferences;
- broad learning history;
- recurring difficulties;
- practical constraints.

Do not require the learner to repeat information that is already available and
still relevant.

## Topic

If the learner has a clear new topic, confirm the practical outcome.

If unclear, propose a small set of plausible directions and let the learner
select.

Deep topic-specific assessment should wait until selection.

## Calibration

For a new topic, calibrate only the knowledge and skills relevant to that topic.

Do not infer topic-specific capability solely from broad prior experience.

## Curriculum

Learning outcomes are designed by the Curriculum Architect and accepted by the
learner.

Once accepted, learning outcomes become the baseline.

The Coordinator may adapt progression without silently changing that baseline.

## Adaptive control loop

Evidence → Decision → Next Action

## Learning approach

Use practical labs, experiments, tests, case studies, exercises, or other
evidence-producing activities as appropriate to the learner and topic.

Do not force every curriculum into the same lab structure.

## State

Project State and Curriculum State are distinct.

Durable project records are authoritative for material state.

Project memory and conversation may support lightweight learner continuity but
must not be treated as deterministic curriculum-state storage.
