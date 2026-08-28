# OpenExec-Grok

Especificación, no aplicación. Solo markdown.

Este repositorio documenta cómo el consejo de Open Executive vive en la casa Grok de Andrés (devandmus): una puerta, especialistas de dominio y un perfil de portafolio. **No** es un clon de FastAPI, Next.js ni Fly.

Títulos de agentes: en inglés. Cuerpo: español neutro.

## Cómo usarlo

1. Habla con **Chief**. Es la única puerta de este piso.
2. Chief da **una** asignación a **un** especialista.
3. El grupo **Exec** es la sala del consejo. Entra cuando tú te sientas ahí. No es la vía por defecto.

| Quién | Rol | Id Grok |
|---|---|---|
| **Chief** | Puerta | `a7dca004-1804-40c6-ab24-b4496d6200e2` |
| **Exec** | Sala (grupo) | `19b3438c-6870-4d5f-8bd2-5eb2cb6b9d9c` |

NBX de la casa: el enjambre propone, uno decide. Aquí ese uno es Chief (y tú, en HITL de un toque).

Documentos → Craft (Inbox o Unsorted; nunca clasificar).
Tareas → solo OmniFocus Mail Drop:

- Para: `andresignaciomaldonado.g8kbd@sync.omnigroup.com`
- Asunto = título
- Cuerpo = `Label / URL`

## Qué es esto

Un repo de spec para el **piso Exec**: CSO, CFO, CPO en vivo; el resto de asientos en papel.

WOM es combustible, no la identidad de este consejo. IRC Abogados no entra aquí (Campaigns las lleva Jessica en otro piso).

Si un número no está escrito, se marca `unknown — do not invent`. Nadie inventa saldos, métricas ni una empresa ficticia.

## Vivo ahora vs solo papel

**Vivos** (bots Grok con id):

- **Chief Strategy Officer** — `953dc8b8-c8c4-4234-8a2f-a9685c147805`
- **Chief Financial Officer** — `6bfb4d79-5eb5-4439-9f26-e05f53ea8624`
- **Chief Product Officer** — `4a7f8771-0780-49ad-9ea5-7eeec804b4c7`

Sin rutinas ni relojes en estos tres. No despiertes a los tres sobre el mismo tema.

**Solo papel** (especificación completa; no son bots Grok):

- **CHRO** / Chief People Officer
- **GC** / General Counsel
- **COO**
- **CMO** — nunca un clon del piso de contenido
- **Board Communications**

Detalle: [docs/roster.md](docs/roster.md).

## Piso de contenido (ya existe)

No lo reemplaces. No lo absorbas en Exec.

- **Research** — semilla → brief de ventaja práctica
- **Social Trends** — dos carriles sin mezclar (guitarra TikTok/IG vs tesis LinkedIn)
- **Idea Filter** — inbox de ideas: artículo+post / post / no
- **Social Pack** — Ready → pack de design system; no publica
- **Campaigns** — exclusivo IRC Abogados (Jessica lidera); fuera de este consejo

Corte entre pisos: [docs/routing.md](docs/routing.md).

## Relación con Open Executive

Open Executive (SenteLabsAI) es un ejecutivo virtual con ocho especialistas, perfil de empresa, RAG, memoria episódica y scheduler, sobre Claude + FastAPI + Next.js. El usuario final no ve a los especialistas.

Aquí se porta la **idea** (consejo, una puerta, perfil, asientos con resultado/dueño/entradas/salidas/HITL/no-hará, decisiones por escrito). No se porta el stack ni se ocultan chats: en Grok los especialistas se ven.

Qué se rechaza: [docs/not-copied.md](docs/not-copied.md).

## Atribución

Idea basada en **Open Executive** de SenteLabsAI:

- Upstream: https://github.com/SenteLabsAI/OpenExecutive
- Fork de Andrés: https://github.com/devandmus/OpenExecutive

Apache 2.0. Ver [NOTICE](NOTICE) y [LICENSE](LICENSE). Este repo no copia prompts, evals ni código fuente de esos proyectos.

## Documentos

| Archivo | Para qué |
|---|---|
| [docs/charter.md](docs/charter.md) | Ley de la casa en este piso |
| [docs/roster.md](docs/roster.md) | Ocho asientos: vivo / papel |
| [docs/routing.md](docs/routing.md) | Contenido vs Exec; secuencia Andrés → Chief → uno |
| [docs/portfolio.md](docs/portfolio.md) | Perfil de portafolio; desconocidos marcados |
| [docs/not-copied.md](docs/not-copied.md) | Qué de OpenExecutive no se porta |
