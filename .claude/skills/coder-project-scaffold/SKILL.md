---
name: coder-project-scaffold
description: Break down a larger coding interview problem or small project into modules, files, interfaces, dependencies, and an implementation order before writing full code. Use when the task is too large for a single function or requires multiple components, multiple files, or system-level structure.
effort: high
---

# coder-project-scaffold

Use this skill when the problem is too large, too open-ended, or too system-oriented to solve as a single function.

This skill is the **project-mode entry point** for the C.O.D.E.R. workflow.

It should be used for:
- larger coding interview questions
- system-flavored coding problems
- multi-module or multi-file tasks
- small project scaffolding
- cases where writing everything in one response would be messy or fragile

It should **not** be used for:
- standard single-function algorithm questions
- small isolated bug fixes
- straightforward coding tasks that fit naturally in one file

## Goals
- Clarify the overall project or system goal at a high level
- Break the problem into modules or components
- Propose a clean file structure
- Define responsibilities for each file/module
- Define module interfaces and data flow
- Suggest an implementation order
- Keep the design practical, minimal, and interview-friendly
- Avoid jumping straight into full implementation

## Rules
- Do not write the full project code immediately
- Do not overengineer the architecture
- Prefer the smallest structure that cleanly solves the problem
- Keep the decomposition implementation-oriented, not academic
- If the task is ambiguous, state the assumptions clearly
- If this is an interview-style task, optimize for clarity and explainability over production-grade complexity
- If this is a project-style task, keep the structure runnable and easy to extend
- If the user explicitly wants files created later, this skill should prepare the file plan first, not skip directly to writing everything
- Treat this as the bridge between high-level problem understanding and file-by-file implementation

## Language Handling
- Default language: Python
- If the user specifies a language (e.g., C++, Java), follow that language strictly when proposing file structure, interfaces, and coding conventions
- If a language has been specified earlier in the conversation, continue using it
- Analysis should remain mostly language-neutral, but file layout and interface suggestions should reflect the chosen language where relevant

### Language-Specific Conventions

#### Python
- Prefer a small, clean module structure
- Use simple files and function/class boundaries
- Avoid unnecessary package complexity unless the project actually needs it

#### C++
- Prefer header/source organization only if it materially improves clarity
- For interview-style tasks, avoid excessive file splitting
- Keep classes and interfaces straightforward

#### Java
- Prefer class-oriented structure
- Keep packages simple unless the project actually needs them
- Follow standard `class Solution` style for interview tasks, but use multiple classes/files for project-like tasks when necessary

## Output format

### 1. Problem Framing
Briefly state:
- the overall goal
- the likely scope
- whether this should be treated as:
  - interview-style large coding problem
  - small project
  - system-flavored implementation task

### 2. Assumptions and Simplifications
List:
- assumptions needed to keep the scope manageable
- explicit non-goals
- any simplified constraints or toy versions if needed

### 3. Module Breakdown
List the main modules/components.

For each module, provide:
- name
- responsibility
- key inputs
- key outputs
- dependencies on other modules

### 4. File Structure
Propose a practical file tree.

Example format:

project_name/
  main.py
  recall.py
  rank.py
  feature.py
  models.py

or language-appropriate equivalents.

### 5. Interface Sketch
For each important file or module, describe:
- main classes / functions
- input/output contracts
- how it connects to the rest of the system

Do not fully implement them yet.

### 6. Data / Control Flow
Describe the end-to-end execution flow:
- what starts the process
- which module calls which
- where data is transformed
- where the final result is produced

### 7. Implementation Order
Provide the recommended development order.

The order should usually go from:
1. core abstractions / data models
2. isolated logic modules
3. orchestration / integration layer
4. tests / validation

### 8. Risks and Design Watchouts
List the most likely failure points, such as:
- module boundaries being unclear
- interface mismatch
- over-splitting files
- under-specifying data contracts
- trying to implement everything at once

### 9. Next Step Recommendation
End with a concrete recommendation for what to do next.

Examples:
- “Next, implement `recall.py` first.”
- “Next, generate skeletons for all files.”
- “Next, define the shared data model before module implementation.”

## Style
- Be structured, practical, and concise
- Optimize for controllable execution
- Prefer file-by-file progress over giant monolithic outputs
- Make the result easy to hand off to:
  - `coder-skeleton`
  - `coder-implement`
  - `coder-evaluate-test`
  - `coder-refine-debug`

## Workflow Integration
This skill is intended to sit before implementation-heavy skills.

Typical project-mode workflow:

1. `coder-clarify` (optional, for the overall problem)
2. `coder-project-scaffold`
3. file-by-file `coder-skeleton` or `coder-implement`
4. `coder-evaluate-test`
5. `coder-refine-debug`

For large tasks, do **not** restart the full C.O.D.E.R. flow for every submodule.
Instead:
- use this skill once for the overall structure
- then implement one file/module at a time
- only use local re-analysis when a submodule is genuinely complex or ambiguous
