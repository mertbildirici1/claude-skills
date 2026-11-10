---
name: concise-clean-code
description: Write concise, clean, readable code with clear structure and minimal complexity. Use when implementing new features, refactoring existing code, or when the user asks for cleaner or simpler code.
disable-model-invocation: true
---

# Concise Clean Code

## Goal

Produce code that is easy to read, easy to change, and hard to misuse.

## Rules

1. Prefer straightforward logic over clever shortcuts.
2. Keep functions focused on one responsibility.
3. Use clear names that communicate intent.
4. Remove duplication when it improves clarity.
5. Add brief comments only when intent is not obvious from the code.
6. Handle expected errors explicitly.
7. Match project conventions instead of introducing new patterns.

## Workflow

1. Restate the requirement in one sentence.
2. Implement the smallest correct solution.
3. Do one cleanup pass for naming and structure.
4. Validate behavior with tests or quick checks.
5. Remove unnecessary code and comments.

## Definition of Done

- Code is readable without extra explanation.
- No dead code or avoidable complexity remains.
- Error paths are handled clearly.
- Changes are limited to what the task requires.
