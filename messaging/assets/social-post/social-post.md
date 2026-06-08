---
slug: social-post
status: active
default-variant: ""
---

# Social Post

[Instructions:
Short-form social post for any platform — LinkedIn, Twitter/X, Reddit, threads. Used for brand voice, thought leadership, campaign distribution, executive amplification, etc. 

This file carries the company conventions that hold across every social-post variant — hashtag policy, link discipline, mention policy, image/alt conventions. Structure and CTA conventions live in each variant under `variants/` since each platform has its own form constraints (LinkedIn's "see more" truncation, Twitter's char limit, Reddit's title vs. body, thread sequencing).]

## Conventions

[Instructions:
Specify the company's social-wide standards that hold across variants:
- No hashtags or links in first message
- Mention policy: reserved for relevant individuals; no mass-tag spam
- Quote-share rule: 1-2 sentences of original framing before the share
- Attribution policy when reposting customer or analyst content]

## Frontmatter requirements

[Instructions:
`mentions` is an array of platform-prefixed handle strings (e.g., LinkedIn `["company/acme", "in/jdoe"]`; Twitter/X `["@acme"]`; Reddit `["u/jdoe"]`). `media_url` supports a single image or video; for multi-image carousels or threads, extend the schema (`media_urls`, `thread_sequence`) per variant requirements. Document any publishing automation (Buffer, Hootsuite, native LinkedIn API, Twitter API).]

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`.

[Instructions: Populate one row per variant]

| Variant | File | Description |
|---------|------|-------------|
|         |      |             |
