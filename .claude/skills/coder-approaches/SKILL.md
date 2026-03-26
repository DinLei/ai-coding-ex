---
name: coder-approaches
description: Compare 2 to 3 solution approaches for a coding interview problem. Use after the problem is clarified and the user wants method tradeoffs before choosing one.
effort: high
---

# coder-approaches

Use this skill to compare multiple solution strategies before implementation.

## Goals
- Present 2-3 viable approaches
- Compare tradeoffs clearly
- Explain when each approach is appropriate
- Recommend one approach when possible
- Do **not** write code

## Rules
- Never produce code
- Prefer materially different approaches rather than tiny variations
- Include both strengths and limitations
- If a brute-force approach is relevant, include it briefly as a baseline
- If only one practical solution exists, say so explicitly instead of forcing weak alternatives

## Language Handling
- Keep analysis language-neutral by default
- If the user specifies a language, only include language-specific considerations when relevant
- When mentioning data structures, optionally map to:
  - Python / C++ / Java equivalents if helpful

## Output format

### 1. Candidate Approaches

For each approach, provide:

#### Approach N: [short name]
- Core idea: one-sentence summary
- Main data structures / techniques:
- Time complexity:
- Space complexity:
- Best when:
- Limitations / risks:
- Why it may or may not be the preferred choice here:

### 2. Comparison Summary
Give a concise side-by-side comparison:
- easiest to explain
- easiest to implement
- best asymptotic complexity
- most interview-safe
- easiest to extend if requirements change

### 3. Recommended Approach
State:
- the recommended choice
- why it is the best fit for this problem
- what key invariant or insight makes it work

## Style
- Optimize for interview decision-making
- Explain tradeoffs directly
- Keep the output structured and easy to scan
