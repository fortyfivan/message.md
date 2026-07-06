---
slug: whitepaper
status: active
default-variant: ""
---

# Whitepaper

[Instructions:
Long-form analytical content backed by primary data, methodology, citations, or strategic argument. Used for research studies, topic deep-dives, market benchmarks, point-of-view papers, analyst-style briefs, regulatory or technical guides — anything that earns authority through depth rather than brevity. 

This file carries the company conventions that hold across every whitepaper variant — citation discipline, attribution requirements, gating model, author credibility convention. Structure and CTA conventions live in each variant under `variants/` since they vary by editorial intent (a research study leads with methodology; a topic paper leads with the thesis; a benchmark leads with the data; a point-of-view paper leads with the contrarian argument).]

## Conventions

[Instructions:
Specify the company's whitepaper-wide standards that hold across variants:
- Word count bands (e.g., 3,000-10,000 words depending on variant scope)
- Citation style (footnote on same page as claim; no orphan stats)
- Every quantitative claim attributes a source; every directional claim names its evidence basis
- Designed for gated download; supports both PDF and web rendering
- Author byline + contact conventions
- Methodology disclosure rule (when applicable to variant)]

## Output schema

[Instructions:
The structured contract for this asset's JSON output. This prose section is the home for production schema. Declare the parts that hold across every variant of this asset:

- **Metadata** — the gated-PDF + landing head: `title`, `download_cta_label`/`download_cta_url` for gated (drop for web-only), and gating fields (`form_id`, `landing_page_url`). State the destination the metadata targets (the gated-content platform — HubSpot / Marketo — plus the PDF render).
- **Arrays** — optional repeatable groups the consumer iterates; declare the item shape, not instances. None by default — variant-specific data groups (a research variant's tables keyed by `survey_n`/`survey_date`; a benchmark's `peer_set`) are declared on the relevant variant.

Examples:
- Gated: `download_cta_label`, `download_cta_url`, `form_id`, `landing_page_url` (drop the CTA fields for web-only)
- Variant-specific: a research variant's `survey_n`, `survey_date`; a benchmark's `peer_set`

Body keys are NOT declared here. They vary by editorial intent and are defined per variant, annotated on each variant's Structure section. The envelope owns the invariant head; the variant owns the body.]

[Tips:
- Declare only what the destination actually consumes — don't mirror an exhaustive field list.
- Keep the metadata keys consistent with the `Key` column in your variant's Structure table.
- For the landing page's SEO fields, note whether the CMS derives them from the title or wants them explicit.]

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`.

[Instructions: Populate one row per file in `variants/` when authoring — agents treat this table as the authoritative variant index. `Load When` is a compact trigger phrase (a few words, styled like the Pillars/Collections `Load When` columns in MESSAGE.md) that lets the agent choose the right variant file before loading it — not the 2-4 sentence prose that previously lived in each variant's `## When to use` section.

Examples for this asset:
- research — Primary research with novel data
- topic — Strategic argument or category deep dive
- benchmark — Comparative data across vendors or time
- point-of-view — Contrarian stance backed by evidence
- analyst-brief — Analyst-style format (Gartner/Forrester/IDC)
- technical-guide — Standards, compliance, or technical reference]

| Variant | File | Description | Load When |
|---------|------|-------------|-----------|
|         |      |             |           |
