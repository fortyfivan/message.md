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
- Naming discipline: match the MESSAGE.md Glossary exactly (preferred terms over banned synonyms; excluded / roadmap terms)
- Competitive framing rules that recur across decks (e.g., position alongside adjacent categories, never against)
- Proof / analyst routing: which analyst recognitions and customer references are cleared for which audiences, and where quantitative outcomes come from (`proof.md` ranges — never invent precision)]

[Tips:
- Make the narrative spine explicit and ordered; a vague spine produces feature-tour decks.
- Keep proof routing concrete — name which references go to executive vs. practitioner audiences.]

## Output schema

[Instructions:
The structured contract for this asset's JSON output. This prose section is the home for production schema. Declare the parts that hold across every variant of this asset:

- **Metadata** — the deck/title-slide head: `title` (at the persona's altitude — no product names where the persona is executive), `subtitle`, `persona` (the single target reader), `cta_label` (the specific next step, not generic "contact sales"), `cta_url`, and `logo_url` (co-branded decks). State the destination the metadata targets (the design system / slide renderer).
- **Arrays** — optional repeatable groups the consumer iterates; declare the item shape, not instances. `slides` is the ordered group of slide objects: `heading` (the takeaway as a claim), `body` (sparse on-slide content — a short statement, ≤4 bullets, or a stat / quote), `speaker_notes` (what the presenter says), optional `proof` (quote / metric + attribution) and `visual` (a note on the intended chart / diagram). The variant's Structure defines the slide sequence.

Examples:
- Title-slide head: `title`, `subtitle`, `persona`, `cta_label`, `cta_url`, `logo_url`
- Slide item (`slides[]`): `heading`, `body`, `speaker_notes`, optional `proof`, `visual`
- Variant-specific: a partner deck's `partner_name`

Body keys are NOT declared here. The slide sequence varies by editorial intent and is annotated on each variant's Structure section, where each slide maps to one `slides[]` item. The envelope owns the invariant head and the slide item shape; the variant owns the sequence.]

[Tips:
- Declare only what the renderer actually consumes — don't mirror an exhaustive field list.
- Keep the metadata keys consistent with the {keys} your variant Structures assume.
- This renders to slides, not a CMS — keep on-slide `body` sparse so it fits the template; depth lives in `speaker_notes`.]

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`.

[Instructions: Populate one row per file in `variants/` when authoring — agents treat this table as the authoritative variant index. `Load When` is a compact trigger phrase (a few words, styled like the Pillars/Collections `Load When` columns in MESSAGE.md) that lets the agent choose the right variant file before loading it — not the 2-4 sentence prose that previously lived in each variant's `## When to use` section.

Examples for this asset:
- first-call — Booked first meeting, problem-to-platform in 15-20 min
- partner — Joint go-to-market, co-branded deck
- executive-briefing — Exec/board audience, outcomes only
- technical-deep-dive — Technical evaluator, architecture depth]

| Variant | File | Description | Load When |
|---------|------|-------------|-----------|
|         |      |             |           |
