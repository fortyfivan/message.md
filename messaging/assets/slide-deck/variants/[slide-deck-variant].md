---
slug: ""
asset: slide-deck
status: active
last-reviewed: ""
---

# [Instructions: Variant name, e.g. "First-call", "Partner", "Executive briefing", "Technical deep-dive"]

[Instructions: One-line description of this variant — what makes it different from siblings in this asset's `variants/` directory.]

## Voice notes

[Instructions:
Variant-specific voice shifts on top of MESSAGE.md Brand Guardrails + profile.md voice attributes. What changes in this variant's register that doesn't apply to the asset overall?

Examples:
- Presenter's deck, not a leave-behind: slides sparse, the argument lives in speaker notes; if a slide reads like a document, distill it
- Story over catalog: lead through one argument; don't open with the platform
- Confident, honest, peer-level: a credible expert walking a buyer through a real problem — acknowledge what current tools do well before showing the gap
- Altitude-matched: executive cut = outcomes / risk / cost, no product internals on-slide; practitioner cut = enough mechanism to be credible
]

[Tips:
- Keep this short (3-5 bullets). Voice anchors, not a full style guide.
- Only specify what's different from the asset's base register.]

## Structure

[Instructions:
Full slide sequence for this variant — one row per slide, in presentation order. Every slide shares one fixed item shape across every deck variant (declared in the asset's `## Output schema`): `heading`, `body`, `speaker_notes`, optional `proof`, optional `visual`. This table declares what varies per variant — the sequence and each slide's content — not new keys per slide. Sequence position is stable contract; reordering or removing a row is a breaking change for downstream consumers.

Example (first-call deck, 10–15 slides):]

| # | `heading` (the claim) | `body` (on-slide, sparse) | `speaker_notes` covers | `proof` | `visual` |
|---|---|---|---|---|---|
| 1 | Title — hero message / outcome | Subtitle framing who this is for | — | — | Title art / logo |
| 2 | The shift — macro change, urgency | One-line claim | Why now, in the presenter's words | — | Trend chart (optional) |
| 3 | The cost of [problem] | One concrete stat | Framing narrative | — | Stat callout |
| 4 | Why it persists | Structural reason, ≤4 bullets | Non-vendor-gripe framing | — | — |
| 5 | What good looks like | The reframe statement | — | — | Before/after diagram |
| 6 | How [company] does it | Mechanism, persona-altitude | Depth per persona | — | Architecture diagram |
| 7 | Proof | Named outcome + metric | Attribution, audience routing | Yes | Logo / quote card |
| 8 | Differentiation | ≤4 bullets, structural | — | — | Comparison table |
| 9 | The path | Stage sequence (discovery → demo / POC → value) | Engagement detail | — | Timeline graphic |
| 10 | Close / CTA | The specific next step | — | — | CTA card |

[Format: one row per slide in emission order (`slides[]` index). Populate `proof`/`visual` columns only where that slide uses them — otherwise `—`. Reordering/inserting/removing rows is a breaking change for downstream consumers.]

## CTA conventions

[Instructions:
The closing slide names one specific next step matched to the deal stage — a technical working session, a scoped POC, an executive briefing, or a business-case build — never generic "contact sales" and never a single bare "book a demo." Where an adjacent system came up (e.g., an incumbent ITSM / CMDB), run the cooperation reframe, not a displacement push. The CTA is the next meeting, not the signature.

Cover where the CTA lands, what it links to, and the button / next-step text pattern.]

[Tips:
- Specific destinations beat generic. "Scope a 30-minute working session" beats "Book a demo."
- Match the CTA to the deal stage and the persona's altitude.]

## Writing checks

[Instructions:
Testable, variant-specific checks the writer must satisfy at generation time — a first writing gate on top of the global voice gate. Capture format-specific tells the global voice gate doesn't already catch; don't restate global banned phrases or Brand Guardrails. Each check must be observable, not vague.

Examples (slide deck):
- Slide count within the variant's band, following its required spine; opens on the hero message, not the platform
- Every slide heading states a takeaway as a claim, not a label; reading only the headings conveys the argument
- Slides are sparse (claim + ≤4 bullets / one stat-or-quote); the depth lives in `speaker_notes`, which read as what the presenter actually says
- One persona, one altitude throughout — executive cut carries no product internals; practitioner cut stays credible to an evaluator
- Proof sits on the slide where its claim is earned, attributed and routed per audience; stats within `proof.md` ranges, no invented precision
- Differentiation is structural and positioned alongside adjacent categories — never displacement against a named cooperating system
- Close names one specific, stage-matched next step — not "contact sales," not a bare "book a demo"
- Naming accuracy: every product / term matches the MESSAGE.md Glossary
]

[Format: testable bullet rules. Omit this section if the variant has no tells beyond the global voice gate.]

## Examples

[Instructions: Optional. Link or cite 1-3 reference assets that exemplify this variant — internal or external. URLs preferred.]
