---
name: coder-explain-concept
description: Explain an algorithm, data structure, or coding interview concept that the user does not fully understand yet. Use when the user asks for a quick concept refresher or a from-scratch explanation before solving the problem.
effort: medium
---

# coder-explain-concept

Use this skill when the user needs a concept explained before continuing the coding interview workflow.

## Modes
Infer one of these two modes from the user's request:

### Mode A: Refresher
Use when the user has heard of the concept but forgot details.

### Mode B: From Scratch
Use when the user does not know the concept at all.

## Rules
- Do not over-teach unrelated theory
- Focus on interview usefulness
- Prefer intuition + minimal examples
- Do not write a full problem solution unless the user explicitly asks
- Small pseudocode-like descriptions are okay only if necessary, but avoid full implementation

## Language Handling
- Keep analysis language-neutral by default
- If the user specifies a language, only include language-specific considerations when relevant
- When mentioning data structures, optionally map to:
  - Python / C++ / Java equivalents if helpful

## Output format

### 1. What It Is
Define the concept simply.

### 2. Why It Exists
Explain what problem it helps solve.

### 3. Core Intuition
Explain the key invariant, mechanism, or mental model.

### 4. Minimal Example
Give a tiny example that makes the idea concrete.

### 5. Typical Use Cases
List common interview scenarios where this concept appears.

### 6. Common Mistakes
List the most likely misunderstandings or bugs.

### 7. What to Watch for in This Problem
Relate the concept back to the current problem if applicable.

## Style
- If the user sounds rusty, optimize for fast recall
- If the user sounds unfamiliar, build intuition first
- Avoid unnecessary historical or academic detail
