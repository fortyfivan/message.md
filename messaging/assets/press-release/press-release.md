---
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
- Boilerplate pulled verbatim from the `messaging/pillars/profile.md` boilerplate field — it renders as the closing body section]

## Output

The deliverable is a markdown document. The body follows the selected variant's Structure section — the wire-format spine in order, closing with the boilerplate section.

[Instructions:
Declare the frontmatter the distribution destination consumes (wire platform or newsroom CMS) as a literal block like the one below — one line per field, with an inline comment stating the rule. Add distribution-platform fields (e.g., PR Newswire / Business Wire `category`, `industry_codes`) only if the platform requires them. If self-distributed with no CMS, delete the block and state that the output is body-only.]

```markdown
---
headline:       # AP style; no banned superlatives
subhead:        # one sentence extending the headline
dateline:       # CITY — Month Day, Year
media_contact:  # name, title, email
---
```

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`. 

[Instructions: Populate one row per file in `variants/` — agents treat this table as the authoritative variant index. `Load When` is a compact trigger phrase (a few words, styled like the Pillars/Collections `Load When` columns in MESSAGE.md) that lets the agent choose the right variant before loading it.

Examples for this asset:
- company-news — Corporate milestone (funding, exec hire, win, award)
- product-launch — New product or capability reaching GA
- partnership — Alliance, integration, or joint GTM with named partner]

| Variant | File | Description | Load When |
|---------|------|-------------|-----------|
|         |      |             |           |
