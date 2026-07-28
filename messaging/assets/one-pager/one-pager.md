---
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
- Hard page cap (e.g., must fit one printed page — typically ≤400 words; design templates enforce; note any field length caps the template enforces)
- Design system / PDF generation tool (Figma → PDF, Notion, custom designer, etc.) — name the canonical template
- Persona-bound rule: one persona per one-pager; multi-persona pages dilute
- Champion-forwardable rule: a director receives this and can forward to their CISO without explaining
- Brand styling constraints (color tokens, logo placement, footer)
- File naming convention for the rendered PDF]

## Output

The deliverable is a markdown document. The body follows the selected variant's Structure section — one heading per section, in order, sized to fit the one-page cap.

[Instructions:
Declare the frontmatter the design system / PDF generator consumes as a literal block like the one below — one line per field, with an inline comment stating the rule. A variant may note additional fields only it needs (e.g., a battlecard's `competitor`) in its own file. If nothing downstream consumes this asset, delete the block and state that the output is body-only.]

```markdown
---
title:        # at the persona's altitude
template_id:  # the canonical design template (Figma component, PDF generator)
brand_theme:  # light / dark / partner co-brand
---
```

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`. 

[Instructions: Populate one row per file in `variants/` — agents treat this table as the authoritative variant index. `Load When` is a compact trigger phrase (a few words, styled like the Pillars/Collections `Load When` columns in MESSAGE.md) that lets the agent choose the right variant before loading it.

Examples for this asset:
- sales — Champion needs an internal pitch leave-behind
- battlecard — Competitive, head-to-head selection moment
- datasheet — Technical evaluator needs capability + spec reference
- partner-overview — Joint solution needs co-branded leave-behind
- executive-brief — Executive or board-level summary]

| Variant | File | Description | Load When |
|---------|------|-------------|-----------|
|         |      |             |           |
