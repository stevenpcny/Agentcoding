# Technical Debt Management

## Core rule
Technical debt must be made visible, quantified, and intentionally managed rather than allowed to accumulate invisibly. Agents should regularly identify, prioritize, and repay debt as part of normal development work.

## When to use
- After completing features or refactors that introduced shortcuts
- During codebase audits or onboarding to a new project
- When velocity is slowing due to accumulated complexity

## When not to use
- Early-stage prototypes where speed is intentionally prioritized
- When the team has not yet established baseline quality standards

## Decision rules
- Make debt explicit by documenting it (in code comments, issues, or a debt register)
- Categorize debt (code quality, architecture, testing, documentation, dependencies)
- Repay debt opportunistically during related work rather than in dedicated "debt sprints"
- Track the cost of debt (time lost to complexity) to justify repayment
- Avoid creating new debt without a conscious decision and plan to repay it

## Verification checklist
- Is the debt visible to future agents (not just in the original developer's mind)?
- Has the debt been prioritized against current business goals?
- Is there a measurable improvement after repayment?
- Was new debt introduced only after evaluating the trade-off?

## Anti-patterns
- Silently accumulating workarounds and TODOs without tracking
- Treating all debt as equal (ignoring high-interest debt)
- Using "we'll fix it later" without a concrete plan
- Refusing to take on any debt even when it blocks delivery

## Evidence notes
- `knowledge/notes/2026-05-11-2053814471793971582-mindos-lisa.md`

## Example prompts
- Read this playbook and audit the current module for technical debt.
- Apply this playbook: identify the highest-interest technical debt in this area and propose a repayment plan.
- Add technical debt tracking rules to the project AGENTS.md.