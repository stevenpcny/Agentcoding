# Agent Prompt Engineering

## Core rule
Effective agent performance depends on clear, structured, and context-aware instructions rather than relying on the model to guess intent.

## Industry Alignment
Based on Anthropic’s and OpenAI’s prompt engineering guidelines and production agent usage patterns.

## When to use
- Designing AGENTS.md or CLAUDE.md
- Creating reusable skills or prompt templates
- Troubleshooting poor agent output

## Decision rules
- Start with explicit goal and success criteria
- Separate context, instructions, constraints, and output format
- Include relevant examples when helpful
- Externalize stable rules instead of repeating them
- Use consistent structure across prompts

## Verification checklist
- Is the goal and acceptance criteria unambiguous?
- Would different agents produce consistent results?
- Are constraints explicitly stated?
- Is the prompt structured for easy maintenance?

## Anti-patterns
- Vague instructions like “make it good”
- Repeating the same context every session
- Mixing multiple unrelated tasks in one prompt

## Example prompts
- "Rewrite this request using the structured prompt template."
- "Design a reusable prompt template for this type of task."