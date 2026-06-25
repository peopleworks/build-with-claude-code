---
name: new-component
description: Crea un componente React siguiendo las convenciones de TaskFlow. Úsalo cuando pidan "crea un componente" o "nuevo componente".
---

# Crear componente React

1. Ubícalo en `web/src/components/<Nombre>/`.
2. Archivos: `<Nombre>.tsx`, `<Nombre>.test.tsx`, `index.ts` (re-export).
3. Componente funcional con TypeScript; props tipadas con una `interface` exportada.
4. Nada de estilos inline; usa CSS modules (`<Nombre>.module.css`).
5. Si consume datos, recíbelos por props o por un hook; no fetch dentro del render.
6. Genera el test base (render + una interacción) en `<Nombre>.test.tsx`.
7. Si tocas más de este componente, propón el plan antes de escribir.
