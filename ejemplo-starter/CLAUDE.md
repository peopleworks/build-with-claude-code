# TaskFlow — Gestor de tareas full-stack (proyecto de ejemplo)

App de ejemplo para enseñar la estructura. Un gestor de tareas con API y frontend.

## Stack
- **Backend:** Node.js + Express + PostgreSQL (Prisma ORM)
- **Frontend:** React + Vite + TypeScript
- **Tests:** Vitest (unit) + Playwright (e2e)
- **Lint/format:** ESLint + Prettier

## Arquitectura
- `api/` — servidor Express; rutas en `api/routes/`, lógica en `api/services/`
- `web/` — app React; componentes en `web/src/components/`
- `prisma/schema.prisma` — modelo de datos (User, Task, Project)
- Más detalle en `docs/architecture.md`

## Comandos
- `npm run dev` — levanta API (:3000) y web (:5173)
- `npm test` — corre todos los tests
- `npm run lint` — ESLint sobre todo el repo

## Reglas siempre activas
Sigue las reglas en:
- `.claude/rules/coding-style.md`
- `.claude/rules/testing.md`
- `.claude/rules/security.md`

## Lo que Claude debe hacer
- Proponer un plan antes de tocar más de un archivo (usa plan mode).
- Escribir o actualizar tests para cualquier cambio de comportamiento.
- Usar el agente `code-reviewer` antes de proponer un commit.

## Lo que Claude NO debe hacer
- No instalar dependencias nuevas sin proponerlo primero.
- No commitear secretos; usar variables de entorno (`.env`, nunca en el repo).
- No desactivar reglas de lint con `// eslint-disable` para "que pase".
