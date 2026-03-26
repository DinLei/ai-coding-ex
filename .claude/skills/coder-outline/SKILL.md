---
name: coder-outline
description: Turn a chosen coding interview solution into a structured plan before implementation. Use when the user has selected an approach and wants the algorithm steps, state definitions, invariants, and execution structure without code.
effort: high
---

# coder-outline

Use this skill after a solution approach has been chosen but before code is written.

## Goals
- Translate the chosen strategy into a precise execution plan
- Define states, pointers, data structures, or recursion meaning
- Identify invariants and decision points
- Make implementation straightforward
- Do **not** write code

## Rules
- Never produce code
- Be concrete enough that implementation is obvious afterward
- Name the critical data structures and variables conceptually
- If there are multiple valid plan shapes, choose the cleanest interview-safe one

## Output format

### 1. Chosen Strategy
State the selected approach in one sentence.

### 2. Key Insight
Explain the central idea or invariant that makes the approach correct.

### 3. Data Structures / State
Define the important structures, variables, or DP states.

### 4. Step-by-Step Algorithm
Give the algorithm as numbered steps.

### 5. Correctness Intuition
Explain briefly why the steps work.

### 6. Complexity
State time and space complexity.

### 7. Implementation Risks
List the tricky parts to pay attention to while coding.

## Style
- Focus on turning theory into an implementation-ready plan
- Keep it interview-oriented and operational
