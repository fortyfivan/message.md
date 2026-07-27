# CLAUDE.md

[Instructions: add the following to your CLAUDE.md file to teach the agent how the messaging system is structured]

## About MESSAGE.md

`MESSAGE.md` is a dynamic messaging framework specification for agents to follow. It represents the totality of a company's positioning and messaging, modeled for dynamic progressive loading based on real-time task scenarios. 

## Always-On Foundation

Read `MESSAGE.md` before starting any messaging or content task — it is the foundational context everything else builds on. It provides:

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

1. **Infer the scenario** from the Scenarios dimensions in MESSAGE.md, the task, and current context.
2. **Assemble the context** by loading pillars, collections, and assets per the rules below, letting each scenario dimension shape the assembly.

**Default loading behavior:**

- **Pillars** load per the catalog's `Load When` column.
- **Collections** load per the catalog's `Load When` column. Entity recognition is grounded in the catalog's `Known Entities` column: when content references an entity listed there, load that profile from the collection's directory.
- **Assets** load when generating content. Variants under the asset's `variants/` directory load per the `Load When` column in that asset's own `## Variants` table — the same mechanism as the Pillars/Collections `Load When` columns — not only when a specific variant is named.
- **Templates** — a variant with a sibling `variants/[slug].html` file uses it as the HTML render template. Load it only when producing HTML output, and fill its `{{placeholders}}` from the asset's Output frontmatter fields and the variant's Structure sections.
