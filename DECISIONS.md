# Technical Decisions

### Consequences

- One repository contains the whole system.
- Shared types can be extracted into packages later.
- CI can validate the whole project from one place.
- Changes across frontend, backend, and infrastructure are easier to coordinate.

---

## Decision 003 — Use Documentation-First AI Workflow

Date: 2026-05-19

### Context

The project will be continued with AI-assisted development tools such as Claude Code or Codex in WebStorm.

AI tools need clear project context, rules, and constraints to make safe and consistent changes.

### Decision

Add root and app-specific CLAUDE.md files, reusable AI skills, ROADMAP.md, PROGRESS.md, and DECISIONS.md from the beginning.

### Consequences

- Future AI sessions can understand the project faster.
- Changes should stay aligned with the roadmap.
- Documentation becomes part of the development workflow.

---

## Decision 004 — Start with Production-Like Simplicity

Date: 2026-05-19

### Context

The project should be realistic, but not overengineered.

### Decision

Start with a simple full-stack architecture and improve it step by step.

Initial stack:

- React + Vite frontend.
- NestJS backend.
- PostgreSQL database.
- Docker for local development.
- Terraform for AWS infrastructure.
- GitHub Actions for CI/CD.

### Consequences

- The first working version can be delivered quickly.
- More advanced topics can be introduced later.
- Complexity remains controlled.