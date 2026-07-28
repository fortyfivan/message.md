---
status: active
default-variant: ""
---

# Blog Post

[Instructions:
The canonical long-form editorial format for the company.

This file carries the company conventions that hold across every blog variant — length norms, naming discipline, platform quirks. Structure and CTA conventions live in each variant under `variants/`, since both genuinely vary by editorial intent.]

## Conventions

[Instructions:
The company's blog-wide standards that hold across variants — only the non-obvious, company-specific norms an agent couldn't infer from good general writing. Examples:
- Length bands by variant (e.g., 800-1,500 words standard; 1,500-2,500 anchor)
- H1 handling (set by frontmatter vs. in body)
- Image cadence (e.g., one image per ~400 words)
- Naming discipline (preferred terms when describing the product space)
- Voice and tone notes specific to blog (vs. other formats)

Be specific about word counts — vague guidance leads to inconsistent output. Variant-specific length adjustments belong in the variant's Structure section, not here.]

## Output

The deliverable is a markdown document. The body follows the selected variant's Structure section — one heading per section, in order.

[Instructions:
If a downstream tool consumes this asset (the blog CMS), declare the frontmatter it needs as a literal block like the one below — one line per field, with an inline comment stating the rule. Declare only what the destination actually consumes, and note controlled vocabularies and format constraints in the comments. If nothing downstream consumes this asset, delete the block and state that the output is body-only.]

```markdown
---
title:            # rendered H1; not repeated in the body
slug:             # lowercase, hyphen-delimited
excerpt:          # 1-2 sentence teaser for listing pages
author:           # person or team byline
seo_title:        # may differ from title; front-load the primary keyword
seo_description:  # search snippet
categories: []    # controlled vocabulary — list the allowed values here
tags: []          # free-form; reuse existing tags over near-duplicates
---
```

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`.

[Instructions: Populate one row per file in `variants/` — agents treat this table as the authoritative variant index. `Load When` is a compact trigger phrase (a few words, styled like the Pillars/Collections `Load When` columns in MESSAGE.md) that lets the agent choose the right variant before loading it.

Examples for this asset:
- use-case — Customer pain is acute and named
- thought-leadership — Category inflection or emerging trend
- product-announcement — New feature or product update
- tactical-guide — Operator-focused tactical walkthrough]

| Variant | File | Description | Load When |
|---------|------|-------------|-----------|
|         |      |             |           |
