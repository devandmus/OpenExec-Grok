# OpenExec-Grok

Especificación, no aplicación. Solo markdown.

Este repositorio documenta cómo el consejo de Open Executive vive en la casa Grok de Andrés (devandmus): un agente de entrada (**Open Executive**), ocho especialistas de dominio y un perfil de portafolio. **No** es un clon de FastAPI, Next.js ni Fly.

Títulos de agentes: en inglés. Cuerpo: español neutro.

## Cómo usarlo

1. Para el piso **Exec**, habla con **Open Executive**. Es el único punto de entrada.
2. **Open Executive** invoca especialistas por mensaje directo y **él** responde. Nunca «pregúntale a CSO».
3. Andrés no opera en un grupo. No hay sala de debate.
4. **Chief** es solo casa: el día y el piso de contenido. Si el tema es dominio Exec, va a **Open Executive**.

| Quién | Rol | Id Grok |
|---|---|---|
| **Open Executive** | Entrada del enjambre (invoca y resuelve) | `91d2e055-48f7-4e5f-a7e9-7a37941f7a30` |
| **Chief** | Casa: día + piso de contenido | `a7dca004-1804-40c6-ab24-b4496d6200e2` |

El canal **Exec** (`19b3438c-6870-4d5f-8bd2-5eb2cb6b9d9c`) está **inerte**. No publiques ahí. Andrés lo quitará de la barra.

NBX de la casa: el enjambre propone, uno decide. Aquí ese uno es **Open Executive** (y tú, en HITL de un toque).

Documentos → Craft (Inbox o Unsorted; nunca clasificar).
Tareas → solo OmniFocus Mail Drop:

- Para: `andresignaciomaldonado.g8kbd@sync.omnigroup.com`
- Asunto = título
- Cuerpo = `Label / URL`

## Qué es esto

Un repo de spec para el **piso Exec**: **Open Executive** gobierna el enjambre de ocho especialistas, todos vivos.

WOM es combustible, no la identidad de este consejo. IRC Abogados no entra aquí (Campaigns las lleva Jessica en otro piso).

Si un número no está escrito, se marca `unknown — do not invent`. Nadie inventa saldos, métricas ni una empresa ficticia.

## Enjambre vivo

**Entrada** (no es asiento de dominio):

- **Open Executive** — `91d2e055-48f7-4e5f-a7e9-7a37941f7a30` — gobierna el enjambre; invoca por mensaje directo y resuelve. Nombre visible: **Open Executive**, no «Orchestrator».

**Casa** (fuera del enjambre Exec):

- **Chief** — `a7dca004-1804-40c6-ab24-b4496d6200e2` — día + piso de contenido.

**Ocho especialistas** (vivos; **Open Executive** los llama por mensaje directo):

- **Chief Strategy Officer** — `953dc8b8-c8c4-4234-8a2f-a9685c147805`
- **Chief Financial Officer** — `6bfb4d79-5eb5-4439-9f26-e05f53ea8624`
- **Chief Product Officer** — `4a7f8771-0780-49ad-9ea5-7eeec804b4c7`
- **Chief Operating Officer** — `e4a8f2e1-698f-4f11-843a-cbfc7784ab79`
- **Chief People Officer** — `7b3905a9-817a-4482-9892-30bdfdc59fb8`
- **General Counsel** — `5d658ba1-5f7a-4704-84f3-6ceb7ce5228a`
- **Chief Marketing Officer** — `9ca5bdc5-e33c-45e5-8c7a-989c4018301a` — GTM de Sophieat / compañía. Nunca el pipeline social **@devandmus** ni un clon de Social Trends / Idea Filter / Social Pack.
- **Board** — `64aa4b78-fd07-42b0-bfd7-afee2962705c` — vivo; no hay ronda activa.

Sin rutinas ni relojes en estos asientos. No hay asientos de papel.

Detalle: [docs/roster.md](docs/roster.md).

## Piso de contenido (ya existe)

No lo reemplaces. No lo absorbas en Exec.

- **Research** — semilla → brief de ventaja práctica
- **Social Trends** — dos carriles sin mezclar (guitarra TikTok/IG vs tesis LinkedIn)
- **Idea Filter** — inbox de ideas: artículo+post / post / no
- **Social Pack** — Ready → pack de design system; no publica
- **Campaigns** — exclusivo IRC Abogados (Jessica lidera); fuera de este consejo

Corte entre pisos: [docs/routing.md](docs/routing.md).

## Relación con el producto Open Executive (SenteLabsAI)

El agente de entrada de este piso se llama **Open Executive** (Grok, id arriba). El producto de SenteLabsAI también se llama Open Executive. No son el mismo runtime.

Open Executive (SenteLabsAI) es un ejecutivo virtual con ocho especialistas, perfil de empresa, RAG, memoria episódica y scheduler, sobre Claude + FastAPI + Next.js. El usuario final no ve a los especialistas.

Aquí se porta la **idea** (consejo, una puerta, perfil, asientos con resultado/dueño/entradas/salidas/HITL/no-hará, decisiones por escrito). No se porta el stack. Andrés opera solo con el agente de entrada; los especialistas existen como bots Grok y se invocan por mensaje directo.

Qué se rechaza: [docs/not-copied.md](docs/not-copied.md).

## Atribución

Idea basada en **Open Executive** de SenteLabsAI:

- Upstream: https://github.com/SenteLabsAI/OpenExecutive
- Fork de Andrés: https://github.com/devandmus/OpenExecutive

Apache 2.0. Ver [NOTICE](NOTICE) y [LICENSE](LICENSE). Este repo no copia prompts, evals ni código fuente de esos proyectos.

## Documentos

| Archivo | Para qué |
|---|---|
| [docs/charter.md](docs/charter.md) | Ley de la casa: sin rebote; Open Executive resuelve; sin sala de grupo |
| [docs/roster.md](docs/roster.md) | Open Executive + ocho asientos vivos |
| [docs/routing.md](docs/routing.md) | Andrés → Open Executive → DM a especialista(s) → Open Executive resuelve |
| [docs/portfolio.md](docs/portfolio.md) | Perfil de portafolio; desconocidos marcados |
| [docs/not-copied.md](docs/not-copied.md) | Qué de OpenExecutive no se porta |
