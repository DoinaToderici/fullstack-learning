# Full-stack learning plan

17 weeks, about 1h30 per day (around 9h per week), working solo with an AI assistant as a teacher.
Target stack: TypeScript everywhere, React 19 + Next.js (front), NestJS + PostgreSQL (back), Docker + GitHub Actions (delivery).

Each phase ends with a small, concrete exercise pushed to this repository, in its `phase-X` folder.
Daily rhythm: 45 min learning (docs, courses) + 45 min practice (coding).

## Current status

- Current phase: **Phase 1 – Modern JavaScript & TypeScript** (week 2)
- Last update: 2026-11-19

## Overview

| Phase | Weeks | Topic | Exercise |
| --- | --- | --- | --- |
| 0 | 1 | Tools: terminal, Git, GitHub, VS Code, AI | This repository |
| 1 | 2–4 | Modern JavaScript & TypeScript | Typed functions to filter and sort a list of listings |
| 2 | 5–8 | React 19 & Next.js | A "practical guides" page in two languages (ro/fr) |
| 3 | 9–10 | Backend basics: HTTP, REST, Node.js | In-memory listings REST API |
| 4 | 11–12 | SQL, PostgreSQL, ORM (Prisma) | Database schema for listings |
| 5 | 13–15 | NestJS, authentication, security | Listings API with user accounts |
| 6 | 16–17 | Testing, Docker, CI/CD, deployment | Mini-app online, tested and deployed |

## Phase 0 – Tools (week 1)

- [x] Install Node (LTS, managed with fnm), Git, VS Code + ESLint, Prettier, Error Lens
- [x] Terminal basics: cd, pwd, ls, mkdir, touch, echo, cat, cp, mv, rm
- [x] Git: init, status, add, commit, log, diff, branches, merge
- [x] GitHub: push, pull, pull requests, Conventional Commits
- [x] AI assistant set up (Claude Code + CLAUDE.md learning rules)
- [ ] Professional GitHub profile (photo, bio, profile README) – postponed

## Phase 1 – Modern JavaScript & TypeScript (weeks 2–4)

- Week 2 – Modern JavaScript: let/const, arrow functions, destructuring, spread, modules (import/export), array methods (map, filter, reduce), optional chaining (`?.`) and `??`.
- Week 3 – Async: promises, async/await, `fetch`, error handling with try/catch. Call a public API and display the result.
- Week 4 – TypeScript: basic types, interfaces and types, unions, simple generics, typing a function and an API response, `tsconfig.json`.

Exercise: define a `Listing` type (title, category, city, price, date) and write typed functions to filter listings by city and sort them by date.

- [ ] I can explain the difference between promises and async/await
- [ ] I can write an interface and a simple generic function
- [ ] Exercise pushed to GitHub

## Phase 2 – React 19 & Next.js (weeks 5–8)

- Week 5 – Modern React: function components, props, `useState`, `useEffect`, lists and keys, controlled forms. What changed: React Compiler, Actions, `useActionState`.
- Week 6 – Next.js App Router: folder-based routing, layouts, dynamic routes (`[slug]`), Server Components vs Client Components (`"use client"`).
- Week 7 – Data and forms: server-side data loading, Server Actions, validation with Zod, loading and error states.
- Week 8 – Styling and i18n: Tailwind CSS, shadcn/ui, internationalization (next-intl), SEO basics (metadata).

Exercise: a "practical guides" page with a list of guides and one page per guide, in Romanian and French.

- [ ] I can explain Server Components vs Client Components
- [ ] I can create a dynamic route and a layout
- [ ] My guides page works in both languages

## Phase 3 – Backend basics (weeks 9–10)

- Week 9 – HTTP and REST: request/response, methods (GET, POST, PUT, PATCH, DELETE), status codes (200, 201, 400, 401, 404, 500), headers, JSON, CORS, clean REST routes. Tool: Bruno or Postman.
- Week 10 – Node.js: event loop, npm and `package.json`, environment variables (`.env`), a first server with Express or Fastify, middlewares, error handling.

Exercise: an in-memory listings API (create, list, update, delete), tested with Bruno.

- [ ] I know the main HTTP status codes and when to use them
- [ ] I can write a full REST CRUD
- [ ] Exercise pushed to GitHub

## Phase 4 – Databases (weeks 11–12)

- Week 11 – SQL and modeling: tables, types, primary and foreign keys, relations (one-to-many, many-to-many), SELECT, WHERE, JOIN, GROUP BY, INSERT, UPDATE, DELETE, indexes.
- Week 12 – PostgreSQL + Prisma: run PostgreSQL with Docker, Prisma schema, migrations, typed queries. Connect the phase 3 API to the database.

Exercise: design and create a basic schema: `User`, `Listing`, `Category`, `City`, with relations.

- [ ] I can write a JOIN query without help
- [ ] I can create and apply a migration
- [ ] My API stores listings in PostgreSQL

## Phase 5 – NestJS, authentication, security (weeks 13–15)

- Week 13 – NestJS: modules, controllers, services, dependency injection, DTOs and validation, pipes and exception filters. Rebuild the API with NestJS + Prisma.
- Week 14 – Authentication: password hashing (argon2/bcrypt), sessions vs JWT, refresh tokens, httpOnly cookies, guards, roles (user, pro, admin). Know ready-made solutions (Auth.js, Better Auth).
- Week 15 – Security and clean APIs: OWASP top risks (injection, XSS, CSRF), rate limiting, pagination, file uploads, Swagger/OpenAPI docs.

Exercise: NestJS listings API with sign-up, login, and only the author can edit or delete a listing.

- [ ] I can explain modules, controllers and services
- [ ] I can explain how a JWT works and its risks
- [ ] My API has Swagger documentation

## Phase 6 – Testing, Docker, CI/CD, deployment (weeks 16–17)

- Week 16 – Testing and Docker: unit tests (Vitest/Jest), API tests, one end-to-end test with Playwright. Docker: image, container, `Dockerfile`, `docker compose` for front + API + PostgreSQL.
- Week 17 – CI/CD and going live: GitHub Actions (lint + tests on every push), deploy the front (Vercel), the API and database (Railway, Render, Fly.io or a VPS), production env variables, logs and error monitoring (Sentry).

Exercise: put the mini-app online, with a CI that blocks merging if a test fails.

- [ ] I can write a unit test and an API test
- [ ] I can run the whole project with `docker compose up`
- [ ] My mini-app is online with a public URL

## Weekly review (10 min, Sunday)

- Tick the boxes of the current phase
- Write what I learned and what blocked me in the phase notes
- Ask the AI for a 5-question quiz on the week

If a phase takes longer than planned, shift the schedule rather than skipping a step.
