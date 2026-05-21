# CLAUDE.md — Terraform AWS Sandbox

This file provides project context and rules for AI-assisted development tools such as Claude Code, Codex, or other coding agents.

## Project Summary

Terraform AWS Sandbox is a production-like full-stack learning project focused on Terraform, AWS, Docker, CI/CD, testing, and cloud deployment practices.

The application domain is intentionally simple: a Todo app.

The main goal is to practice the full engineering lifecycle, not to build a complex product.

## Repository Type

This is a pnpm workspace monorepo.

Planned structure:

```txt
apps/api       # NestJS API
apps/web       # React + Vite frontend
packages/shared
packages/config
infra/terraform
```

## Main Stack
- TypeScript
- Node.js
- NestJS
- React
- Vite
- PostgreSQL
- Prisma
- Docker
- Terraform
- AWS
- GitHub Actions
- Vitest / Jest
- Playwright

## Development Rules
1. Check existing files and functionality before creating new files. 
2. Keep changes small and focused. 
3. Prefer simple, readable solutions. 
4. Avoid unnecessary abstractions. 
5. Follow SOLID principles where they make sense. 
6. Do not implement business logic before the required project foundation exists. 
7. Update documentation when commands, architecture, infrastructure, or behavior changes. 
8. Add or update tests for meaningful behavior changes. 
9. Never commit secrets, credentials, or local .env files. 
10. Treat Terraform and AWS changes as high-impact changes.

## Before Making Changes

Before making important changes:

1. Inspect the existing structure.
2. Check README.md, ROADMAP.md, PROGRESS.md, and DECISIONS.md. 
3. Identify the current roadmap day. 
4. Propose a short implementation plan. 
5. Prefer the incremental changes over large rewrites. 

## Documentation Expectations

Documentation is part of the implementation.

Update documentation when:

- a new command is added;
- setup steps change;
- architecture changes;
- infrastructure changes;
- environment variables are added or changed;
- testing workflow changes;
- deployment workflow changes.

Important documentation files:

- README.md — project overview and setup.
- ROADMAP.md — implementation plan.
- PROGRESS.md — current progress.
- DECISIONS.md — technical decisions.
- CLAUDE.md — AI assistant rules and context.

## Testing Expectations

Use the right level of testing:

- Unit tests for pure logic and services.
- Integration tests for API behavior and database interaction.
- Component tests for important UI behavior.
- E2E tests for critical user flows.
- Terraform validation for infrastructure changes.

Do not add tests only for the sake of coverage. Tests should protect important behavior.

## Terraform Rules

For Terraform changes:

1. Prefer small infrastructure increments. 
2. Run `terraform fmt`.
3. Run `terraform validate` when possible. 
4. Explain expected AWS resources. 
5. Mention possible costs. 
6. Avoid broad IAM permissions. 
7. Never hardcode secrets. 
8. Prefer remote state for shared workflows. 
9. Document how to apply and destroy resources safely.

## GitHub Actions Rules

For CI/CD changes:

1. Keep workflows readable.
2. Separate validation and deployment where possible. 
3. Avoid long-lived AWS credentials when OIDC can be used. 
4. Do not deploy automatically before the deployment strategy is documented. 
5. Add comments for non-obvious workflow steps.

## Coding Style

General:

- TypeScript-first.
- Prefer explicit types at boundaries.
- Avoid `any` unless justified.
- Keep functions small and focused.
- Use meaningful names.
- Avoid hidden side effects.
- Prefer the composition over inheritance.

Backend:

- Keep NestJS modules focused.
- Use DTOs for request validation.
- Keep business logic in services.
- Avoid putting domain logic directly in controllers.
- Keep database access isolated.

Frontend:

- Keep components small and focused.
- Prefer feature-based organization.
- Use TanStack Query for server state.
- Avoid duplicating API state in local component state.
- Keep accessibility in mind.

## Current Phase

Check PROGRESS.md before starting work.
