---
status: active
default-variant: ""
---

# Slide Deck

[Instructions:
The slide-based presentation asset — a narrated sequence of slides a rep or executive presents live, where the story unfolds slide by slide rather than as a single page of prose. Covers first-call pitch decks and other live presentation formats.

This file carries the company conventions that hold across every deck variant — one-idea-per-slide, narrative spine, headline-as-claim, speaker-notes discipline, proof routing, persona-binding, naming accuracy. Per-type slide sequence, voice, and presenter conventions live in each variant under `variants/`.]

## Conventions

[Instructions:
Specify the company's deck-wide standards that hold across variants:
- One idea per slide: a single point — a headline that states it + minimal support; depth lives in speaker notes, not on the slide
- Narrative spine, not a feature tour: the deck tells one story end to end; document the canonical spine explicitly and ordered (e.g., problem → why it persists → reframe → how we do it → proof → path) and the rule not to reorder it into a product catalog — a vague spine produces feature-tour decks
- Headline slides: each heading states the takeaway as a claim ("You can't protect what no tool confirms exists"), not a label ("Asset Visibility"); skimming the headings alone should convey the argument
- Speaker notes carry the talk: every slide pairs sparse on-slide content with notes — what the presenter actually says (nuance, proof framing, transitions)
- Proof inline, at the moment it's earned: a named quote / analyst line sits on the slide where its claim is made, not in an end-of-deck proof dump
- Persona-bound: one persona per deck; match altitude to the single target reader
- Messaging-grounded: every claim / differentiator / proof traces to the messaging house (`pitch.md`, `position.md`, `portfolio.md`, `proof.md`) — introduce no positioning not supported there
- Naming discipline: match the MESSAGE.md Glossary exactly (preferred terms over banned synonyms; excluded / roadmap terms)
- Competitive framing rules that recur across decks (e.g., position alongside adjacent categories, never against)
- Proof / analyst routing: which analyst recognitions and customer references are cleared for which audiences — name which go to executive vs. practitioner — and where quantitative outcomes come from (`proof.md` ranges — never invent precision)]

## Output

The deliverable is a markdown document. The body is the deck: one heading per slide, in the order the selected variant's Structure section defines. Under each heading, the sparse on-slide content (a short statement, ≤4 bullets, or a stat / quote), followed by a `Speaker notes:` block carrying what the presenter says.

[Instructions:
Declare the frontmatter the slide renderer / design system consumes as a literal block like the one below — one line per field, with an inline comment stating the rule. A variant may note additional fields only it needs (e.g., a partner deck's `partner_name`) in its own file. If nothing downstream consumes this asset, delete the block and state that the output is body-only.]

```markdown
---
title:      # at the persona's altitude — no product names for executive personas
subtitle:   # one-line frame
persona:    # the single target reader
cta_label:  # the specific next step, not generic "contact sales"
cta_url:    # where the closing slide drives
---
```

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`. 

[Instructions: Populate one row per file in `variants/` — agents treat this table as the authoritative variant index. `Load When` is a compact trigger phrase (a few words, styled like the Pillars/Collections `Load When` columns in MESSAGE.md) that lets the agent choose the right variant before loading it.

Examples for this asset:
- first-call — Booked first meeting, problem-to-platform in 15-20 min
- partner — Joint go-to-market, co-branded deck
- executive-briefing — Exec/board audience, outcomes only
- technical-deep-dive — Technical evaluator, architecture depth]

| Variant | File | Description | Load When |
|---------|------|-------------|-----------|
|         |      |             |           |
