# 📚 Lector Activo — Agent Skill para Lectura Profunda

> **Un compañero de lectura activa que convierte libros en acción.**
> Compatible con Claude Code y cualquier agente que soporte el estándar SKILL.md.

---

## ¿Qué hace este skill?

La mayoría de los enfoques de lectura producen notas que nunca se usan.
Este skill cambia eso: en lugar de resumir pasivamente, activa un sistema de
6 modos que llevan cada libro desde la primera exploración hasta la aplicación
concreta en proyectos reales.

**El objetivo, ademas de lectura, es activar ideas.**

Diseñado para libros de no ficción, tecnología/IA y filosofía/pensamiento sistémico.

---

## Los 6 Modos

| Modo | Trigger | Para qué |
|------|---------|----------|
| 🔍 **EXPLORAR** | `explorar [libro]` | Decidir si vale leerlo y cómo |
| 📖 **LEER** | `capítulo [N]: [tema]` | Procesar secciones en tiempo real |
| 🧠 **SINTETIZAR** | `sintetizar [libro]` / `terminé [libro]` | Consolidar el libro completo |
| 🔗 **CONECTAR** | `conectar [libro A] con [libro B]` | Lectura sintópica entre libros |
| 🚀 **ACTIVAR** | `activar para [proyecto]` | Convertir conocimiento en acción |
| 📤 **EXPORTAR** | `exportar notebooklm / tarjetas / mindmap / guion [libro]` | Generar insumos para otras herramientas |

---

## Instalación

### Claude Code
```bash
# Instalación en proyecto (compartida con el equipo)
cp -r lector-activo-skill/ .claude/skills/

# Instalación personal (disponible en todos tus proyectos)
cp -r lector-activo-skill/ ~/.claude/skills/
```

### OpenAI Codex CLI
```bash
cp -r lector-activo-skill/ ~/.codex/skills/
```

El agente activará el skill automáticamente cuando detecte el contexto de lectura,
o podés activarlo con los triggers explícitos de la tabla de arriba.

---

## Ejemplos de uso

```
explorar Thinking, Fast and Slow
```
```
capítulo 3: Los dos sistemas
```
```
sintetizar The Mom Test
```
```
conectar Thinking Fast and Slow con The Black Swan
```
```
activar para lanzamiento de producto en Q3
```
```
exportar notebooklm Thinking, Fast and Slow
```
```
exportar tarjetas The Mom Test
```

---

## Marco metodológico

Este skill integra y combina:

- **Mortimer Adler** — *How to Read a Book*: lectura inspectiva, analítica y sintópica
- **Richard Feynman** — Técnica Feynman: si no podés explicarlo simple, no lo entendés
- **Tiago Forte** — *Building a Second Brain* (CODE): Capture, Organize, Distill, Express
- **Make It Stick** (Brown, Roediger, McDaniel): recuperación activa y práctica intercalada
- **Niklas Luhmann** — Zettelkasten: conexiones entre ideas, no colecciones de notas
- **Scott Young** — *Ultralearning*: el aprendizaje más rápido es el más aplicado
- **Sönke Ahrens** — *How to Take Smart Notes*: Progressive Summarization

---

## Exportación a herramientas externas

El Modo 6 genera insumos listos para:

| Comando | Genera | Herramienta |
|---------|--------|-------------|
| `exportar notebooklm [libro]` | Documento fuente completo | [NotebookLM](https://notebooklm.google.com) |
| `exportar tarjetas [libro]` | 20 flashcards Q&A | Anki / Quizlet |
| `exportar mindmap [libro]` | Jerarquía Markdown | Miro / XMind / Coggle / Obsidian |
| `exportar guion [libro]` | Guion conversacional | Video / Podcast / NotebookLM Audio |

**Flujo más potente:**
`sintetizar [libro]` → `exportar notebooklm [libro]` → subir a NotebookLM → podcast + mindmap + study guide en un clic.

---

## Principios de diseño

- **Sin resumen sin tensión crítica.** Un resumen sin desacuerdo es información muerta.
- **Sin aplicación forzada.** Si una idea no conecta con nada concreto, se dice.
- **Profundidad calibrada.** Algunos libros merecen 20 minutos, otros 20 horas.
- **Test Feynman siempre disponible.** Si algo suena abstracto, se traduce.

---

## Autor

Creado por [Adrian Lasso](https://github.com/alasso) — socio y director de desarrollo de negocios en [Baufest](https://baufest.com), mentor en el ecosistema emprendedor.

---

## Licencia

MIT License — libre para usar, modificar y distribuir.

---

*Skill compatible con el estándar abierto [SKILL.md](https://agentskills.io) — funciona con Claude Code, OpenAI Codex CLI y cualquier agente compatible.*
