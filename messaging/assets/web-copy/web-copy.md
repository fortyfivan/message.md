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

## Frontmatter requirements

[Instructions:
Document what the publishing destination expects. If the CMS renders pages as ordered blocks, populate `sections` as an array of block objects (`{type, heading, body, image_url, ...}`); the per-variant Structure section defines the block sequence. A comparison-page section block may carry table data.

`sections` renders as an ordered array of blocks. No CMS is configured by default — extend frontmatter (e.g., `og_image_url`, `product_slug`, `feature_list`) when a publishing destination is set. Per-variant SEO patterns belong in the variant (e.g., comparison `seo_title` includes both company names; topic `seo_title` leads with the primary keyword).]

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`.

[Instructions: Populate one row per file in `variants/` when authoring — agents treat this table as the authoritative variant index]

| Variant | File | Description |
|---------|------|-------------|
|         |      |             |
