# Skill: Terraform Change

Use this skill when changing infrastructure code.

## Steps

1. Read `infra/terraform/CLAUDE.md`.
2. Inspect existing Terraform structure.
3. Identify the target environment.
4. Explain what resources will be created, changed, or destroyed.
5. Prefer small changes.
6. Run or recommend:
    - `terraform fmt`
    - `terraform validate`
    - `terraform plan`
7. Update documentation if infrastructure behavior changes.

## Rules

- Never hardcode secrets.
- Avoid broad IAM permissions.
- Mention possible AWS costs.
- Mention cleanup/destroy steps.
- Keep modules simple.
- Do not add production infrastructure before dev is stable.

## Output

Summarize:

- Infrastructure change.
- Expected AWS resources.
- Commands to run.
- Cost/security notes.
- Rollback or destroy notes.