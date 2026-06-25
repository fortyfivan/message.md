---
slug: email
status: active
default-variant: ""
---

# Email

[Instructions:
Email asset — nurture sequences, cold outbound, promotional sends, lifecycle messages, etc. 

This file carries the company conventions that hold across every email variant — subject-line policy, sender identity, deliverability discipline, sequence-position-implicit rule. Structure and CTA conventions live in each variant under `variants/` since they vary significantly by editorial intent.]

## Conventions

[Instructions:
Specify the company's email-wide standards that hold across variants:
- Subject line policy (e.g., ≤8 words for nurture, ≤6 words for outbound, no sales clichés like "circling back" / "touching base" / "just following up")
- Preheader rule (extends subject; treats as second headline; never repeats subject)
- Sender identity (named human vs. generic "team@"; signature conventions)
- Sequence-position-implicit rule (don't write "Email 3 of 5" in body)
- One asset reference per email (multiple links dilute conversion)]

## Output schema

[Instructions:
The structured contract for this asset's JSON output. This prose section is the home for production schema. Declare the parts that hold across every variant of this asset:

- **Metadata** — the head fields the sending platform consumes: `subject`, `preheader`, and sender identity (`sender_name`/`sender_title`, or platform-resolved). Note format constraints (subject/preheader character limits) and any routing hints (e.g., `segment`). State the destination the metadata targets (the marketing-automation or sales-engagement platform — Marketo, HubSpot, Outreach, etc.).
- **Arrays** — optional repeatable groups the consumer iterates; declare the item shape, not instances. A single email has none — omit.

Examples:
- Marketo / Pardot: `program`, `step_number`, `program_token`
- HubSpot: `workflow_id`, `subscription_type`
- Outreach / Salesloft / Apollo: liquid/handlebars merge tokens in `subject`/body; `cta_url` carries tracking params per platform
- Routing / sender: `segment` (a hint — replace or remove per platform); `sender_name`/`sender_title` (omit if platform-resolved)

Body keys are NOT declared here. They vary by editorial intent and are defined per variant, annotated on each variant's Structure section. The envelope owns the invariant head; the variant owns the body.]

[Tips:
- Declare only what the destination actually consumes — don't mirror an exhaustive platform field list.
- Keep the metadata keys consistent with the {keys} your variant Structures assume.
- Where the platform injects merge tokens into `subject`/body, the contract carries the token, not the resolved value.]

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`.

[Instructions: Populate one row per file in `variants/` when authoring — agents treat this table as the authoritative variant index]

| Variant | File | Description |
|---------|------|-------------|
|         |      |             |
