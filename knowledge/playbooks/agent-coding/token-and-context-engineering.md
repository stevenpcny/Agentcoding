# Token and Context Engineering

## Core rule
Token usage is primarily a context design problem. The goal is to give the agent the minimum necessary high-signal information while preserving output quality.

## When to use
- Long-running or multi-file tasks
- Large repositories
- Repeated sessions on the same project
- When hitting context limits frequently

## When not to use
- Small, one-shot tasks
- Pure exploration with no reuse

## Decision rules
- Externalize all stable knowledge (project rules, architecture, conventions) into repo files instead of prompts
- Use structured, compact formats (markdown, JSON, checklists) instead of prose
- Prefer retrieval (graph, search, skills) over dumping entire files
- Keep session context focused on the current phase only
- Reuse proven prompt templates instead of writing new ones each time

## High-Signal Patterns

### 1. Context Externalization
- Put durable rules in `AGENTS.md` / `CLAUDE.md`
- Store architecture decisions in `ARCHITECTURE.md`
- Move repeated instructions into skills or reusable prompts

### 2. Structured Input
- Use checklists and bullet points instead of paragraphs
- Use code blocks with clear labels
- Prefer `Goal + Constraints + Verification` format

### 3. Phased Context Loading
- Load only the context needed for the current phase
- Use retrieval tools before expanding context
- Summarize previous phase results instead of re-pasting

### 4. Token-Efficient Prompt Template
```
Goal: [one sentence]
Constraints: [bullet list]
Relevant Context: [minimal files or summaries]
Verification: [how to confirm success]
```

## Verification checklist
- Is stable context stored outside the current prompt?
- Can the input be reduced by 30%+ without losing critical information?
- Is the agent re-reading the same large files across turns?
- Does the prompt follow a consistent high-signal structure?

## Anti-patterns
- Dumping entire files or long chat history every turn
- Repeating project rules in every prompt
- Using vague instructions that require the model to guess
- Ignoring retrieval tools when available

## Evidence notes
- Multiple notes on context management and error reduction through better structure

## Example prompts
- "Summarize only the parts of this file relevant to the current task."
- "Load minimal context and solve this using the token-efficient template above."