---
name: coder-evaluate-test
description: Evaluate a coding interview solution for correctness, complexity, edge cases, and interview readiness. Use when the user already has code and wants a dry run, risk review, and test coverage analysis before or after execution.
effort: high
---

# coder-evaluate-test

Use this skill to assess an existing solution rather than rewrite it immediately.

## Goals
- Check correctness at a high level
- Dry-run a representative case
- Identify weak edge-case coverage
- Verify complexity against likely constraints
- Predict interview follow-up risks
- Avoid unnecessary rewrites

## Rules
- Do not immediately replace the code with a different solution
- Evaluate first, rewrite only if the user explicitly asks
- Be specific about failure modes
- If the code is incomplete, assess the intended logic as far as possible

## Output format

### 1. Correctness Check
State:
- whether the core approach appears correct
- any obvious logical flaws
- any hidden assumptions or unhandled scenarios

### 2. Dry Run
Use one representative test case and walk through:
- major state changes
- key variable updates
- where correctness depends on a specific invariant

### 3. Edge Case Coverage
List critical edge cases:
- which ones matter most
- whether the current solution likely handles them

### 4. Complexity Review
State:
- time complexity
- space complexity
- whether they are likely acceptable

### 5. Interview Risk Check
List likely follow-up questions or points of challenge from an interviewer.

### 6. Verdict
Give one of:
- ready
- mostly ready with minor risks
- not interview-safe yet

## Style
- Evaluate before editing
- Keep the review concrete and actionable
