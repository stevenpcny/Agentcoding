# Repo Instructions and Project Memory

## Core rule
Project-level instruction files should store durable repository context, not act like disposable prompt files.

## Industry Alignment
Aligns with modern practices of maintaining living documentation and agent-friendly project instructions.

## When to use
- Designing AGENTS.md, CLAUDE.md, or similar files
- Projects where agents repeatedly re-learn structure
- Establishing stable engineering conventions

## Decision rules
- Put durable context in repo docs, not in every prompt
- Keep project maps, conventions, and verification habits in inspectable files
- Store reusable procedures in skills when possible
- Keep system-level rules separate from project-specific rules

## Verification checklist
- Does this belong in the repo long-term?
- Will this still matter in future sessions?
- Does it reduce re-orientation cost for agents?
- Is it written as durable context rather than temporary instructions?

## Anti-patterns
- Treating AGENTS.md as a generic prompt dump
- Putting temporary task state into long-lived files
- Mixing engineering rules with hype or business observations

## Example prompts
- "Decide what belongs in AGENTS.md vs a skill vs a task plan."
- "Rewrite these project instructions into durable repo context."