---
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
- Industry / region labeling conventions (pin the controlled vocabularies so values stay consistent across stories)]

## Output

The deliverable is a markdown document. The body follows the selected variant's Structure section — one heading per section, in order. Outcome metrics live in the body, in the section the variant's Structure assigns them.

[Instructions:
If a downstream tool consumes this asset (the customers-section CMS), declare the frontmatter it needs as a literal block like the one below — one line per field, with an inline comment stating the rule. Declare only what the destination actually consumes. If nothing downstream consumes this asset, delete the block and state that the output is body-only.]

```markdown
---
title:       # story headline; outcome-led, not "Customer X case study"
customer:    # customer name as approved for publication
industry:    # controlled vocabulary — list the allowed values here
region:      # controlled vocabulary — list the allowed values here
---
```

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`. A variant with a sibling `variants/[slug].html` file uses it as the render template when producing HTML output; the template loads only at render time.

[Instructions: Populate one row per file in `variants/` — agents treat this table as the authoritative variant index. `Load When` is a compact trigger phrase (a few words, styled like the Pillars/Collections `Load When` columns in MESSAGE.md) that lets the agent choose the right variant before loading it.

Examples for this asset:
- anchor-case-study — Flagship reference customer, full narrative with metrics
- mini-story — Short proof snippet for logo wall or deck
- video-transcript-companion — Written companion to a recorded testimonial
- vertical-spotlight — Industry/segment-framed story for a named vertical]

| Variant | File | Description | Load When |
|---------|------|-------------|-----------|
|         |      |             |           |
