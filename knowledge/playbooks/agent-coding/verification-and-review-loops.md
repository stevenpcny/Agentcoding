# Verification and Review Loops

## Core rule
Reliable agent output requires separating diagnosis, implementation, verification, and review into distinct phases rather than blending them.

## Industry Alignment
Follows established practices from test-driven development, code review culture (Google, Microsoft), and agent reliability research (Anthropic, OpenAI).

## When to use
- Bug fixing
- Refactoring
- Feature implementation with side effects
- Any change with non-trivial risk

## Decision rules
- Diagnose root cause before editing
- Define verification criteria before implementation
- Use risk-based review depth
- Separate "done" from "verified"
- Always have a rollback path for risky changes

## Verification checklist
- Was the problem understood before changes?
- Is there an automated, repeatable verification step?
- Was a review performed after implementation?
- Are regression risks covered?
- Is rollback feasible if needed?

## Anti-patterns
- Editing before understanding the failure
- Declaring success without evidence
- Skipping review on complex changes
- No clear verification command

## Example prompts
- "Diagnose → Implement → Verify → Review this task."
- "Define the verification method before starting implementation."