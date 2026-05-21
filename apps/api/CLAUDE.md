# CLAUDE.md — API App

This file provides context for the backend application.

## App Purpose

The API app will be a NestJS backend for the Todo application.

It should expose a clean REST API, persist data in PostgreSQL, and be suitable for Docker and AWS deployment later.

## Planned Stack

- Node.js
- TypeScript
- NestJS
- PostgreSQL
- Prisma
- ConfigModule
- Unit and integration tests

## Backend Rules

- Keep controllers thin.
- Put business logic in services.
- Use DTOs for validation.
- Use clear error handling.
- Avoid leaking database implementation details to controllers.
- Keep modules focused by domain.
- Prefer explicit boundaries.
- Add tests for service behavior and API behavior.

## Planned Structure

```txt
apps/api/
├── src/
│   ├── app.module.ts
│   ├── main.ts
│   ├── config/
│   ├── health/
│   ├── todos/
│   └── prisma/
├── test/
└── package.json
```

## Expected First Features
- Health endpoint.
- Todo CRUD.
- PostgreSQL persistence.
- Input validation.
- Error handling.
- Tests.

## Do Not Do Yet

- Do not add authentication in the first phase.
- Do not introduce microservices.
- Do not overcomplicate the Todo domain.
- Do not add queues or event-driven architecture before the basic app works.