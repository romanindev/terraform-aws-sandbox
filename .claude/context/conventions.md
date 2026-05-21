# Project Conventions

## General

- Use TypeScript.
- Prefer explicit naming.
- Keep files focused.
- Avoid large unrelated changes.
- Update docs when behavior or commands change.

## Git

Suggested branch naming:

- `chore/day-0-foundation`
- `feat/day-1-monorepo-skeleton`
- `feat/day-2-api-foundation`
- `infra/day-7-terraform-bootstrap`

Suggested commit style:

- `chore: add repository foundation docs`
- `chore: initialize pnpm workspace`
- `feat(api): add health endpoint`
- `infra(terraform): add dev environment skeleton`

## Documentation

Update `PROGRESS.md` after each logical milestone.

Update `DECISIONS.md` when a meaningful technical decision is made.

Update `README.md` when setup or usage instructions change.

## Testing

Prefer tests that protect important behavior.

Avoid snapshot-heavy tests unless they add clear value.

## Environment Variables

- Use `.env.example` to document required variables.
- Do not commit `.env`.
- Prefer clear names such as `DATABASE_URL`, `API_PORT`, `WEB_API_BASE_URL`.