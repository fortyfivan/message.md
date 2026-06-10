---
slug: enablement
status: active
default-variant: ""
---

# Enablement

[Instructions:
Internal-facing GTM enablement — the reference assets revenue teams pull up under pressure: competitive battlecards, GTM playbooks, rep/CS FAQs, talk tracks, discovery guides, demo scripts, etc. 

This file carries the company conventions that hold across every enablement variant — scannability, actionability, honesty about competitors, scenario-driven organization, messaging-grounding, naming accuracy, and the routing / disqualification rules reps rely on. Per-type structure, voice, and use-in-the-field conventions live in each variant under `variants/`.]

## Conventions

[Instructions:
Specify the company's enablement-wide standards. Enablement is consumed under pressure — mid-call, pre-meeting, between deal stages — so optimize for a rep with 30 seconds to find what they need.
- Scannability over prose: headers, tables, bold key phrases; the right section findable in seconds
- Actionable over informational: "say this" beats "understand this" — exact language, not background reading
- Honest over optimistic: acknowledge competitor strengths honestly; understating a rival's real strength damages credibility the moment a rep faces a buyer who's done their research
- Scenario-driven over comprehensive: organize around situations reps encounter ("When they bring up [competitor]"), not abstract categories
- Competitor groupings & strategic approaches: document the canonical competitor groupings and, for each, the strategic approach (beat / differentiate / coexist / cooperate), what to lead with, and what to acknowledge — battlecards and objection handling map to these
- Customer-reference routing: which named references back which deal types (for win/loss and battlecard proof)
- Disqualification patterns: hard guidance on which deals to walk away from (size, single-domain stacks, compliance-only scope, pure point-tool-replacement evaluations, etc.)]

[Tips:
- Make competitor handling concrete: a table of grouping → approach → lead-with → acknowledge beats prose.
- Keep disqualification as hard rules, not soft suggestions — reps need a clear walk-away line.]

## Frontmatter requirements

[Instructions:
These are internal documents — design-system-driven, typically rendered to PDF for field use rather than published through a CMS. No publishing tool is configured by default; extend when one is set.

Keys: `title` (the document headline, e.g. "Battlecard: [competitor]" / "Playbook: [play]"), `subtitle` (one-line frame where the layout uses one), `audience` (the single internal consumer — AE, SDR/BDR, SE, or CSM; one audience per document), `body` (the rendered content following the variant's Structure section).

Variant-specific frontmatter gets added per-variant — e.g. a battlecard's `competitor` (matching `messaging/collections/competitors/`), a playbook's `play`, an FAQ's topic groups.]

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`.

[Instructions: Populate one row per file in `variants/` when authoring — agents treat this table as the authoritative variant index]

| Variant | File | Description |
|---------|------|-------------|
|         |      |             |
