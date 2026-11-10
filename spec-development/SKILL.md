---
name: spec-development
description: Create human-readable specs from problem statements, including alternative designs and tradeoffs. Use when scoping features, aligning stakeholders, or choosing among multiple implementation options.
disable-model-invocation: true
---

# Spec Development

## Goal

Turn a problem into a clear, decision-ready spec that helps users compare options and pick a design.

## Spec Structure

Use this structure in order:

1. Problem statement
2. Goals and non-goals
3. Constraints and assumptions
4. Proposed approaches (at least two when possible)
5. Tradeoff analysis
6. Recommended option
7. Implementation outline
8. Test and rollout plan
9. Open questions

## Requirements for Alternative Designs

For each alternative include:

- Short description
- Advantages
- Disadvantages
- Complexity level (low/medium/high)
- Risk level (low/medium/high)
- Best-fit situations

## Decision Guidance

When recommending one option:

- Explain why it best matches goals and constraints
- State what is being traded off
- Identify when another option should be chosen instead

## Quality Bar

- Language is plain and non-ambiguous
- Scope is explicit and realistic
- Risks and unknowns are visible
- The reader can make a decision without extra context
