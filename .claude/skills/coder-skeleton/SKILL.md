---
name: coder-skeleton
description: Generate a language-appropriate function or class skeleton for a coding interview problem based on a chosen approach. Use when the user wants only the structure and step-by-step implementation plan, without the full code.
effort: medium
---

# coder-skeleton

Use this skill to create an implementation-ready skeleton without writing the actual solution.

## Goals
- Provide a clean, interview-appropriate function or class signature
- Reflect the selected approach in structured comments
- Keep the structure easy to complete during a live interview
- Avoid filling in actual algorithm logic
- Optionally include helper function signatures without implementations

## Rules
- Do not write the full implementation
- Do not hide real logic inside dense comments
- Keep comments aligned with the previously chosen approach
- If input format is ambiguous, state assumptions before the skeleton
- Match the structure to common interview platform expectations (e.g., LeetCode)

## Language Handling
- Default language: Python
- If the user specifies a language (e.g., C++, Java), follow that language strictly
- If a language has been specified earlier in the conversation, continue using it
- If unclear, ask or default to Python

### Language-Specific Conventions

#### Python
- Use a function-based solution
- Include type hints when helpful
- Use `#` for comments

#### C++
- Use `class Solution` if appropriate
- Use STL types (e.g., vector, unordered_map)
- Use `//` for comments
- Prefer pass-by-reference when reasonable

#### Java
- Use `class Solution` with a public method
- Use standard collections (e.g., ArrayList, HashMap)
- Use `//` for comments
- Keep structure simple and interview-friendly

## Output format

### 1. Assumptions
State:
- input format
- output format
- platform-specific expectations (if any)

### 2. Skeleton Code
Provide:
- language-appropriate function or class signature
- structured step-by-step comments inside the main function
- helper function signatures only if clearly needed

### 3. Mapping to Plan
Briefly map:
- each comment block → corresponding algorithm step

## Style
- Clean and minimal
- Easy to complete live
- Language-idiomatic but not overengineered