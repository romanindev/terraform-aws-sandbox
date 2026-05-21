# Architecture Context

## High-Level Architecture

The project is planned as a simple full-stack application with production-like delivery practices.

```txt
React Web App -> NestJS API -> PostgreSQL
      │              │
      │              └── Docker / ECS later
      │
      └── S3 + CloudFront later
```

## Main Boundary Decisions

- `apps/web` owns the browser UI.
- `apps/api` owns API behavior and persistence access.
- `packages/shared` may contain shared types only when duplication becomes real.
- `infra/terraform` owns AWS infrastructure.
- `.claude` owns AI development context and reusable skills.

## Architecture Principles

- Start simple.
- Make boundaries clear.
- Avoid premature abstraction.
- Make changes observable through tests and documentation.
- Keep infrastructure changes incremental.
