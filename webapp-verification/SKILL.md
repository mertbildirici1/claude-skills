---
name: webapp-verification
description: Verify webapp behavior through interactive UI testing, including click-through flows, state transitions, and error handling. Use after implementation, before demo, or when validating fixes in a browser.
disable-model-invocation: true
---

# Webapp Verification

## Goal

Validate that the implemented webapp works for real user flows, not just code-level expectations.

## Parallel Usage

Use this skill together with `code-review`:

- `code-review` checks code risks and structure.
- `webapp-verification` checks runtime behavior and user experience.

Run both in parallel when time allows.

## Verification Order

1. Smoke check app startup and critical route load.
2. Validate primary user flow end-to-end.
3. Validate empty/loading/error states.
4. Validate edge interactions and input boundaries.
5. Re-run the primary flow after fixes.

## Browser Workflow (Chrome DevTools MCP)

When Chrome DevTools MCP is available:

1. Open the app and wait for stable render.
2. Click through primary flows like a user.
3. Fill forms with valid and invalid inputs.
4. Observe visible output and network/error signals.
5. Record exact repro steps for each issue.

If MCP is unavailable, do the same workflow with manual browser checks.

## Must-Check Scenarios

- First render with no data
- Loading indicators and disabled states
- Error message behavior on failed actions
- Form validation messages and submit behavior
- Multiple rapid clicks and duplicate submissions
- Back/forward navigation and state consistency
- Refresh behavior and persisted state expectations

## Reporting Format

For each issue, report:

- Severity: critical / major / minor
- Repro steps
- Expected behavior
- Actual behavior
- Suspected area (if known)

If no issues are found, report what was verified and what remains untested.
