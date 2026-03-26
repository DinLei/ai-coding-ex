---
name: coder-refine-debug
description: Debug or refine a coding interview solution after a failure, bug, complexity issue, or new interviewer requirement appears. Use when the user provides a failing case, error, or requested change and wants a minimal, reasoned fix.
effort: high
---

# coder-refine-debug

Use this skill when an existing solution needs to be corrected or adjusted.

## Goals
- Identify root cause
- Propose the smallest effective fix
- Preserve working parts of the original solution
- Add regression-oriented tests
- Explain whether complexity or correctness changes

## Rules
- Do not rewrite everything unless the current approach is fundamentally broken
- Prefer minimal diffs conceptually
- Distinguish between:
  - logic bug
  - boundary bug
  - data structure misuse
  - complexity issue
  - misunderstanding of problem requirements
  - algorithmic bugs
  - language-specific bugs
- If a full redesign is needed, state that clearly and explain why

## Language Handling
- Default language: Python
- If the user specifies a language (e.g., C++, Java), follow that language strictly
- If a language has been specified earlier in the conversation, continue using it
- If unclear, ask or default to Python

## Output format

### 1. Problem Diagnosis
State:
- observed failure
- likely root cause
- category of issue

### 2. Fix Plan
Explain:
- what should change
- why that fixes the issue
- whether the chosen approach still remains valid

### 3. Updated Code
Provide the corrected solution.

### 4. Regression Tests
Provide a small set of tests, including:
- the failing case
- at least one nearby edge case
- one normal case

### 5. Post-Fix Review
State:
- whether correctness improved
- whether complexity changed
- any remaining risks

## Style
- Be surgical
- Keep the reasoning explicit
- Optimize for fast interview recovery
