# CLAUDE.md — Terraform Infrastructure

This file provides context for Terraform and AWS infrastructure work.

## Infrastructure Purpose

Terraform code in this project is used to learn and provision AWS infrastructure for a small production-like full-stack application.

The infrastructure should be built gradually and safely.

## Planned AWS Services

Initial phases may include:

- S3
- CloudFront
- IAM
- ECR
- ECS Fargate
- RDS PostgreSQL
- CloudWatch
- Secrets Manager or SSM Parameter Store

## Terraform Rules

- Keep changes small and reviewable.
- Run `terraform fmt` after changes.
- Run `terraform validate` when possible.
- Prefer modules only when reuse becomes clear.
- Do not over-abstract early.
- Never hardcode credentials or secrets.
- Explain expected resources and possible costs.
- Prefer least-privilege IAM.
- Document state backend decisions.
- Document destroy/cleanup steps.

## Planned Structure

```txt
infra/terraform/
├── environments/
│   ├── dev/
│   └── prod/
└── modules/
```

## Safety Notes

AWS resources can create real costs.

Before adding or applying Terraform code:

1. Explain what resources will be created. 
2. Explain possible monthly cost impact. 
3. Explain how to destroy resources. 
4. Avoid production-grade expensive services until explicitly planned.

## Do Not Do Yet

- Do not create Kubernetes infrastructure in the first phase.
- Do not introduce multi-account AWS setup at the beginning.
- Do not create production infrastructure before the dev environment works.
- Do not use broad administrator IAM policies without explicit justification.