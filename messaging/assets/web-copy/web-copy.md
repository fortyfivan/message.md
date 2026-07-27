---
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
- Naming discipline: the website is the most terminology-sensitive surface — match the Glossary exactly; list the canonical product names and the banned synonyms, not just "follow the glossary"
- CTA altitude defaults: set the default primary-CTA register for the typical champion, and note when exec-targeted pages flex up (executive briefing / peer reference)
- Length bands per variant, with specific numbers (e.g., product 800–1,200; solution 800–1,400; comparison 900–1,600; topic 1,800–3,500 words)]

## Output

The deliverable is a markdown document. The body follows the selected variant's Structure section — one heading per page section, in order; the headings are the page's H1/H2 skeleton.

[Instructions:
If a downstream tool consumes this asset (the marketing-site CMS), declare the frontmatter it needs as a literal block like the one below — one line per field, with an inline comment stating the rule. Per-variant SEO patterns belong in the variant (a comparison `seo_title` includes both company names; a topic `seo_title` leads with the primary keyword). If nothing downstream consumes this asset, delete the block and state that the output is body-only.]

```markdown
---
title:            # page title; the H1 lives in the body
seo_title:        # front-load the primary keyword
seo_description:  # search snippet
og_image_url:     # social share image
---
```

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`. A variant with a sibling `variants/[slug].html` file uses it as the render template when producing HTML output; the template loads only at render time.

[Instructions: Populate one row per file in `variants/` — agents treat this table as the authoritative variant index. `Load When` is a compact trigger phrase (a few words, styled like the Pillars/Collections `Load When` columns in MESSAGE.md) that lets the agent choose the right variant before loading it.

Examples for this asset:
- product-page — Maps to a specific product or platform service
- solution-page — Maps to a GTM solution or use case
- comparison-page — Commercial-intent "[us] vs [competitor]" query
- topic-page — Informational-intent "what is X" query
- landing-page — Single-offer conversion capture]

| Variant | File | Description | Load When |
|---------|------|-------------|-----------|
|         |      |             |           |
