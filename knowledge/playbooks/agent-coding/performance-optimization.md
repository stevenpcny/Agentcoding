# Performance Optimization and Observability

## Core rule
Performance work must be measurement-driven. Never optimize without establishing a baseline and clear success criteria. Observability must be added together with performance-sensitive changes.

## Industry Alignment
Follows Google SRE principles, data-driven optimization practices, and modern observability standards (OpenTelemetry, etc.).

## When to use
- Identified bottlenecks with measurable impact
- High-traffic paths or resource-heavy operations
- Latency, memory, or cost-sensitive features

## Decision rules
- Measure first (profiling, benchmarks, tracing)
- Define specific, quantifiable goals
- Add observability at the same time as optimization
- Prefer algorithmic improvements over micro-optimizations
- Document trade-offs made

## Verification checklist
- Is there a reproducible benchmark?
- Does the change include monitoring?
- Is the improvement justified by data?
- Has it been tested under realistic load?

## Anti-patterns
- Optimizing without measurement
- Sacrificing readability for marginal gains
- Adding complexity without corresponding observability

## Example prompts
- "Profile first, then propose a data-backed improvement."
- "Add observability while optimizing this function."