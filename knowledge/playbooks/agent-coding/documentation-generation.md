# Documentation Generation and Maintenance

## Core rule
Documentation should be treated as executable context for both humans and agents. It must be updated as part of the development workflow.

## Industry Alignment
Aligns with "Documentation as Code" and modern practices from high-quality open source projects and engineering teams.

## When to use
- New modules, functions, or APIs
- Complex business logic or architectural decisions
- Public interfaces and configuration

## Decision rules
- Document the "why" more than the "how"
- Keep documentation close to the code
- Update docs in the same commit as code changes
- Use examples over abstract descriptions

## Verification checklist
- Can a future agent understand usage without reading implementation?
- Is the documentation accurate after changes?
- Are examples realistic and runnable?

## Anti-patterns
- Writing docs long after code is complete
- Duplicating implementation details
- Leaving outdated documentation

## Example prompts
- "Generate clear documentation for this function."
- "Review the code and produce minimal useful documentation."