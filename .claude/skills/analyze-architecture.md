# Skill: Analyze Architecture

Use this skill when evaluating or changing project architecture.

## Steps

1. Read README.md, ROADMAP.md, DECISIONS.md, and relevant CLAUDE.md files.
2. Identify current architecture boundaries.
3. Check whether the proposed change is needed now.
4. Compare simple and advanced options.
5. Recommend the simplest option that satisfies current needs.
6. Record meaningful decisions in DECISIONS.md.

## Rules

- Avoid premature abstraction.
- Prefer incremental architecture.
- Consider testing, deployment, and maintainability.
- Consider AWS cost and operational complexity.

## Output

Use this structure:

```text
## Context

## Current State

## Options

## Recommendation

## Trade-offs

## Decision Record Needed
```