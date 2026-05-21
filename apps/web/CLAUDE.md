# CLAUDE.md — Web App

This file provides context for the frontend application.

## App Purpose

The web app will be a React + Vite frontend for the Todo application.

It should provide a simple, clean, accessible interface for managing todos.

## Planned Stack

- React
- TypeScript
- Vite
- React Router
- TanStack Query
- Vitest
- Testing Library
- Playwright

## Frontend Rules

- Keep components small and readable.
- Prefer feature-based structure.
- Use TanStack Query for server state.
- Do not duplicate server state unnecessarily in local state.
- Keep API access isolated in a client/module.
- Add tests for important UI behavior.
- Keep accessibility in mind from the start.
- Prefer simple styling before introducing a design system.

## Planned Structure

```txt
apps/web/
├── src/
│   ├── app/
│   ├── features/
│   │   └── todos/
│   ├── shared/
│   │   ├── api/
│   │   ├── components/
│   │   └── utils/
│   └── main.tsx
├── tests/
└── package.json
```

## Expected First Features

- Todo list page.
- Create todo form.
- Complete/uncomplete todo action.
- Delete todo action.
- Loading and error states.
- Basic responsive layout.

## Do Not Do Yet

- Do not add complex design systems at the start.
- Do not introduce global state libraries unless needed.
- Do not build advanced task management features.
- Do not add authentication in the first phase.
