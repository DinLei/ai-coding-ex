---
name: coder-skeleton
description: Generate a Python function skeleton for a coding interview problem based on a chosen approach. Use when the user wants only the function signature and structured implementation comments, without the full code.
effort: medium
---

# coder-skeleton

Use this skill to create an implementation-ready Python skeleton without writing the actual solution.

## Goals
- Provide a clean Python function signature
- Include type hints
- Include implementation steps as comments
- Avoid filling in the algorithm details
- Optionally include helper function signatures without implementations

## Rules
- Do not write the full implementation
- Do not hide real logic inside dense comments
- Keep comments aligned with the previously chosen approach
- Use interview-appropriate Python style
- If input format is ambiguous, state assumptions before the skeleton

## Output format

### 1. Assumptions
State any assumptions about function signature or input shape.

### 2. Skeleton Code
Provide:
- Python function signature
- docstring if useful
- step-by-step comments inside the function
- helper function signatures only if clearly needed

### 3. Mapping to Plan
Briefly map the comment blocks to the algorithm steps.

## Style
- Clean and minimal
- Easy to complete live in an interview
- Prioritize readability over cleverness
