# Testing Strategy

## Core rule
Every meaningful change must have a clear, fast, and deterministic verification method defined before implementation.

## Industry Alignment
Follows the Testing Pyramid and modern practices from Google, Thoughtworks, and high-velocity engineering teams.

## When to use
- Feature development
- Bug fixes
- Refactoring
- Behavioral changes

## Decision rules
- Define verification before coding
- Prefer fast unit tests over slow E2E
- Test observable behavior, not implementation details
- Make tests runnable with one command
- Add tests that would catch likely regressions

## Verification checklist
- Is there automated verification?
- Does it cover key paths and edge cases?
- Can it run locally and in CI?
- Is it deterministic?

## Anti-patterns
- Code first, tests later
- Only manual testing
- Slow or flaky tests
- Testing private methods

## Example prompts
- "Design the minimal test for this change."
- "Convert this task into: implement + test + verification command."