---
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

## Output

The deliverable is a markdown document. The body follows the selected variant's Structure section — one heading per section, in order, with citations placed per the Conventions.

[Instructions:
Declare the frontmatter the gated-content platform (HubSpot / Marketo) and PDF render consume as a literal block like the one below — one line per field, with an inline comment stating the rule. A variant may note additional fields only it needs (e.g., a research variant's `survey_n` / `survey_date`; a benchmark's `peer_set`) in its own file. If ungated and self-hosted with no downstream tool, delete the block and state that the output is body-only.]

```markdown
---
title:             # paper title as rendered on cover and landing page
author:            # byline; person or team
form_id:           # gating form; drop for web-only
landing_page_url:  # the gated download destination; drop for web-only
---
```

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`. 

[Instructions: Populate one row per file in `variants/` — agents treat this table as the authoritative variant index. `Load When` is a compact trigger phrase (a few words, styled like the Pillars/Collections `Load When` columns in MESSAGE.md) that lets the agent choose the right variant before loading it.

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
