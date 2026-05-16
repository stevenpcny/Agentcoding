# Large-Scale Refactoring and Codebase Evolution

## Core rule
Large-scale refactoring must be treated as a planned engineering project with clear phases, safety checkpoints, and rollback strategies rather than a single massive change.

## When to use
- Systemic changes across many files (e.g., API migration, framework upgrade, architecture shift)
- Removing widespread duplication or legacy patterns
- Modernizing large portions of the codebase

## When not to use
- Small localized improvements
- Changes that can be done incrementally without coordination

## Decision rules
- Break the refactoring into small, independently verifiable steps
- Establish a "strangler fig" or incremental migration pattern when possible
- Define clear rollback criteria and automated tests before starting
- Communicate the plan and progress using durable artifacts (issues, plans, or project docs)
- Prioritize changes that deliver value early rather than big-bang delivery

## Verification checklist
- Is there a phased plan with measurable checkpoints?
- Are automated tests and verification steps defined for each phase?
- Can the system be partially rolled back if a phase fails?
- Is the refactoring plan documented and reviewable by other agents?

## Anti-patterns
- Attempting to refactor everything in one pass
- Changing too many things at once without intermediate verification
- Starting large refactors without a clear end state or rollback plan
- Ignoring the cost of merge conflicts during long-running refactors

## Evidence notes
- `knowledge/notes/2026-05-11-2053814471793971582-mindos-lisa.md`

## Example prompts
- Read this playbook and break the requested large change into safe, verifiable phases.
- Apply this playbook: design an incremental migration plan for replacing this legacy module.
- Generate a refactoring plan document suitable for multi-session agent execution.