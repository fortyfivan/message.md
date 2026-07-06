---
slug: blog-post
status: active
default-variant: ""
---

# Blog Post

[Instructions:
The canonical long-form editorial format for the company.

This file carries the company conventions that hold across every blog variant — length norms, CMS quirks, image cadence, frontmatter requirements. Structure and CTA conventions live in each variant under `variants/`, since both genuinely vary by editorial intent.]

## Conventions

[Instructions:
Specify the company's blog-wide standards that hold across variants. Examples:
- Length bands (e.g., 800-1,500 words standard; 1,500-2,500 anchor; 600-900 short-form)
- H1 handling (set by frontmatter vs. in body)
- Image cadence (e.g., one image per ~400 words)
- Quote attribution rules
- Sign-off / author byline conventions
- Voice and tone notes specific to blog (vs. other formats)]

[Tips:
- Be specific about word counts; vague guidance leads to inconsistent output
- Note any platform-specific quirks (e.g., HubSpot character limits, WordPress excerpt fields)
- Variant-specific length adjustments belong in the variant's Structure section, not here]

## Output schema

[Instructions:
The structured contract for this asset's JSON output. This prose section is the home for production schema. Declare the parts that hold across every variant of this asset:

- **Metadata** — the head/publishing fields the blog CMS consumes: `title`, `slug`, `excerpt`, author byline, SEO (`seo_title`, `seo_description`), and where the destination needs them `published_date` and `canonical_url`. Note controlled vocabularies (e.g., the fixed set of allowed categories) and format constraints (slug casing, ISO 8601 dates). State the destination the metadata targets (the blog CMS).
- **Arrays** — optional repeatable groups the consumer iterates; declare the item shape, not instances. A standard post has none — `categories`/`tags` are flat metadata lists, not iterated item groups; omit unless the CMS models a repeatable block.

Examples:
- Core content: `title`, `slug`, `excerpt`, `author`, and — where the destination needs them — `published_date`, `canonical_url`
- SEO: `seo_title`, `seo_description` (or CMS-derived from title/excerpt)
- Controlled vocab: the fixed `categories` list; `tags`]

[Tips:
- Declare only what the destination actually consumes — don't mirror an exhaustive CMS field list.
- Keep the metadata keys consistent with the {keys} your variant Structures assume.
- For SEO fields, note whether the CMS derives `seo_title`/`seo_description` from title/excerpt or wants them explicit.]

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`.

[Instructions: Populate one row per file in `variants/` when authoring — agents treat this table as the authoritative variant index. `Load When` is a compact trigger phrase (a few words, styled like the Pillars/Collections `Load When` columns in MESSAGE.md) that lets the agent choose the right variant file before loading it — not the 2-4 sentence prose that previously lived in each variant's `## When to use` section.

Examples for this asset:
- use-case — Customer pain is acute and named
- thought-leadership — Category inflection or emerging trend
- product-announcement — New feature or product update
- tactical-guide — Operator-focused tactical walkthrough]

| Variant | File | Description | Load When |
|---------|------|-------------|-----------|
|         |      |             |           |
