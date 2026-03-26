---
name: coder-implement
description: Implement a complete solution for a coding interview problem using the previously chosen approach. Use when the user is ready for full code after problem clarification and design are complete.
effort: high
---

# coder-implement

Use this skill to produce the full implementation once the problem and solution approach are already settled.

## Goals
- Write a correct, interview-appropriate solution
- Preserve the selected approach
- Use clear structure and readable naming
- Keep comments helpful but not excessive
- Ensure the code is valid for the chosen language

## Rules
- Do not change the chosen approach unless necessary; if you must, explain why first
- Prefer clarity over clever micro-optimizations
- Keep the solution realistic for a live coding interview
- Avoid unnecessary abstraction or overengineering
- If helper functions improve clarity, use them
- If important assumptions are needed, state them explicitly before the code

## Language Handling
- Default language: Python
- If the user specifies a language (e.g., C++, Java), follow that language strictly
- If a language has been specified earlier in the conversation, continue using it
- If unclear, ask or default to Python

### Language-Specific Conventions

#### Python
- Use function-based solutions
- Use type hints when helpful
- Prefer built-in data structures (list, dict, set)
- Avoid overly concise tricks that hurt readability

#### C++
- Use STL (vector, unordered_map, etc.)
- Use references where appropriate
- Avoid complex templates or metaprogramming
- Ensure code compiles cleanly
- Watch for edge cases like overflow or indexing

#### Java
- Use `class Solution` structure
- Use standard collections (ArrayList, HashMap, etc.)
- Avoid unnecessary object wrappers
- Keep code straightforward and readable

## Output format

### 1. Implementation Notes
Briefly state:
- assumptions
- platform-specific considerations (if any)

### 2. Code
Provide the full solution in the selected language.

### 3. Walkthrough
Briefly explain:
- the structure of the solution
- key invariants or logic points
- time and space complexity

## Style
- Interview-oriented
- Correct and readable
- Language-idiomatic but simple
- Avoid overengineering