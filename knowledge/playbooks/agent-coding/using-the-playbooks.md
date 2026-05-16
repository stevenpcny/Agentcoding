# Using the Agent Coding Playbooks

## Purpose
This guide explains how Codex, Claude, Hermes, and other agents should use the agent-coding playbooks in real development work.

## Recommended Workflow

### 1. Task Intake
- Always start with **Goal and Task Framing**
- Define Goal, Constraints, and Completion Criteria

### 2. Planning Phase
- Load relevant playbooks based on task type:
  - Complex changes → Large-Scale Refactoring + Technical Debt
  - Security-sensitive → Security Review
  - Performance-related → Performance Optimization

### 3. Execution Phase
- Apply **Verification and Review Loops**
- Use **Self-Correction** when repeated errors occur
- Follow **Testing Strategy** and **Code Quality**

### 4. Context Management
- Use **Token and Context Engineering** to stay efficient
- Externalize stable rules into AGENTS.md / CLAUDE.md

### 5. Completion
- Verify against original completion criteria
- Update documentation if needed

## When to Load Multiple Playbooks
- Feature development: Goal Framing + Testing + Code Quality
- Debugging: Verification Loops + Self-Correction
- Large refactors: Large-Scale Refactoring + Technical Debt

## Best Practice
Treat these playbooks as durable engineering policy. Reference them explicitly when needed rather than re-explaining rules in every session.