# Qué no se porta de Open Executive

Este repo toma la **idea** del consejo. No toma el producto. No copies archivos, prompts ni evals desde:

- https://github.com/SenteLabsAI/OpenExecutive
- https://github.com/devandmus/OpenExecutive (fork de Andrés; misma regla)

Apache 2.0 exige atribución (ver [NOTICE](../NOTICE)), no un fork disfrazado de markdown.

## Stack y runtime — no

- FastAPI, uvicorn, Python de aplicación, `packages/core`
- Next.js, App Router, Tailwind, `packages/ui`
- Fly.io (`fly.api.toml`, `fly.ui.toml`, honcho, QA twin, volúmenes, tokens de deploy)
- Docker / docker-compose / Makefile de app
- ChromaDB, sentence-transformers, índices vectoriales
- SQLite de memoria episódica, Honcho como capa de memoria
- Claude / Anthropic como backbone obligatorio, prompt caching, extended thinking
- OpenRouter, modelos locales tipo Ollama/vLLM como “mismo orquestador”
- CI de producto, evals como gate, “CI theater” en este repo
- Variables de entorno, `.env.example`, wizard de onboarding con YAML de empresa

## Interfaces que la casa no usa así — no

- Bots de Slack, Discord, Telegram, Google Chat
- Poller IMAP/SMTP de “email executive”
- CLI `openexecutive chat` / upload API
- Web UI en localhost:3000
- Especialistas **ocultos** detrás de una sola voz (en Grok los chats se ven)

## Orquestación y relojes — no

- Llamadas paralelas a los ocho especialistas por cada mensaje
- Router con tool-use a un registry de ocho
- Scheduler / job runner / `UPDATE … RETURNING`
- Ocho cron clocks (uno por asiento) o alerts proactivos de producto
- Rutinas en CSO, CFO o CPO (charter: cero relojes en los tres vivos)

## Conocimiento y fixtures — no

- RAG sobre markdown MBA (`knowledge/builtin/` u equivalente)
- Colección `company_docs` / upload de decks al vector store
- Fixtures **Halcyon Motors**, **Meridian Petroleum**, **Tandem Robotics**
- Profiles, rosters o docs de demo de esas empresas
- Completar un “company profile” de startup de muestra

## Código, prompts, evals — no

- `packages/core/openexecutive/prompts/` y cualquier persona/domain prompt
- Agentes Python (`agents/`, `orchestrator/`, `workflows/`)
- `evals/` (escenarios, LLM-as-judge, rúbricas)
- Scripts de operador (Fly secrets, Google auth)
- Architecture internals, audit log de app, people/talent modules de producto

## Semántica que no se copia

| Open Executive | Esta casa |
|---|---|
| Una voz ejecutiva; el usuario no ve especialistas | Chats Grok visibles; Chief es puerta, no máscara |
| Company = startup onboarded | Company = portafolio de Andrés; nada ficticio |
| Memoria episódica en SQLite | Decisiones por escrito en Craft (Inbox / Unsorted) |
| Tareas / follow-ups del scheduler | Solo OmniFocus Mail Drop |
| CMO = GTM genérico de la app | CMO papel ≠ clon de Social Trends / Idea Filter / Social Pack |
| Ocho asientos en caliente | Tres vivos; cinco en papel hasta que haya trabajo semanal |

## Qué sí se copia (idea)

- Consejo de especialistas de dominio
- Una puerta
- Un perfil de company/portafolio
- Cada asiento: result / owner / inputs / outputs / HITL / will-not-do
- Decisiones episódicas que viven por escrito

Si un PR trae `.py`, app, workflow de CI de producto, prompt pegado o fixture de Halcyon/Meridian/Tandem: fuera de alcance. Rechazar.
