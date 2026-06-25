---
name: log-triage
description: Diagnostica un error a partir de logs o un stack trace. Úsalo cuando peguen un error, un log o digan "falla en producción".
---

# Triage de logs

1. Lee el stack trace de abajo hacia arriba: la última línea de TU código es el origen.
2. Abre ese `archivo:línea` y lee el contexto alrededor.
3. Reproduce mentalmente el estado que causó el fallo (valores nulos, race, etc.).
4. Forma una hipótesis ANTES de cambiar nada y dila.
5. Propón el fix mínimo + un **test de regresión** que falle hoy y pase con el fix.
6. No silencies el error con try/catch vacío.
