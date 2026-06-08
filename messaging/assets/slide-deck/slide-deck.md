---
slug: slide-deck
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
- Narrative spine, not a feature tour: the deck tells one story end to end; document the canonical spine (e.g., problem → why it persists → reframe → how we do it → proof → path) and the rule not to reorder it into a product catalog
- Headline slides: each heading states the takeaway as a claim ("You can't protect what no tool confirms exists"), not a label ("Asset Visibility"); skimming the headings alone should convey the argument
- Speaker notes carry the talk: every slide pairs sparse on-slide content with notes — what the presenter actually says (nuance, proof framing, transitions)
- Proof inline, at the moment it's earned: a named quote / analyst line sits on the slide where its claim is made, not in an end-of-deck proof dump
- Persona-bound: one persona per deck; match altitude to the single target reader
- Messaging-grounded: every claim / differentiator / proof traces to the messaging house (`pitch.md`, `position.md`, `portfolio.md`, `proof.md`) — introduce no positioning not supported there
- Naming discipline: match the `messaging/pillars/profile.md` Glossary exactly (preferred terms over banned synonyms; excluded / roadmap terms)
- Competitive framing rules that recur across decks (e.g., position alongside adjacent categories, never against)
- Proof / analyst routing: which analyst recognitions and customer references are cleared for which audiences, and where quantitative outcomes come from (`proof.md` ranges — never invent precision)]

[Tips:
- Make the narrative spine explicit and ordered; a vague spine produces feature-tour decks.
- Keep proof routing concrete — name which references go to executive vs. practitioner audiences.]

## Frontmatter requirements

[Instructions:
These are presentation documents — design-system-driven, rendered to a slide deck rather than published through a CMS. No CMS is configured by default; extend when one is set.

`slides` is the ordered array of slides. Each slide is an object: `heading` (the takeaway as a claim), `body` (sparse on-slide content — a short statement, ≤4 bullets, or a stat / quote), and `speaker_notes` (what the presenter says). A slide may carry an optional `proof` (quote / metric + attribution) or `visual` (a note on the intended chart / diagram). The variant's Structure section defines the slide sequence.

Other keys: `title` (title-slide headline at the persona's altitude — no product names where the persona is executive), `subtitle`, `persona` (the single target reader), `cta_label` (the specific next step, not generic "contact sales"), `cta_url`, `logo_url` (co-branded for partner decks). Variant-specific frontmatter (e.g., a partner deck's `partner_name`) gets added per-variant when needed.]

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`.

[Instructions: Populate one row per variant]

| Variant | File | Description |
|---------|------|-------------|
|         |      |             |
