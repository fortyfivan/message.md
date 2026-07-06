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
Full slide sequence for this variant — each slide = one heading-as-claim + sparse body + speaker notes. Annotate each slide with its output key in `{snake_case}`; each slide is one `slides[]` item. These keys become the body schema agents emit as JSON.

Example (first-call deck, 10–15 slides):
Title — the hero message / outcome the meeting is about; subtitle frames for whom → {title_slide}
The shift — the macro change that makes this urgent now      → {shift}
The cost of [problem] — make it concrete; one stat           → {problem_cost}
Why it persists — the structural reason, not a vendor gripe  → {why_persists}
What good looks like — the reframe                           → {reframe}
How [company] does it — mechanism at the persona's altitude  → {mechanism}
Proof — a named customer outcome, attributed, routed per audience → {proof}
Differentiation — why this is structurally different         → {differentiation}
The path — what engagement looks like (discovery → demo / POC → value) → {path}
Close / CTA — the specific next step                         → {cta}

Each slide's `body` stays sparse (a statement, ≤4 bullets, or one stat / quote); `speaker_notes` carry the talk track.]

[Format: Each slide carries a {key}. Be specific about what each slide delivers. Keys are stable contract — renaming one is a breaking change for downstream consumers.]

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
