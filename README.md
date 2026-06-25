<div align="center">

# 🤖 Build with Claude Code

### Plan de curso **+** manual de laboratorio interactivo para dominar Claude Code

[![Pagina en vivo](https://img.shields.io/badge/🌐_Pagina_en_vivo-peopleworks.github.io-7c3aed?style=for-the-badge)](https://peopleworks.github.io/build-with-claude-code/)
[![Hecho con Claude Code](https://img.shields.io/badge/Hecho_con-Claude_Code-0F766E?style=for-the-badge&logo=anthropic&logoColor=white)](https://claude.com/claude-code)

![Licencia](https://img.shields.io/badge/Licencia-MIT-14B8A6?style=flat-square)
![HTML](https://img.shields.io/badge/HTML-autonomo-ff9d10?style=flat-square)
![Curso](https://img.shields.io/badge/Curso-3_dias-7c3aed?style=flat-square)

*De carpeta vacía a una app full-stack con base de datos real conectada — usando buenas prácticas.*

</div>

---

## 🌐 Página en vivo

👉 **[peopleworks.github.io/build-with-claude-code](https://peopleworks.github.io/build-with-claude-code/)**

Un solo `index.html` autónomo que funciona como **plan de curso** y, a la vez, como **laboratorio que ejecutas paso a paso**: comandos copy-paste, biblioteca de prompts y los trucos que aprendimos a la fuerza.

---

## 📂 Qué hay en este repo

| Recurso | Descripción |
|---|---|
| 🖥️ **`index.html`** | La página del curso: temario de 3 días, los 5 pilares, laboratorio paso a paso, comandos, prompts y trucos. Con botones **"Copiar"** en cada bloque. |
| 📦 **`ejemplo-starter/`** | La **estructura de referencia** de un repo *Claude-ready*: `CLAUDE.md`, agentes, skills, reglas y "Second Brain". Úsalo como plantilla. |

---

## 🚀 Empieza en 60 segundos

```bash
# 1. Clona el repo
git clone https://github.com/peopleworks/build-with-claude-code.git
cd build-with-claude-code

# 2. Abre la guía en el navegador
#    Windows:  start index.html
#    Mac:      open index.html

# 3. ¿Quieres la plantilla de proyecto? Cópiala y arranca Claude Code
cp -r ejemplo-starter mi-proyecto
cd mi-proyecto
claude
```

---

## 🧪 El laboratorio en 10 pasos

> El recorrido completo que ejecutamos en vivo — de cero a app conectada.

1. **Crear el proyecto** → `mkdir` · `git init`
2. **Lanzar Claude Code** → `claude`
3. **Darle memoria** → `/init` (genera el `CLAUDE.md`)
4. **Crear una Skill y un Agente**
5. **Plan Mode** antes de codear → `Shift + Tab`
6. **Construir** usando la Skill (tests primero)
7. **Conectar PostgreSQL** → `.env` + `npx prisma migrate dev`
8. **Ver la base de datos** → `npx prisma studio`
9. **Correr la app** → `npm run dev`
10. **Revisar con el Agente** y cerrar el **Pull Request**

*El detalle de cada paso, con comandos y prompts, está en la [página en vivo](https://peopleworks.github.io/build-with-claude-code/#laboratorio).*

---

## 🗂️ Anatomía de un proyecto *Claude-ready*

```
ejemplo-starter/
├── CLAUDE.md                 # 🧠 la memoria del proyecto
├── .claude/
│   ├── settings.json         # permisos + hooks
│   ├── agents/               # 🤖 subagentes especializados
│   │   ├── code-reviewer.md
│   │   ├── test-writer.md
│   │   └── explorer.md
│   ├── skills/               # ✨ flujos reutilizables
│   │   ├── new-component/SKILL.md
│   │   ├── log-triage/SKILL.md
│   │   └── pr-description/SKILL.md
│   └── rules/                # 📏 reglas siempre activas
│       ├── coding-style.md
│       ├── testing.md
│       └── security.md
└── docs/                     # 📚 "Second Brain"
    ├── architecture.md
    └── decisions.md
```

---

## 🔑 La regla de oro

> ### 🧠 `CLAUDE.md` = **QUÉ** y bajo qué reglas &nbsp;·&nbsp; ✨ **Skills** = **CÓMO** repetir un flujo &nbsp;·&nbsp; 🤖 **Agents** = **QUIÉN** hace una tarea aislada

---

## ⌨️ Comandos y atajos esenciales

| Acción | Atajo / comando |
|---|---|
| Inicializar `CLAUDE.md` | `/init` |
| Limpiar el contexto | `/clear` |
| Gestionar subagentes | `/agents` |
| Cambiar de modo (plan / accept edits) | `Shift + Tab` |
| Guardar en memoria | `# tu nota` |
| Ejecutar comando bash | `! comando` |

💡 **Truco de oro (Windows):** si la base de datos "no responde" aunque el servicio corra, usa **`127.0.0.1`** en vez de `localhost`.

---

## 👤 Autor

**Pedro Hernández** — CEO de PeopleWorks · Microsoft MVP (Developer Technologies, .NET)

[![GitHub](https://img.shields.io/badge/GitHub-peopleworks-181717?style=flat-square&logo=github)](https://github.com/peopleworks)

---

## 📜 Licencia y créditos

Publicado bajo licencia **MIT** — úsalo, modifícalo y compártelo libremente.

Temario inspirado en el curso **"Build with Claude Code"** de ByteByteGo (John Kim). Materiales y código de este repo preparados por **PeopleWorks**.

<div align="center">

**¿Te sirvió? Dale una ⭐ al repo y compártelo con tu equipo.**

*Hecho con ❤️ y 🤖 Claude Code*

</div>
