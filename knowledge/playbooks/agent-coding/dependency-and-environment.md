# Dependency and Environment Management

## Core rule
Dependencies and environment setup must be explicit, reproducible, and minimal. The agent should be able to recreate the development and runtime environment from the repository alone.

## Industry Alignment
Follows modern practices from reproducible builds, infrastructure as code, and dependency management standards (e.g., lockfiles, semantic versioning discipline).

## When to use
- Adding or updating third-party libraries
- New project setup or environment onboarding
- Debugging environment-specific issues

## Decision rules
- Pin exact versions using lockfiles
- Document environment requirements in a single discoverable file
- Prefer declarative configuration
- Separate dev and prod dependencies clearly
- Justify every new dependency

## Verification checklist
- Can a fresh machine reproduce the environment?
- Are all dependencies version-pinned?
- Is there a documented update process?
- Would environment drift be detectable?

## Anti-patterns
- Global installations or "works on my machine"
- Mixing dev/prod dependencies
- Adding dependencies without lockfiles
- Undocumented manual setup steps

## Example prompts
- "Audit dependencies for reproducibility."
- "Add this library while maintaining environment reproducibility."