# Regla: Estilo de código

- TypeScript estricto; nada de `any` salvo justificación en comentario.
- Nombres en inglés; funciones = verbos (`getUser`), booleanos = `is/has/can`.
- Funciones pequeñas y puras cuando sea posible; máximo ~40 líneas.
- Prefiere `const`; evita mutación; usa métodos de array sobre bucles imperativos.
- Sin código muerto ni comentarios obvios; comenta el *por qué*, no el *qué*.
- Imports ordenados: librerías externas, luego internas, luego relativos.
