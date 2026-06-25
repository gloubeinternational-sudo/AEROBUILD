# DEV_RULES

## MODULE

Development Rules

---

## PURPOSE

Define mandatory development rules for Codex and all future contributors.

---

## LANGUAGE

All source code, comments, commits, documentation files and technical names must be written in English.

---

## STACK

Frontend:
- React
- TypeScript
- Telegram WebApp SDK

Backend:
- Python
- FastAPI

Database:
- PostgreSQL

Infrastructure:
- Docker
- GitHub
- Environment variables
- REST API

---

## PROJECT STRUCTURE

backend/

frontend/

database/

docs/

scripts/

assets/

---

## BACKEND RULES

- Use FastAPI.
- Use async endpoints where possible.
- Use Pydantic schemas.
- Separate routers, services, models and repositories.
- Do not place business logic inside API routes.
- Use clear error handling.
- Use environment variables for secrets.

---

## FRONTEND RULES

- Use React with TypeScript.
- Build mobile-first UI.
- Optimize for Telegram Mini App.
- Keep screens simple.
- Use reusable components.
- Do not hardcode API URLs.
- Use environment variables.

---

## DATABASE RULES

- Use PostgreSQL.
- Every table must have an ID.
- Use created_at and updated_at fields.
- Use foreign keys for relations.
- Use indexes for frequently queried fields.
- Store payment and transaction history permanently.

---

## API RULES

- REST API.
- Version prefix: /api/v1
- JSON only.
- Use consistent response format.
- Validate all input.
- Return proper HTTP status codes.
- Protect private endpoints with authentication.

---

## AUTHENTICATION

- Telegram Login.
- JWT access token.
- Refresh token.
- Role-based access control.

---

## SECURITY

- Never store secrets in code.
- Use HTTPS in production.
- Validate Telegram authentication data.
- Use rate limiting.
- Log security events.
- Protect admin endpoints.

---

## PAYMENTS

- Every payment must create an order.
- Every confirmed payment must create a transaction.
- Every transaction must be auditable.
- Failed payments must be stored.
- Refunds must be traceable.

---

## ADMIN PANEL

Admin panel must allow:

- User management.
- Aircraft management.
- Product management.
- Payment monitoring.
- Transaction review.
- Analytics.
- System settings.

---

## NAMING RULES

- Use snake_case for database fields.
- Use camelCase for frontend variables.
- Use PascalCase for React components.
- Use lowercase API routes.
- Use English names only.

---

## GIT RULES

Branches:

- main
- develop
- feature/*
- fix/*

Commits must be clear and short.

Examples:

- add user authentication
- create aircraft model
- implement payment endpoint

---

## TESTING

Required tests:

- API tests.
- Database tests.
- Payment flow tests.
- Authentication tests.
- Critical business logic tests.

---

## ENVIRONMENT

Required files:

- .env.example
- docker-compose.yml
- README.md

Production secrets must not be committed.

---

## CODEX RULES

Codex must:

- Read docs before writing code.
- Follow DEV_RULES.md.
- Follow SYSTEM_ARCHITECTURE.md.
- Use DATABASE.md for data models.
- Use API.md for endpoints.
- Use TELEGRAM_MINI_APP.md and UX_UI.md for frontend flow.
- Not invent features outside specification without marking them as TODO.
- Ask for clarification if implementation conflicts with documentation.

---

## STATUS

Draft v1.0
