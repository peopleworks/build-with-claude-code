# Arquitectura — TaskFlow (Second Brain)

Documentación que NO cabe en CLAUDE.md pero que Claude puede cargar bajo demanda.

## Visión general
TaskFlow es un monorepo con dos paquetes: `api/` (backend) y `web/` (frontend),
que comparten tipos generados desde el esquema de Prisma.

## Flujo de una petición
1. `web/` llama a `POST /tasks` con el token JWT en el header.
2. `api/middleware/auth.ts` valida el token y adjunta `req.user`.
3. `api/routes/tasks.ts` valida el body con zod y delega en `api/services/taskService.ts`.
4. El service usa Prisma para persistir y devuelve el DTO.

## Modelo de datos
- `User` 1—N `Task`
- `Project` 1—N `Task`
- Una `Task` pertenece a un `User` (owner) y opcionalmente a un `Project`.

## Decisiones clave
Ver `docs/decisions.md` para el registro de decisiones de arquitectura (ADR).
