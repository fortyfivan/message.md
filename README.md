# MESSAGE.md

MESSAGE.md is a dynamic messaging specification for AI agents — a structured way to keep AI-generated content consistent, on-brand, and relevant without dumping your whole brand into every prompt.

## What it is

Every AI system that generates content needs a **messaging house**: codified positioning, ICP, voice, and proof that define the brand. MESSAGE.md is that house, expressed as structured markdown with opinionated conventions.

What makes it dynamic is **per-task assembly**. The house is static; what an agent loads is not. A blog post for a CISO pulls different context than a sales battlecard against a named competitor. One source of truth produces calibrated outputs for every channel, audience, and use case — without loading everything every time.

## Design Principles

- **Pluggable architecture** — Drop `MESSAGE.md` and the `messaging/` directory into any repository; your `AGENTS.md` or `CLAUDE.md` teaches the agent how to read and use it.
- **Runtime messaging** — Assembly is driven by the scenario, so the agent delivers the right message at the right time for the right reasons.
- **Progressive loading** — Tight, per-task context assembly avoids confusion, hallucination, and bloat.
- **Asset definitions** — LLMs already know how to write; they don't need skills for that. What they need is structured output and company-specific rules — for better content and for downstream production.
- **Self-updating** — The dynamic design lets agents tune, add, and modify messaging from real-time intelligence: market moves, competitive shifts, new innovations.

## Core elements

| Concept | What it is |
|---|---|
| **MESSAGE.md** | The entry point. Company narrative, glossary, scenario vocabulary, and the catalog tables indexing pillars, collections, and assets. Agents load this first. |
| **Pillars** | Six foundational documents — the static layer that defines the company. |
| **Collections** | Eight granular profile types, loaded on demand. Pillars reference collection items. |
| **Assets** | Deliverable specs — what a blog post, email, or customer story looks like in your stack, and the conventions each follows. |

```
message.md/
├── MESSAGE.md                  # entry point + routing
├── CLAUDE.md                   # teaches the agent how to load the system
└── messaging/
    ├── pillars/                # profile, pitch, position, people, portfolio, proof
    ├── collections/            # personas, products, competitors, segments,
    │                           #   solutions, stories, categories, reports
    └── assets/                 # blog-post, customer-story, email, landing-page,
                                #   one-pager, press-release, social-post, whitepaper,
                                #   web-copy, slide-deck, enablement
```

- **Pillars (6)** — `profile`, `pitch`, `position`, `people`, `portfolio`, `proof`.
- **Collections (8)** — `personas`, `products`, `competitors`, `segments`, `solutions`, `stories`, `categories`, `reports`. Each holds multiple items.
- **Assets (11, extensible)** — each is an envelope (`<slug>/<slug>.md`) carrying cross-variant conventions, plus variant scaffolds under `variants/`.

## How to follow it

**Authoring.** The files in this repository are templates with guided instructions for you or your agent to populate. Fill the `[Instructions: …]` placeholders with your company's content - reference `[Tips: …]` for help. 

**Runtime.** Wire the system into your agent by adding the MESSAGE.md handling block to your agent's `AGENTS.md` or `CLAUDE.md` (as this repo's `CLAUDE.md` does). From there:

1. MESSAGE.md loads first, as always-on foundation — attributes, glossary, brand guardrails, scenario vocabulary, and the catalogs of what else is available.
2. For each task, the agent infers the **scenario** from the Scenarios dimensions, then progressively loads only the pillars, collections, and assets whose catalog **Load When** conditions match. Asset variants load when a specific variant is named.

The result is a tightly scoped context assembled per task, not the entire messaging house in every prompt.

## Reference implementation

[**claude-message**](https://github.com/fortyfivan/claude-message) is the complete Claude-native reference implementation — clone, personalize, ship. It includes a guided bootstrap and content-generation workflows on top of the spec. The fastest way to a working messaging system.
