# JobTrack AI

Job application tracker with AI features (CV-to-job matching, cover letter drafts,
interview prep). Learning project: built from scratch to production by one developer.

## About me
- 5+ years React Native, comfortable with React and Next.js
- Currently LEARNING Go and Flutter. Treat me as a beginner in those two.

## Repo structure (monorepo)
- `apps/api`    — Go backend (REST API)
- `apps/web`    — Next.js web dashboard
- `apps/mobile` — Flutter mobile app
- `infra/`      — Docker, deployment config
- `docs/`       — schema, architecture notes, decisions
- `openapi.yaml` — API contract, single source of truth for all apps

## Stack
- API: Go, chi, PostgreSQL, sqlc, goose migrations, JWT auth
- Web: Next.js (App Router), TypeScript, TanStack Query
- Mobile: Flutter, Riverpod, go_router
- AI: LLM API, pgvector for embeddings (RAG)
- CI/CD: GitHub Actions; web on Vercel; API in Docker

## How to work with me
- In `apps/api` and `apps/mobile`: explain the approach and WHY before writing code.
  Prefer idiomatic Go / Flutter and point out when I write non-idiomatic code.
- When I write code myself and ask for review, review it; don't rewrite it unless I ask.
- Change only one app per task unless I explicitly ask for a cross-app change.
- API changes: update `openapi.yaml` first, then the code.
- Every new feature needs tests.
- Keep changes small and easy to review. Use conventional commits (feat:, fix:, chore:).
- Never commit secrets. Use `.env` files (gitignored) and `.env.example`.

## Commands
<!-- Fill these in as each app is set up -->
- API:    `cd apps/api && go test ./...`
- Web:    `cd apps/web && npm run dev`
- Mobile: `cd apps/mobile && flutter run`