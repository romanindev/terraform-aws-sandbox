# Roadmap

- Dockerfile for API.
- Dockerfile for web.
- Docker Compose full-stack setup.
- Healthchecks.
- Local Docker run documentation.

## Day 7 — Terraform Bootstrap

Goal: initialize Terraform safely.

Expected result:

- Terraform directory structure.
- AWS provider configuration.
- Dev environment skeleton.
- Remote state strategy documented.
- Terraform fmt/validate command documented.
- Initial CI plan for Terraform validation.

## Day 8 — Frontend AWS Deployment

Goal: deploy static frontend infrastructure.

Expected result:

- S3 bucket for frontend assets.
- CloudFront distribution.
- Terraform outputs.
- GitHub Actions deployment plan.
- Documentation updates.

## Day 9 — API AWS Infrastructure

Goal: prepare backend deployment infrastructure.

Expected result:

- ECR repository.
- ECS cluster.
- ECS task definition.
- Application Load Balancer.
- CloudWatch logs.
- IAM roles.
- GitHub Actions image build/push plan.

## Day 10 — Database and Secrets

Goal: connect backend to managed AWS persistence.

Expected result:

- RDS PostgreSQL or documented alternative.
- Network/security group configuration.
- Secrets Manager or SSM Parameter Store usage.
- Migration strategy.
- Updated deployment documentation.

## Later Improvements

- Authentication.
- Observability dashboard.
- Cost monitoring.
- Separate staging/prod environments.
- Infrastructure modules refactoring.
- More advanced GitHub Actions workflows.
- Security scanning.
- Performance testing.