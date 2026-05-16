# Code Quality and Safe Refactoring

## Core rule
All changes must prioritize readability, simplicity, and explicit intent. Refactoring should only occur when it improves maintainability or verifiability, always with safety mechanisms.

## Industry Alignment
Based on Clean Code (Robert C. Martin), Refactoring (Martin Fowler), and modern practices from senior engineering teams.

## When to use
- Non-trivial code changes
- Duplicate or overly complex code
- Preparing code for long-term maintenance

## Decision rules
- Apply "Simplicity First"
- One responsibility per function
- Make implicit assumptions explicit
- Refactor one dimension at a time
- Never refactor without tests or verification

## Verification checklist
- Does the code read clearly to a future developer?
- Are changes minimal and focused?
- Is behavior preserved and verified?
- Does it follow project conventions?

## Anti-patterns
- Clever code that reduces readability
- Large, multi-concern refactors
- Changes without verification
- Ignoring existing style

## Example prompts
- "Refactor for readability while keeping behavior identical."
- "Review this diff for quality issues using clean code principles."