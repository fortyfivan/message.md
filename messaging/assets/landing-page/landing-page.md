---
slug: landing-page
status: active
default-variant: ""
---

# Landing Page

[Instructions:
Single-purpose conversion page used for campaign destinations, product pages, gated assets, webinar registrations, event pages, partner co-marketing pages — anything that turns intent into a single conversion action. 

This file carries the company conventions that hold across every landing-page variant — word count caps, hero headline derivation, CMS section structure. Structure and CTA conventions live in each variant under `variants/` since they vary by editorial intent (a product page leads with capability; a webinar landing page leads with date/speaker; an event page leads with format/location; a gated asset leads with the offer).]

## Conventions

[Instructions:
Specify the company's landing-page standards that hold across variants:
- Single goal per page (one CTA, no competing actions) — applies to every variant
- Above-the-fold word count cap (e.g., ≤400 words)
- Full-page word count cap (e.g., ≤800 words)
- Lead-with rule (outcome vs. feature) — company-wide stance
- Hero headline derivation rule (from the persona's altitude)
- Image / video usage norms]

## Frontmatter requirements

[Instructions:
Document what the publishing destination expects. If the CMS uses structured sections, populate `sections` as an array of block objects (`{type, heading, body, image_url, ...}`). For flat-HTML CMSs, replace with a single `body` key.

Common additions for any variant: `og_image_url`, `form_id` (for gated pages), `pardot_form_handler_url`, `marketo_form_id`.

Variant-specific fields added per-variant during `/design asset landing-page --add-variant`:
- webinar / event: `event_date`, `event_time`, `event_duration`, `speakers` (array), `agenda` (array), `registration_cta_url`, `on_demand_cta_url`, webinar platform integration fields (Zoom, ON24, Demio)
- gated-asset: `asset_download_url`, `gated_form_id`
- product-page: `product_slug`, `feature_list` (array)]

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`.

[Instructions: Populate one row per file in `variants/` when authoring — agents treat this table as the authoritative variant index]

| Variant | File | Description |
|---------|------|-------------|
|         |      |             |
