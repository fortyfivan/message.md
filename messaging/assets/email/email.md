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

## Frontmatter requirements

[Instructions:
Document fields the marketing-automation or sales-engagement platform expects. Common patterns:
- Marketo / Pardot: `program`, `step_number`, `program_token`
- HubSpot: `workflow_id`, `subscription_type`
- Outreach / Salesloft / Apollo: liquid/handlebars merge tokens in `subject` and `body` strings; `cta_url` carries tracking params per platform
- `segment` is a routing hint; replace or remove based on the platform
- `sender_name`/`sender_title` may be platform-resolved (omit if so)]

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`.

[Instructions: Populate one row per variant]

| Variant | File | Description |
|---------|------|-------------|
|         |      |             |
