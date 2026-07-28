---
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

## Output

The deliverable is a markdown document. The body is the post text itself, following the selected variant's Structure section — the variant carries the platform's form constraints (character limits, truncation points, thread sequencing). By default the output is body-only: the variant already identifies the platform.

[Instructions:
If a publishing tool consumes this asset (Buffer, Hootsuite, a native platform API), declare the frontmatter it needs as a literal block — one line per field, with an inline comment stating the rule, e.g.:

```markdown
---
title:      # Reddit only — the post title, separate from body
media_url:  # single image/video attachment
mentions:   # platform-prefixed handles, e.g. ["in/jdoe"] / ["@acme"] / ["u/jdoe"]
---
```

If no publishing tool consumes it, omit the block.]

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`. 

[Instructions: Populate one row per file in `variants/` — agents treat this table as the authoritative variant index. `Load When` is a compact trigger phrase (a few words, styled like the Pillars/Collections `Load When` columns in MESSAGE.md) that lets the agent choose the right variant before loading it.

Examples for this asset:
- linkedin — Long-form prose, professional audience
- twitter-x-post — Punchy statement, ≤280 chars, real-time
- twitter-x-thread — Multi-part narrative or breakdown
- reddit — Practitioner community expecting discussion]

| Variant | File | Description | Load When |
|---------|------|-------------|-----------|
|         |      |             |           |
