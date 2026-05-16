# Agent Coding Playbooks Usage Guide

This guide explains how to effectively use the agent-coding knowledge base with Codex, Claude, Hermes, and other AI coding agents.

## 1. Core Philosophy

All complex development work should follow a **goal-driven, verification-first** approach. The playbooks exist to reduce ambiguity, improve reliability, and minimize token waste.

## 2. Recommended Daily Workflow

### Step 1: Task Framing (Always Start Here)
- Read: `goal-and-task-framing.md`
- Clearly define: Goal, Constraints, Completion Criteria

### Step 2: Select Relevant Playbooks
| Task Type                    | Recommended Playbooks                              |
|-----------------------------|----------------------------------------------------|
| New Feature                 | Goal Framing + Testing + Code Quality              |
| Bug Fixing                  | Verification Loops + Self-Correction               |
| Refactoring                 | Code Quality + Large-Scale Refactoring             |
| Security-sensitive Work     | Security Review + Testing                          |
| Performance Work            | Performance Optimization + Observability           |
| Long-running Autonomous     | Token Engineering + Self-Correction                |

### Step 3: Execution
- Use **Verification and Review Loops**
- Apply **Self-Correction** when errors repeat
- Maintain **Token Efficiency** throughout

### Step 4: Completion & Documentation
- Verify against original completion criteria
- Update documentation using `documentation-generation.md`

## 3. Token Efficiency Best Practices

- Externalize stable rules into `AGENTS.md` / `CLAUDE.md`
- Use structured templates instead of long prose
- Load only phase-relevant context
- Prefer retrieval over dumping entire files

## 4. Global Configuration

The following files are set up for global loading:
- `~/.hermes/AGENTS.md`
- `~/.claude/CLAUDE.md`
- `~/.codex/AGENTS.md`

These provide baseline rules across all projects.

## 5. Project-Level Customization

Every project can extend the global rules by adding:
- `AGENTS.md`
- `CLAUDE.md`
- `project-agents.md`

These files should only contain **project-specific** rules.

## 6. Quick Reference

**Most Used Playbooks** (in order of frequency):
1. Goal and Task Framing
2. Verification and Review Loops
3. Testing Strategy
4. Code Quality and Safe Refactoring
5. Self-Correction and Recovery
6. Token and Context Engineering

## 7. Maintenance

- Review and update playbooks quarterly
- Add new patterns only when they have been validated across multiple projects
- Keep language concise and actionable

---

**Last Updated**: 2026-05-16
**Maintained by**: Steven