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

## Output schema

[Instructions:
The structured contract for this asset's JSON output. This prose section is the home for production schema. Declare the parts that hold across every variant of this asset:

- **Metadata** — the page head the CMS consumes: page `title`, `og_image_url`, and `form_id` for gated pages. Note format constraints and ISO 8601 dates. State the destination the metadata targets (the marketing-site CMS).
- **Arrays** — optional repeatable groups the consumer iterates; declare the item shape, not instances. `sections` is the ordered group of block objects (`{type, heading, body, image_url, …}`) where the CMS renders structured sections; the variant's Structure defines the block sequence (for flat-HTML CMSs the body collapses to a single body key, declared per variant). Variant-specific groups (a webinar's `speakers`/`agenda`, a product page's `feature_list`) are declared on the relevant variant.

Examples:
- Any variant: `og_image_url`, `form_id`, `pardot_form_handler_url`, `marketo_form_id`
- Webinar / event: `event_date`, `event_time`, `event_duration`, `speakers` (array), `agenda` (array), `registration_cta_url`, `on_demand_cta_url`, webinar-platform fields (Zoom, ON24, Demio)
- Gated-asset: `asset_download_url`, `gated_form_id`
- Product-page: `product_slug`, `feature_list` (array)

Body keys are NOT declared here. They vary by editorial intent and are defined per variant, annotated on each variant's Structure section. The envelope owns the invariant head; the variant owns the body.]

[Tips:
- Declare only what the destination actually consumes — don't mirror an exhaustive CMS field list.
- Keep the metadata keys consistent with the `Key` column in your variant's Structure table.
- For SEO/OG fields, note whether the CMS derives meta from the title or wants `og_image_url`/meta explicit.]

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`.

[Instructions: Populate one row per file in `variants/` when authoring — agents treat this table as the authoritative variant index. `Load When` is a compact trigger phrase (a few words, styled like the Pillars/Collections `Load When` columns in MESSAGE.md) that lets the agent choose the right variant file before loading it — not the 2-4 sentence prose that previously lived in each variant's `## When to use` section.

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
