# Registro de decisiones (ADR)

## ADR-001 · Prisma como ORM
**Contexto:** necesitábamos type-safety entre BD y código.
**Decisión:** usar Prisma; genera tipos desde `schema.prisma`.
**Consecuencia:** migraciones versionadas; menos SQL manual.

## ADR-002 · Monorepo api + web
**Contexto:** frontend y backend comparten tipos.
**Decisión:** un solo repo con dos paquetes y tipos compartidos.
**Consecuencia:** un solo PR puede cambiar contrato y consumidor a la vez.

## ADR-003 · Vitest sobre Jest
**Contexto:** el frontend usa Vite.
**Decisión:** Vitest por velocidad y config compartida con Vite.
**Consecuencia:** un solo runner para todo el repo.
