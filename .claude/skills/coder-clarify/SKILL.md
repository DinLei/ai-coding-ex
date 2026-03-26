---
name: coder-clarify
description: Analyze a coding interview problem before implementation. Use when the user wants to clarify the core task, inputs, outputs, constraints, ambiguities, pitfalls, and edge cases without writing code.
effort: medium
---

# coder-clarify

Use this skill to clarify and deconstruct a coding interview problem before discussing implementation.

## Goals
- Identify the exact problem being solved
- Define the input and output precisely
- Surface hidden assumptions and ambiguities
- Enumerate constraints and edge cases
- Highlight the most likely pitfalls
- Do **not** write code

## Rules
- Never produce code
- Never jump ahead into full algorithm design
- Keep the analysis practical and interview-oriented
- If the prompt is incomplete, explicitly call out what is missing
- If constraints are absent, infer reasonable possibilities and label them clearly as assumptions

## Language Handling
- Keep analysis language-neutral by default
- If the user specifies a language, only include language-specific considerations when relevant
- When mentioning data structures, optionally map to:
  - Python / C++ / Java equivalents if helpful

## Output format

### 1. Core Problem
Summarize the problem in one sentence.

### 2. Inputs
State:
- data types
- structure / format
- semantic meaning of each input
- whether inputs may be empty, duplicated, unsorted, negative, etc.

### 3. Outputs
State:
- data type
- exact expected structure / format
- any ordering or uniqueness requirements

### 4. Constraints
List:
- explicit constraints from the problem
- inferred practical constraints relevant to algorithm choice
- acceptable time/space complexity range if size is implied

### 5. Edge Cases
List the important edge cases and why each matters.

### 6. Pitfalls
List the most likely implementation or reasoning mistakes.

### 7. Ambiguities / Assumptions
Call out unclear parts of the prompt.
If needed, provide default reasonable assumptions.

## Style
- Be concise but complete
- Use bullets where helpful
- Optimize for interview readiness, not textbook completeness
