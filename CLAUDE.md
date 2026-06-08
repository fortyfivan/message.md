# CLAUDE.md

[Instructions: add the following to your CLAUDE.md file to teach the agent how the messaging system is structured]

## About MESSAGE.md

`MESSAGE.md` is a dynamic messaging framework specification for agents to follow. It represents the totality of a company's positioning and messaging, modeled for dynamic progressive loading based on real-time task scenarios. 

## Always-On Foundation

`MESSAGE.md` loads automatically at session start as foundational context. It provides:

- Company attributes (altitude-setters)
- Glossary (cross-cutting terminology)
- Brand Guardrails (absolute constraints)
- Scenarios vocabulary (dimensions for runtime assembly)
- Messaging pillars (foundational company messaging)
- Collection profiles (specific messaging elements)
- Asset definitions (content artifacts)

## Progressive Loading

After MESSAGE.md, the agent loads additional content based on task context. The catalog tables in MESSAGE.md declare what's available and the load conditions for each.

**Two steps before any task-specific load:**

1. **Infer the scenario** from the Scenarios dimensions in MESSAGE.md, the task, and current context (insights, recent messaging house activity, explicit signals in the request).
2. **Assemble the context** by loading pillars, collections, and assets per the rules below. Apply the inferred content lens to set posture; let the Strategic shape guide which collections and pillars to emphasize.

**Default loading behavior:**

- **Pillars** load per the catalog's `Load When` column. Profile and Pitch load always. Position, People, and Proof load by default for marketing content. Portfolio loads when content references products.
- **Collections** load per the catalog's `Load When` column. Each collection loads when content references its specific entity type (personas when a named role/tier appears, competitors when a named competitor appears, etc.).
- **Assets** load when a specific asset is referenced by content type. Variants under the asset's `variants/` directory load when a specific variant is named.
