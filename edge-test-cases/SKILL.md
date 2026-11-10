---
name: edge-test-cases
description: Generate high-value edge-case tests from requirements and code behavior. Use when writing test plans, expanding test coverage, or when the user asks for tricky or boundary test scenarios.
disable-model-invocation: true
---

# Edge Test Cases

## Goal

Find test scenarios that are likely to reveal bugs, regressions, or unsafe assumptions.

## Edge-Case Categories

Always scan these categories:

1. Boundary values (min, max, off-by-one)
2. Empty and missing inputs
3. Invalid formats and malformed data
4. Duplicate, out-of-order, or conflicting inputs
5. Large inputs and performance-sensitive paths
6. Time, locale, timezone, and encoding differences
7. Partial failures, retries, and interruptions
8. Permission and authentication states

## Output Template

For each test case provide:

- Scenario
- Why this can fail
- Expected result
- Suggested test type (unit/integration/e2e)

## Prioritization

Rank tests by:

1. User impact if broken
2. Likelihood of occurrence
3. Difficulty of detection without tests

Focus on fewer, high-signal tests rather than long unprioritized lists.
