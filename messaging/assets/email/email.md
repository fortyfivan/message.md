---
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
- Preheader rule (extends subject; treat as second headline; never repeats subject)
- Sender identity (named human vs. generic "team@"; signature conventions)
- Sequence-position-implicit rule (don't write "Email 3 of 5" in body)
- One asset reference per email (multiple links dilute conversion)]

## Output

The deliverable is a markdown document. The body is the email itself, following the selected variant's Structure section in order.

[Instructions:
Declare the frontmatter the sending platform consumes (Marketo, HubSpot, Outreach, etc.) as a literal block like the one below — one line per field, with an inline comment stating the rule, including character limits. Declare only what the platform actually consumes. Where the platform injects merge tokens (liquid/handlebars) into subject or body, the output carries the token, not the resolved value. If nothing downstream consumes this asset, delete the block and state that the output is body-only.]

```markdown
---
subject:       # ≤N characters; no sales clichés
preheader:     # extends the subject; never repeats it
sender_name:   # named human; omit if platform-resolved
sender_title:  # omit if platform-resolved
cta_url:       # single destination; platform appends tracking params
---
```

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`. A variant with a sibling `variants/[slug].html` file uses it as the render template when producing HTML output; the template loads only at render time.

[Instructions: Populate one row per file in `variants/` — agents treat this table as the authoritative variant index. `Load When` is a compact trigger phrase (a few words, styled like the Pillars/Collections `Load When` columns in MESSAGE.md) that lets the agent choose the right variant before loading it.

Examples for this asset:
- nurture — Lead in active consideration, already engaged
- outbound — Cold prospect, trigger event or persona-pain hook
- promo — Time-bound offer, event invite, or launch
- lifecycle — Renewal, usage milestone, anniversary, churn risk
- transactional-companion — Operational message tied to product event]

| Variant | File | Description | Load When |
|---------|------|-------------|-----------|
|         |      |             |           |
