---
name: pr-description
description: Redacta la descripción de un Pull Request a partir de los commits y el diff. Úsalo al cerrar una feature.
---

# Descripción de Pull Request

Genera la descripción con esta estructura exacta:

```
## Qué
<resumen en 1-2 frases de lo que cambia>

## Por qué
<el problema o necesidad que resuelve>

## Cómo probarlo
1. <pasos concretos para validar>

## Notas
<riesgos, decisiones, follow-ups si los hay>
```

Reglas:
- Basa todo en el `git diff` real, no inventes cambios.
- Lista breaking changes al inicio con ⚠️ si los hay.
- Mantén el "Qué" entendible para alguien sin contexto.
