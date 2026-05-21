# Terraform AWS Sandbox

A production-like full-stack sandbox project focused on learning Terraform, AWS, Docker, CI/CD, and cloud deployment practices through a simple Todo application.

The goal of this project is not to build a complex product, but to understand the full engineering lifecycle: local development, testing, containerization, infrastructure as code, CI/CD, deployment to AWS, documentation, and AI-assisted development workflows.

## Project Purpose

This project is a learning and practice sandbox for building a small but production-minded full-stack application using modern engineering practices.

The Todo domain is intentionally simple. The main focus is on infrastructure, maintainability, deployment, testing, and developer experience.

## Main Learning Goals

- Build a monorepo with pnpm workspaces.
- Create a NestJS API with PostgreSQL persistence.
- Create a React + Vite frontend.
- Use Docker for local development.
- Cover core behavior with unit, integration, and E2E tests.
- Provision AWS infrastructure with Terraform.
- Deploy frontend and backend services to AWS.
- Configure CI/CD with GitHub Actions.
- Use AI-assisted development workflows with clear project context.
- Practice senior-level engineering decisions and documentation.

## Planned Stack

### Frontend

- React
- TypeScript
- Vite
- React Router
- TanStack Query
- Vitest
- Testing Library
- Playwright

### Backend

- Node.js
- TypeScript
- NestJS
- PostgreSQL
- Prisma
- Vitest or Jest

### Infrastructure

- Docker
- Docker Compose
- Terraform
- AWS
- GitHub Actions
- AWS IAM / OIDC
- S3
- CloudFront
- ECR
- ECS Fargate
- RDS PostgreSQL
- CloudWatch

## Repository Structure

```txt
apps/
  api/              # NestJS backend application
  web/              # React + Vite frontend application

packages/
  shared/           # Shared types and utilities
  config/           # Shared tooling/configuration package

infra/
  terraform/        # Terraform infrastructure code

docker/             # Docker-related support files

.claude/            # AI assistant context and reusable skills
```

## Development Principles

- Prefer simple and clear solutions over unnecessary abstraction.
- Check existing functionality before creating new files or components.
- Keep changes small, reviewable, and well documented.
- Cover important behavior with tests.
- Update documentation when behavior, architecture, commands, or infrastructure changes.
- Treat Terraform changes carefully and explain their cost/security impact.
- Use environment variables for configuration.
- Never commit secrets or local `.env` files.

## Non-goals

- Building a feature-rich task management product.
- Overengineering the Todo domain.
- Introducing Kubernetes in the first phase.
- Deploying real production workloads with user data.
- Building a multi-tenant SaaS product.

## Current Status

Project foundation stage. See [ROADMAP.md](./ROADMAP.md) and [PROGRESS.md](./PROGRESS.md).

## Documentation
- ROADMAP.md - implementation plan by days.
- PROGRESS.md - current progress and completed work.
- DECISIONS.md - architecture and technical decisions.
- CLAUDE.md - project context for AI-assisted development.