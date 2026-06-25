---
slug: one-pager
status: active
default-variant: ""
---

# One-Pager

[Instructions:
Single-page leave-behind reference asset. Used for sales pitches, competitive battlecards, product datasheets, partner overviews, executive briefs — anything that must fit on one printed page and be self-contained enough for a champion to forward without explanation. 

This file carries the company conventions that hold across every one-pager variant — page-cap discipline, design system constraints, persona-specific rule, brand styling. Structure and CTA conventions live in each variant under `variants/` since they vary significantly by editorial intent (a sales pitch leads with pain; a datasheet leads with capability tables; a battlecard leads with competitive contrast).]

## Conventions

[Instructions:
Specify the company's one-pager-wide standards that hold across variants:
- Hard page cap (e.g., must fit one printed page — typically ≤400 words; design templates enforce)
- Design system / PDF generation tool (Figma → PDF, Notion, custom designer, etc.) — name the canonical template
- Persona-bound rule: one persona per one-pager; multi-persona pages dilute
- Champion-forwardable rule: a director receives this and can forward to their CISO without explaining
- Brand styling constraints (color tokens, logo placement, footer)
- File naming convention for the rendered PDF]

## Output schema

[Instructions:
The structured contract for this asset's JSON output. This prose section is the home for production schema. Declare the parts that hold across every variant of this asset:

- **Metadata** — the design/render head: `title`, `template_id` (Figma component or PDF generator template), `page_size` (Letter, A4), `brand_theme` (light, dark, partner co-brand), `output_format` (PDF, web, both). State the destination the metadata targets (the design system / PDF generator — no CMS by default).
- **Arrays** — optional repeatable groups the consumer iterates; declare the item shape, not instances. None by default — variant-specific groups (a datasheet's `spec_table` rows, a battlecard's objection list) are declared on the relevant variant.

Examples:
- `template_id` (Figma component or PDF generator template), `page_size` (Letter, A4), `brand_theme` (light, dark, partner co-brand), `output_format` (PDF, web, both)
- Variant-specific: a battlecard's `competitor_name`, a datasheet's `spec_table`

Body keys are NOT declared here. They vary by editorial intent and are defined per variant, annotated on each variant's Structure section. The envelope owns the invariant head; the variant owns the body.]

[Tips:
- Declare only what the renderer actually consumes — don't mirror an exhaustive field list.
- Keep the metadata keys consistent with the {keys} your variant Structures assume.
- This renders to a fixed single page — note any field length caps the template enforces.]

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`.

[Instructions: Populate one row per file in `variants/` when authoring — agents treat this table as the authoritative variant index]

| Variant | File | Description |
|---------|------|-------------|
|         |      |             |
