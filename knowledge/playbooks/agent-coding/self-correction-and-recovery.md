# Self-Correction and Recovery Loops

## Core rule
When the same error class occurs twice, stop blind retries. Research multiple solutions, compare them, and implement only after evaluation.

## Industry Alignment
Reflects debugging best practices and agent reliability patterns from production agent systems.

## When to use
- Repeated compilation/runtime/integration errors
- Long autonomous sessions
- High risk of getting stuck in local loops

## Decision rules
- Treat repeated errors as a mandatory strategy switch
- Research from high-quality sources first
- Generate and compare at least 3 options
- Log error class, attempts, and decision
- Prefer minimal verifiable fixes with rollback

## Verification checklist
- Did the same error occur ≥2 times?
- Were multiple solutions evaluated?
- Is verification defined after the fix?
- Was the decision recorded?

## Anti-patterns
- Repeatedly running the same failing command
- Accepting the first suggested fix
- Hiding error history from the agent

## Example prompts
- "Same error twice. Research 3-5 solutions, compare, then implement."
- "Add self-correction rules to AGENTS.md."