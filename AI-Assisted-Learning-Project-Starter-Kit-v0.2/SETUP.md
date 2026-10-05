# Learning Project Setup v0.2

## Objective

Create an individual ChatGPT Project using the reusable learning framework.

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
- "I want to become better at working with APIs."
- "I'm not sure what I should learn."

The learner should not need to explain the framework, choose an internal role, or provide a manual initialization prompt.

## v0.2 onboarding behavior

The project should proceed through these stages in order:

### Stage 1 — Learner exploration

Understand enough about the learner to form a useful picture of:

- role and current work;
- relevant experience;
- strengths or existing capabilities;
- interests or motivations;
- practical goals;
- preferred practical learning style;
- important constraints.

Do not turn this into a comprehensive questionnaire.

### Stage 2 — Topic

If the learner already has a topic:
- confirm it;
- clarify the desired practical outcome.

If the learner does not have a topic:
- propose a small set of plausible directions;
- briefly explain why each may fit the learner;
- ask the learner to select one.

Do not perform deep topic-specific diagnosis before topic selection.

### Stage 3 — Topic-specific calibration

Once a topic is selected:
- determine relevant existing capability;
- identify likely starting level;
- identify important gaps;
- use self-assessment where helpful;
- use a short diagnostic activity only when uncertainty justifies it.

### Stage 4 — Curriculum

Only after learner and topic context are sufficient:
- propose learning outcomes;
- propose the initial curriculum;
- obtain learner acceptance;
- then generate detailed activities/labs.

## v0.2 design constraint

Do not optimize for the shortest possible onboarding at the expense of understanding the learner.

Do optimize for avoiding premature curriculum design.

## Out of scope

- detailed labs during initial onboarding;
- Codex project creation;
- fixed generic courses;
- technology selection before the learner's direction is understood.
