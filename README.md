# MESSAGE.md

MESSAGE.md is a dynamic messaging specification for agents designed to keep AI-generated content consistent, relevant, and uniquely yours – without breaking the token bank.

## What it is

Every AI GTM content factory needs a **messaging house**: a codified positioning and messaging framework that define the brand, audience, and portfolio so agents don't go off the rails. MESSAGE.md is that house, expressed as structured markdown with opinionated conventions.

This specification is for product marketers, content marketers, GTM engineers, founders, or anyone building AI GTM systems. The spec defines your positioning and messaging so agents can do agent things (like crank out content) and you can do human things (like have an opinion).

This repository is the specification only with instructions to populate. [**claude-message**](https://github.com/fortyfivan/claude-message) is a complete Claude-native reference implementation — feel free to clone, personalize, and ship. It includes a guided bootstrap workflow to setup the messaging to your company. 

## Core elements

- **MESSAGE.md**: sets the altitude. Your company facts, glossary of terms, brand guardrails, and scenario dimensions. Agents load this first.
- **Pillars**: tell the story. Foundational messaging documents for the company, narrative, market, audience, portfolio - with the proof to back it all up.
- **Collections**: hold the details. Granular profiles loaded on demand for specific personas, products, competitors, and more. 
- **Assets**: define the shape. Structured documents for what every asset type looks like for you, with the conventions to design and produce — each carrying an output contract: metadata and arrays in the envelope, body keys annotated on each variant's structure.

## Design Principles

- **Pluggable architecture** — Drop populated `MESSAGE.md` and the `messaging/` directory into any repository; your `AGENTS.md` or `CLAUDE.md` teaches the agent how to read and use it.
- **Runtime assembly** — Context is driven by the scenario, so the agent delivers the right message at the right time for the right reasons.
- **Progressive loading** — Tight, per-task context assembly avoids confusion, hallucination, and bloat.
- **Asset definitions** — LLMs already know how to write; they don't need skills for that. What they need is structured output and company-specific rules for better content and for downstream production. Each asset declares that output contract explicitly: the envelope's `## Output schema` owns the invariant head — metadata and arrays the destination consumes — while each variant's `## Structure` annotates its sections with `{snake_case}` body keys, so the structured output stays in sync with the structure by construction. Rendering to a target format is delegated to a conformant visual spec; the messaging spec stays messaging-pure.
- **Update-ready** — The structured design makes the house maintainable by agents: market moves, competitive shifts, and new innovations land as reviewable file changes. Update workflows live in the reference implementation.

## Getting Started

**Authoring.** The files in this repository are templates with guided instructions for you or an agent to populate. Fill the `[Instructions: ...]` placeholders with your company's content — reference `[Tips: ...]` for help.

**Runtime.** Wire the system into your agent by adding the MESSAGE.md handling block to your agent's `AGENTS.md` or `CLAUDE.md`. From there:

1. MESSAGE.md loads first, as always-on foundation — attributes, glossary, brand guardrails, scenario vocabulary, and the catalogs of what else is available.
2. For each task, the agent infers the **scenario** from the Scenarios dimensions, then progressively loads only the pillars, collections, and assets whose catalog **Load When** conditions match. Asset variants load the same way, per the `Load When` column in each asset's own `## Variants` table.

The result is tightly scoped context assembled per task, not the entire messaging house in every prompt. Message optimized and token optimized.

## How to Use

A fully populated **messaging house** serves as the core context layer for your GTM engine. Depending on your system, harness, tools, and integrations, there's a number of ways to leverage and extend this context:

- **Content Production**: Write web copy, blog posts, landing pages, datasheets, whitepapers, etc., that doesn't suck by using the messaging house as the source of truth for what to say and how to say it.

- **Campaign Planning**: Build out the plan and complete Bill of Materials for marketing campaigns, product launches, events, and sales plays using the messaging house to formulate the right strategy, the right narrative, and the right set of assets.

- **Outreach Messaging**: Ensure that your signal-based workflows don't go off the rails by hooking into the messaging house to assemble tightly scoped context that will craft the most relevant outreach copy.

- **Enablement Programs**: Make supporting training, reference, and supporting content automatic to the tune of every piece of news, launch, and play by hooking up the messaging house to 

- **Continuous Research**: hook up scheduled tasks and loops to the messaging house to perform market, competitive, field, and community research. Bring any notable findings back into the messaging so you are always current to the tune of your environment. Ref: https://github.com/fortyfivan/claude-message/blob/main/.claude/skills/system/run-investigation/SKILL.md


## License

[MIT](LICENSE)
