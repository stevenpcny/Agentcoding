# Goal and Task Framing

## Core rule
Complex work must begin with an explicit goal, clear scope boundaries, and verifiable completion criteria. The agent should never start implementation without these three elements defined.

## When to use
- Any multi-step coding task
- Tasks that span more than one session
- Work involving multiple files, systems, or agents
- Situations with high risk of scope creep

## When not to use
- Trivial single-file changes with obvious intent
- Pure information lookup tasks

## Decision rules
- Define the goal in a single, unambiguous sentence
- Explicitly list what is out of scope
- Define concrete completion criteria before any code is written
- Break work into phases only when each phase has its own verifiable exit condition
- Prefer the smallest verifiable loop that can deliver value

## Verification checklist
- Is the goal stated in one clear sentence?
- Are scope boundaries explicitly documented?
- Is there at least one concrete, measurable completion condition?
- Can success be verified with a command, test, or artifact?
- Has the agent confirmed understanding of constraints?

## Anti-patterns
- Starting implementation with only a vague request ("improve this")
- Mixing ideation, planning, and coding in one step
- Allowing the agent to invent additional requirements mid-task
- Proceeding without defined success criteria

## Evidence notes
- Multiple notes on goal-driven workflows and error reduction through clear framing

## Example prompts
- "Read this playbook and reframe my request into: Goal, Constraints, Completion Criteria, and Phases."
- "Apply this playbook and propose the smallest verifiable execution loop for this task."