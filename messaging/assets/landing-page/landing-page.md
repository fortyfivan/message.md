---
status: active
default-variant: ""
---

# Landing Page

[Instructions:
Single-purpose conversion page used for campaign destinations, product pages, gated assets, webinar registrations, event pages, partner co-marketing pages — anything that turns intent into a single conversion action.

This file carries the company conventions that hold across every landing-page variant — word count caps, hero headline derivation, single-goal discipline. Structure and CTA conventions live in each variant under `variants/` since they vary by editorial intent (a product page leads with capability; a webinar landing page leads with date/speaker; an event page leads with format/location; a gated asset leads with the offer).]

## Conventions

[Instructions:
Specify the company's landing-page standards that hold across variants:
- Single goal per page (one CTA, no competing actions) — applies to every variant
- Above-the-fold word count cap (e.g., ≤400 words)
- Full-page word count cap (e.g., ≤800 words)
- Lead-with rule (outcome vs. feature) — company-wide stance
- Hero headline derivation rule (from the persona's altitude)
- Image / video usage norms]

## Output

The deliverable is a markdown document. The body follows the selected variant's Structure section — one heading per page section, in order.

[Instructions:
If a downstream tool consumes this asset (the marketing-site CMS), declare the frontmatter it needs as a literal block like the one below — one line per field, with an inline comment stating the rule. A variant may note additional fields only it needs (e.g., a webinar's `event_date` and speaker list; a gated asset's `asset_download_url`) in its own file. If nothing downstream consumes this asset, delete the block and state that the output is body-only.]

```markdown
---
title:         # page title; hero headline lives in the body
seo_title:     # front-load the primary keyword
og_image_url:  # social share image
form_id:       # gated pages only; the marketing-automation form
---
```

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`. A variant with a sibling `variants/[slug].html` file uses it as the render template when producing HTML output; the template loads only at render time.

[Instructions: Populate one row per file in `variants/` — agents treat this table as the authoritative variant index. `Load When` is a compact trigger phrase (a few words, styled like the Pillars/Collections `Load When` columns in MESSAGE.md) that lets the agent choose the right variant before loading it.

Examples for this asset:
- campaign-destination — Campaign traffic, single offer
- product-page — Persistent, evergreen product overview
- webinar — Live or on-demand webinar registration
- event — Conference or field event registration
- gated-asset — Gated download (paper, guide, calculator)
- partner-co-marketing — Joint go-to-market with a partner]

| Variant | File | Description | Load When |
|---------|------|-------------|-----------|
|         |      |             |           |
