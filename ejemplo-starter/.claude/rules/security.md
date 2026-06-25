# Regla: Seguridad

- Nunca hardcodear secretos; usar variables de entorno (`process.env`).
- Toda entrada de usuario se valida en el servidor (esquema con zod).
- Consultas a BD siempre vía Prisma (parametrizadas); nunca SQL por concatenación.
- Escapar/renderizar de forma segura el contenido de usuario en el frontend.
- No registrar (log) datos sensibles: tokens, contraseñas, PII.
- Dependencias nuevas: revisar que sean mantenidas y necesarias antes de añadir.
