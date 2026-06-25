# 📦 Claude Code Starter — Estructura de referencia

Este es un proyecto de ejemplo que muestra la **anatomía canónica** de un repositorio
listo para trabajar con Claude Code siguiendo buenas prácticas. Úsalo como plantilla.

```
claude-code-starter/
├── CLAUDE.md                      # Memoria del proyecto (la lee Claude en cada sesión)
├── README.md                      # Este archivo
├── .claude/
│   ├── settings.json              # Permisos + hooks del proyecto
│   ├── agents/                    # Subagentes especializados
│   │   ├── code-reviewer.md       #   · revisa diffs antes del commit
│   │   ├── test-writer.md         #   · escribe tests siguiendo el estilo del repo
│   │   └── explorer.md            #   · mapea codebases desconocidos (read-only)
│   ├── skills/                    # Flujos reutilizables (se invocan por nombre)
│   │   ├── new-component/SKILL.md #   · crea un componente con las convenciones
│   │   ├── log-triage/SKILL.md    #   · diagnostica un error desde los logs
│   │   └── pr-description/SKILL.md #   · redacta la descripción del PR
│   └── rules/                     # Reglas siempre activas (referenciadas por CLAUDE.md)
│       ├── coding-style.md
│       ├── testing.md
│       └── security.md
└── docs/                          # "Second Brain": conocimiento que no cabe en CLAUDE.md
    ├── architecture.md
    └── decisions.md
```

## Las 3 piezas clave

| Pieza | Qué es | Cuándo se usa |
|-------|--------|---------------|
| **CLAUDE.md** | La memoria del proyecto | Se carga automáticamente en cada sesión |
| **Skills** (`.claude/skills/`) | Flujos repetibles empaquetados | Claude los invoca cuando la tarea coincide |
| **Agents** (`.claude/agents/`) | Especialistas con contexto propio | Para delegar (revisar, testear, explorar) |

> 💡 Regla de oro: **CLAUDE.md = QUÉ y bajo qué reglas. Skills = CÓMO repetir un flujo. Agents = QUIÉN hace una tarea aislada.**
