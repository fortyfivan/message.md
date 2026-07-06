---
slug: press-release
status: active
default-variant: ""
---

# Press Release

[Instructions:
Standard wire-format release for company news — product launches, funding announcements, customer wins, partnerships, executive appointments. 

This file carries the company conventions that hold across every press-release variant — the wire-format spine, AP style, quote and boilerplate rules. Structure and CTA conventions live in each variant under `variants/` since they vary by editorial intent (a funding or appointment release leads with the corporate milestone; a product launch leads with the capability; a partnership leads with the joint value and gives both parties balanced billing).]

## Conventions

[Instructions:
Specify standards that hold across variants:
- Word count target (e.g., 400-700 words)
- Style guide (e.g., AP style: numerals 10+, lowercase company verbs)
- One quote per stakeholder; quotes approved by the named speaker
- Banned superlatives in the lede ("revolutionary," "best-in-class," "next-generation")
- Boilerplate pulled verbatim from the `messaging/pillars/profile.md` boilerplate field]

## Output schema

[Instructions:
The structured contract for this asset's JSON output. This prose section is the home for production schema. Declare the parts that hold across every variant of this asset:

- **Metadata** — the wire head the destination consumes: `headline`, `subhead`, `dateline` (`CITY — Month Day, Year`), `boilerplate` (pulled verbatim from `profile.md`), and `media_contact`. Note any distribution-platform fields (e.g., PR Newswire / Business Wire `category`, `industry_codes`) and ISO 8601 machine dates even where the dateline renders long-form. State the destination the metadata targets (the wire / distribution platform or newsroom CMS).
- **Arrays** — optional repeatable groups the consumer iterates; declare the item shape, not instances. None by default — a partnership release may carry a `boilerplates` group (one item per company); declare that on the variant.

Examples:
- Head: `headline`, `subhead`, `dateline`, `boilerplate`, `media_contact`
- PR Newswire / Business Wire: `category`, `industry_codes`
- Self-distributed: the company newsroom CMS fields

Body keys are NOT declared here. They vary by editorial intent and are defined per variant, annotated on each variant's Structure section. The envelope owns the invariant head; the variant owns the body.]

[Tips:
- Declare only what the destination actually consumes — don't mirror an exhaustive distribution-platform field list.
- Keep the metadata keys consistent with the `Key` column in your variant's Structure table.
- Keep dates ISO 8601 in the contract even though the dateline renders them long-form.]

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`.

[Instructions: Populate one row per file in `variants/` when authoring — agents treat this table as the authoritative variant index. `Load When` is a compact trigger phrase (a few words, styled like the Pillars/Collections `Load When` columns in MESSAGE.md) that lets the agent choose the right variant file before loading it — not the 2-4 sentence prose that previously lived in each variant's `## When to use` section.

Examples for this asset:
- company-news — Corporate milestone (funding, exec hire, win, award)
- product-launch — New product or capability reaching GA
- partnership — Alliance, integration, or joint GTM with named partner]

| Variant | File | Description | Load When |
|---------|------|-------------|-----------|
|         |      |             |           |
