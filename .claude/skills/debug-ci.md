# Skill: Debug CI

Use this skill when GitHub Actions or CI checks fail.

## Steps

1. Identify the failing workflow and job.
2. Read the error message carefully.
3. Determine whether the failure is caused by:
    - dependency installation;
    - linting;
    - type checking;
    - tests;
    - build;
    - Docker;
    - Terraform;
    - deployment configuration.
4. Propose the smallest fix.
5. Update documentation if commands or workflows change.

## Rules

- Do not mask errors by disabling checks.
- Do not skip tests unless explicitly justified.
- Prefer fixing root causes.
- Keep CI readable.

## Output

Summarize:

- Root cause.
- Fix.
- Validation command.
- Preventive improvement.