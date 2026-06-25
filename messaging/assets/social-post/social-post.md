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

## Output schema

[Instructions:
The structured contract for this asset's JSON output. This prose section is the home for production schema. Declare the parts that hold across every variant of this asset:

- **Metadata** — the post head the publishing tool consumes: target `channel`/platform, and the post text head where the platform separates it (e.g., a Reddit `title` distinct from body) plus a single `media_url`. Note per-platform character limits as format constraints. State the destination the metadata targets (the social publishing tool — Buffer, Hootsuite, native LinkedIn / Twitter API).
- **Arrays** — optional repeatable groups the consumer iterates; declare the item shape, not instances. `mentions` is the group of platform-prefixed handle strings (LinkedIn `["company/acme", "in/jdoe"]`; Twitter/X `["@acme"]`; Reddit `["u/jdoe"]`). Thread / carousel variants add a `media_urls` or `thread_sequence` group, declared on the variant.

Examples:
- Head: `channel`, the post text head (Reddit `title` vs. body), `media_url` (single image/video)
- Arrays: `mentions` (platform-prefixed handles); thread / carousel `media_urls`, `thread_sequence`
- Automation: Buffer, Hootsuite, native LinkedIn API, Twitter API

Body keys are NOT declared here. They vary by editorial intent and are defined per variant, annotated on each variant's Structure section. The envelope owns the invariant head; the variant owns the body.]

[Tips:
- Declare only what the destination actually consumes — don't mirror an exhaustive field list.
- Keep the metadata keys consistent with the {keys} your variant Structures assume.
- Note each platform's hard character limit so the contract can be validated before publish.]

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`.

[Instructions: Populate one row per file in `variants/` when authoring — agents treat this table as the authoritative variant index]

| Variant | File | Description |
|---------|------|-------------|
|         |      |             |
