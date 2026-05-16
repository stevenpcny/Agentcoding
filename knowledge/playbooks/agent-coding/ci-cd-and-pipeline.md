# CI/CD and Build Pipeline Integration

## Core rule
The build, test, and deployment pipeline is the single source of truth for verification. Local development should closely mirror CI.

## Industry Alignment
Follows modern DevOps and CI/CD best practices (Trunk-based development, fast feedback loops).

## When to use
- Setting up or modifying CI configuration
- Adding quality gates (lint, test, security scan)
- Debugging pipeline failures

## Decision rules
- Define all quality gates in pipeline configuration
- Keep pipelines fast enough for every commit
- Make failures actionable with clear logs
- Ensure local commands can reproduce CI results

## Verification checklist
- Can an agent run equivalent CI locally?
- Are critical checks enforced in the pipeline?
- Is the configuration version-controlled and reviewable?

## Anti-patterns
- Important checks only run locally
- Slow or flaky pipelines left unfixed
- Different environments between local and CI

## Example prompts
- "Audit and improve the current CI configuration."
- "Design a minimal effective pipeline for this project."