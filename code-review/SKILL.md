---
name: code-review
description: Review code for correctness, maintainability, and risk. Use when examining pull requests, local diffs, refactors, or when the user asks for a review.
disable-model-invocation: true
---

# Code Review

## Review Priorities

Assess changes in this order:

1. Correctness and regressions
2. Security and data safety
3. Reliability and error handling
4. Test adequacy
5. Readability and maintainability

## Output Format

Provide findings first, ordered by severity.

- **Critical**: Must fix before merge
- **Major**: High-value fix, likely bug or risk
- **Minor**: Improvement suggestion

For each finding include:

- What is wrong
- Why it matters
- How to fix it

If no issues are found, state that clearly and list residual risks or test gaps.

## Review Checklist

- Inputs validated and assumptions explicit
- Null/empty/error cases handled
- No hidden side effects
- Boundaries and defaults are safe
- Tests cover happy path and key failures
- Naming and structure are clear
