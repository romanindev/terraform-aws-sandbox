# Skill: Review PR

Use this skill when reviewing a branch, diff, or pull request.

## Review Focus

- Correctness.
- Simplicity.
- Maintainability.
- Testing coverage.
- Documentation updates.
- Security issues.
- Infrastructure risk.
- Possible AWS cost impact.

## Steps

1. Understand the goal of the change.
2. Inspect changed files.
3. Check if the change matches ROADMAP.md and PROGRESS.md.
4. Identify bugs, risks, missing tests, or missing docs.
5. Suggest concrete improvements.

## Rules

- Be specific.
- Avoid vague comments.
- Prefer actionable feedback.
- Distinguish blockers from suggestions.

## Output Format

Use this structure:

```text
## Summary

## Blockers

## Suggestions

## Tests

## Documentation

## Risk Notes
```
