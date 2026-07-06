---
slug: web-copy
status: active
default-variant: ""
---

# Web Copy

[Instructions:
High-converting website copy — product pages, solution pages, comparison pages, topic/pillar pages, and conversion landing pages that balance positioning clarity with conversion optimization. 

This file carries the company conventions that hold across every web-copy variant — the clarity test, structure-as-content discipline, CTA-per-section rule, naming accuracy, length bands. Structure and CTA destinations live in each variant under `variants/` since they vary by intent (a product page leads with capability; a comparison page leads with contrast; a topic page leads with an educational definition).]

## Conventions

[Instructions:
Specify the company's web-wide standards that hold across variants. Web is the most constrained surface — every word competes with navigation, visuals, and the back button.
- 5-second clarity test: the reader understands the page within 5 seconds of landing; clarity beats cleverness on every variant
- Structure is content: write the headers first — H1 + H2s alone should convey the value proposition; H2s/H3s double as searchable phrases for SEO/GEO
- One CTA per page section: every scroll depth has one clear next action; don't compete with yourself
- Proof inline: quote, metric, or logo bar sits next to the claim it supports — don't defer the reader to a separate case-study page
- Persona-aware, not persona-exclusive: write to the primary buyer without alienating the technical evaluator or the forwarding champion
- Naming discipline: the website is the most terminology-sensitive surface — match the Glossary exactly (product names, first- vs. second-reference rules, preferred terms over banned synonyms)
- CTA altitude defaults: set the default primary-CTA register for the typical champion, and note when exec-targeted pages flex up (executive briefing / peer reference)
- Length bands per variant (e.g., product 800–1,200; solution 800–1,400; comparison 900–1,600; topic 1,800–3,500 words)]

[Tips:
- Be specific with word-count bands; vague guidance produces inconsistent pages.
- Keep naming rules concrete — list the canonical product names and the banned synonyms, not just "follow the glossary."]

## Output schema

[Instructions:
The structured contract for this asset's JSON output. This prose section is the home for production schema. Declare the parts that hold across every variant of this asset:

- **Metadata** — the page head the CMS consumes: page `title` and SEO (`seo_title`, `seo_description`, meta). Note that per-variant SEO patterns belong on the variant (a comparison `seo_title` includes both company names; a topic `seo_title` leads with the primary keyword). State the destination the metadata targets (the marketing-site CMS — none configured by default).
- **Arrays** — optional repeatable groups the consumer iterates; declare the item shape, not instances. `sections` is the ordered group of block objects (`{type, heading, body, image_url, …}`) where the CMS renders pages as blocks; the variant's Structure defines the block sequence (a comparison-page block may carry table data). Omit if the CMS takes flat body.

Examples:
- Head: page `title`, `seo_title`, `seo_description`, meta
- When a destination is set: `og_image_url`, `product_slug`, `feature_list`
- Per-variant SEO patterns belong on the variant (comparison `seo_title` includes both company names; topic `seo_title` leads with the primary keyword)

Body keys are NOT declared here. They vary by editorial intent and are defined per variant, annotated on each variant's Structure section. The envelope owns the invariant head; the variant owns the body.]

[Tips:
- Declare only what the destination actually consumes — don't mirror an exhaustive CMS field list.
- Keep the metadata keys consistent with the `Key` column in your variant's Structure table.
- For SEO fields, note whether the CMS derives meta from the H1/excerpt or wants them explicit.]

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`.

[Instructions: Populate one row per file in `variants/` when authoring — agents treat this table as the authoritative variant index. `Load When` is a compact trigger phrase (a few words, styled like the Pillars/Collections `Load When` columns in MESSAGE.md) that lets the agent choose the right variant file before loading it — not the 2-4 sentence prose that previously lived in each variant's `## When to use` section.

Examples for this asset:
- product-page — Maps to a specific product or platform service
- solution-page — Maps to a GTM solution or use case
- comparison-page — Commercial-intent "[us] vs [competitor]" query
- topic-page — Informational-intent "what is X" query
- landing-page — Single-offer conversion capture]

| Variant | File | Description | Load When |
|---------|------|-------------|-----------|
|         |      |             |           |
