# MESSAGE.md

MESSAGE.md is a dynamic messaging specification for agents designed to keep AI-generated content consistent, on-brand, relevant, and uniquely yours – without breaking the token bank.

## What it is

Every AI system that generates content needs a **messaging house**: codified positioning and messaging that define the brand, audience, and portfolio. MESSAGE.md is that house, expressed as structured markdown with opinionated conventions.

But most messaging frameworks go stale the second they get written down, and agents have a hard time parsing through messaging when there's multiple products, categories, personas, alternatives in play.

What makes this specification dynamic in practice is the concept of a **messaging room**. This is runtime assembly of the right message for the right audience at the right time. The specification is designed to understand a particular scenario and only load the tightly scoped context it needs. And the structure is purpose-built to stay current to the tune of your market and business.

This specification is for anyone building AI-native content factories – product marketers, content marketers, GTM engineers, founders. The spec defines your message so agents can go do agent things (like crank out content) and you can do human things (like take a stand).

As a spec, this repository is just that. [**claude-message**](https://github.com/fortyfivan/claude-message) is a complete Claude-native reference implementation — feel free to clone, personalize, and ship. It includes a guided bootstrap workflow to setup the messaging to your company and a collection of messaging and content-generation workflows on top of the spec. 

## Core elements

- **MESSAGE.md**: sets the altitude. Your company facts, glossary of terms, brand guardrails, and scenario dimensions. Agents load this first.
- **Pillars**: tell the story. Foundational messaging documents for the company, narrative, market, audience, portfolio - with the proof to back it all up.
- **Collections**: hold the details. Granular profiles loaded on demand for specific personas, products, competitors, and more. 
- **Assets**: define the shape. Structured documents for what every asset type looks like for you, with the conventions to design and produce.

## Design Principles

- **Pluggable architecture** — Drop `MESSAGE.md` and the `messaging/` directory into any repository; your `AGENTS.md` or `CLAUDE.md` teaches the agent how to read and use it.
- **Runtime messaging** — Assembly is driven by the scenario, so the agent delivers the right message at the right time for the right reasons.
- **Progressive loading** — Tight, per-task context assembly avoids confusion, hallucination, and bloat.
- **Asset definitions** — LLMs already know how to write; they don't need skills for that. What they need is structured output and company-specific rules for better content and for downstream production.
- **Update-ready** — The structured design makes the house maintainable by agents: market moves, competitive shifts, and new innovations land as reviewable file changes. Update workflows live in the reference implementation.

## How to use

**Authoring.** The files in this repository are templates with guided instructions for you or an agent to populate. Fill the `[Instructions: …]` placeholders with your company's content — reference `[Tips: …]` for help.

**Runtime.** Wire the system into your agent by adding the MESSAGE.md handling block to your agent's `AGENTS.md` or `CLAUDE.md`. From there:

1. MESSAGE.md loads first, as always-on foundation — attributes, glossary, brand guardrails, scenario vocabulary, and the catalogs of what else is available.
2. For each task, the agent infers the **scenario** from the Scenarios dimensions, then progressively loads only the pillars, collections, and assets whose catalog **Load When** conditions match. Asset variants load when a specific variant is named.

The result is tightly scoped context assembled per task, not the entire messaging house in every prompt. Message optimized and token optimized.

## License

[MIT](LICENSE)
