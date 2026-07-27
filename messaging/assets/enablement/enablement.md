---
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
- Competitor groupings & strategic approaches: document the canonical competitor groupings and, for each, the strategic approach (beat / differentiate / coexist / cooperate), what to lead with, and what to acknowledge — a table of grouping → approach → lead-with → acknowledge beats prose
- Customer-reference routing: which named references back which deal types (for win/loss and battlecard proof)
- Disqualification patterns: hard rules on which deals to walk away from, not soft suggestions — reps need a clear walk-away line]

## Output

The deliverable is a markdown document. The body follows the selected variant's Structure section — one heading per section, in order. One audience per document — don't let a single file try to serve AE and CSM at once.

[Instructions:
If a downstream tool consumes this asset (the design system / PDF render), declare the frontmatter it needs as a literal block like the one below — one line per field, with an inline comment stating the rule. A variant may note additional fields only it needs (e.g., a battlecard's `competitor`, matching `messaging/collections/competitors/`) in its own file. If nothing downstream consumes this asset, delete the block and state that the output is body-only.]

```markdown
---
title:     # e.g., "Battlecard: [competitor]" / "Playbook: [play]"
subtitle:  # one-line frame, where the layout uses one
audience:  # single internal consumer — AE, SDR/BDR, SE, or CSM
---
```

## Variants

Catalog of variants this asset supports. Files live in `variants/[slug].md`. A variant with a sibling `variants/[slug].html` file uses it as the render template when producing HTML output; the template loads only at render time.

[Instructions: Populate one row per file in `variants/` — agents treat this table as the authoritative variant index. `Load When` is a compact trigger phrase (a few words, styled like the Pillars/Collections `Load When` columns in MESSAGE.md) that lets the agent choose the right variant before loading it.

Examples for this asset:
- battlecard — Single-page fight card for a competitor encounter
- playbook — Step-by-step field manual for a GTM play
- faq — Grouped Q&A arming reps with ready answers
- message-map — One-page value-pillar cheat sheet for a theme
- enablement-script — Timed script for an internal recording
- talk-track — Modular cold-call script with response branches
- discovery-guide — Discovery questions surfacing gaps and fit
- demo-script — Prescriptive show-and-say demo choreography]

| Variant | File | Description | Load When |
|---------|------|-------------|-----------|
|         |      |             |           |
