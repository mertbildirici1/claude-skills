---
name: live-coding-plan
description: Create time-boxed live coding plans for webapp interviews with clear milestones, scope control, and communication checkpoints. Use when preparing or starting a coding challenge.
disable-model-invocation: true
---

# Live Coding Plan

## Goal

Deliver a working webapp solution within interview time while showing strong engineering judgment.

## Planning Rules

1. Build the smallest complete MVP first.
2. Timebox each phase and keep buffer for debugging.
3. Defer non-critical polish until core flow works.
4. State assumptions early and verify with the interviewer.
5. Keep communication concise and decision-focused.

## Plan Template

Use this structure:

1. **Clarify (10%)**
   - Restate the problem in one sentence.
   - Ask 3-5 high-signal questions about scope, data, and constraints.
   - Confirm success criteria.

2. **Design (15%)**
   - Outline component/data flow at a high level.
   - Choose one implementation approach and name one fallback.
   - List top 3 edge cases to handle.

3. **Implement MVP (50%)**
   - Build happy path end-to-end first.
   - Add loading/error/empty states.
   - Keep code straightforward and explain tradeoffs while coding.

4. **Test and Fix (15%)**
   - Run critical path manually.
   - Add or describe a few high-value tests.
   - Fix highest-risk bugs first.

5. **Wrap-Up (10%)**
   - Demo what works.
   - Call out tradeoffs and deferred improvements.
   - Describe next steps if more time existed.

## Timebox Outputs

At the end of each phase, provide a one-line status update:

- done
- in-progress
- blocked (with reason and fallback)

## Failure Recovery

If behind schedule:

1. Drop non-essential UI polish.
2. Reduce abstractions to direct implementation.
3. Prioritize correctness of one complete user flow.
4. Narrate scope cuts explicitly.
