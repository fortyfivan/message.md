---
slug: customer-story
status: active
default-variant: ""
---

# Customer Story

[Instructions:
Long-form customer narrative for the website's customers section, sales enablement, and proof-led marketing. 

This file carries only the company conventions that hold across every customer-story variant — length bands, sourcing rules, approval workflow, metrics provenance. Structure and CTA conventions live in each variant under `variants/` since they vary by editorial intent.]

## Conventions

[Instructions:
Specify the company's customer-story standards that hold across variants:
- Length bands (e.g., 600-1,200 words anchor; 200-400 words mini)
- Pull quote must be marked "approved" in the source story file
- Customer logo + photo permissions confirmed before publish
- Industry / region labeling conventions]

## Output schema

[Instructions:
The structured contract for this asset's JSON output. This prose section is the home for production schema. Declare the parts that hold across every variant of this asset:

- **Metadata** — the head fields the CMS consumes: `title`/headline, customer name, industry and region (controlled vocabularies), and `customer_logo_alt` where the CMS requires it for accessibility. State the destination the metadata targets (the customers-section CMS).
- **Arrays** — optional repeatable groups the consumer iterates; declare the item shape, not instances. `metrics` is the group of outcome objects (`{label, value, context}`) — or flat strings where the CMS expects them.

Examples:
- Head: `title`/headline, customer name, `industry`, `region` (controlled vocabularies), `customer_logo_alt` (where required for accessibility)
- Arrays: `metrics` (`{label, value, context}` or flat strings)

Body keys are NOT declared here. They vary by editorial intent and are defined per variant, annotated on each variant's Structure section. The envelope owns the invariant head; the variant owns the body.]

[Tips:
- Declare only what the destination actually consumes — don't mirror an exhaustive CMS field list.
- Keep the metadata keys consistent with the {keys} your variant Structures assume.
- Pin the controlled vocabularies (industries, regions) so values stay consistent across stories.]

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`.

[Instructions: Populate one row per file in `variants/` when authoring — agents treat this table as the authoritative variant index. `Load When` is a compact trigger phrase (a few words, styled like the Pillars/Collections `Load When` columns in MESSAGE.md) that lets the agent choose the right variant file before loading it — not the 2-4 sentence prose that previously lived in each variant's `## When to use` section.

Examples for this asset:
- anchor-case-study — Flagship reference customer, full narrative with metrics
- mini-story — Short proof snippet for logo wall or deck
- video-transcript-companion — Written companion to a recorded testimonial
- vertical-spotlight — Industry/segment-framed story for a named vertical]

| Variant | File | Description | Load When |
|---------|------|-------------|-----------|
|         |      |             |           |
