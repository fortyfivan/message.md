---
slug: ""
asset: email
status: active
last-reviewed: ""
---

# [Instructions: Variant name, e.g. "Nurture", "Outbound", "Promo", "Lifecycle"]

[Instructions: One-line description of this variant — what makes it different from siblings in this asset's `variants/` directory.]

## Voice notes

[Instructions:
Variant-specific voice shifts on top of MESSAGE.md Brand Guardrails + profile.md voice attributes. What changes in this variant's register that doesn't apply to the asset overall?

Examples:
- Nurture: earned attention → less hooky, more "here's the next useful thing"; reference the recipient's last action in the opening
- Outbound: no earned attention → hook in the first sentence; persona-specific pain; bridge to value in 1 sentence; low-friction ask
- Promo: declarative + benefits-led; urgency if real; scannable layout; clear single CTA
- Lifecycle: personal + contextual; references the trigger event; tone matches the moment (renewal = quietly confident; churn-risk = empathetic)
]

[Tips:
- Keep this short (3-5 bullets). Voice anchors, not full style guide.
- Outbound and nurture sound very different — that's the most important distinction to honor.]

## Structure

[Instructions:
Full section sequence for this variant. Annotate each section with its output key in `{snake_case}`. These keys become the body schema agents emit as JSON. The `subject`/`preheader` keys double as the Output schema metadata head — keep them consistent.

Example (nurture):
Subject (≤8 words; can reference prior asset)               → {subject}
Preheader (extends subject)                                 → {preheader}
Opening (1-2 sentences referencing recipient's last action) → {opening}
Body (2-3 short paragraphs delivering the next useful thing) → {body}
CTA (clear next step appropriate to funnel stage)           → {cta}
]

[Format: Each section carries a {key}. Be specific about each section's purpose and length. Keys are stable contract — renaming one is a breaking change for downstream consumers.]

## CTA conventions

[Instructions:
Variant-specific CTA strategy. Email CTAs vary significantly by variant:
- Nurture mid-funnel: webinar invite, ROI calculator, deeper guide — match commitment level to journey stage
- Nurture late-funnel: demo, peer reference call, technical deep-dive
- Outbound first touch: 15-min conversation question-form ("Open to a 15-min walkthrough next week?"); calendar link policy = NONE on first touch
- Outbound touch 2+: calendar link OK; alternative peer-reference offer as lower-commitment ask
- Promo: single CTA tied to the offer; time-bound if the offer is

Cover:
- Question-form vs. imperative CTA
- Calendar link policy by touch / funnel stage
- Whether secondary CTA is allowed (default: no — multiple links dilute)
- Tracking-param convention]

[Tips:
- Demo CTA on first-touch outbound burns reply rate. Reserve for touch 2+.
- Calendar links mid-funnel nurture are premature. Reserve for late-funnel.
- One asset reference per email — multiple links dilute conversion.]

## Writing checks

[Instructions:
Testable, variant-specific checks the writer must satisfy at generation time — a first writing gate on top of the global voice gate. Capture format-specific tells the global voice gate doesn't already catch; don't restate global banned phrases or Brand Guardrails. Each check must be observable, not vague.

Examples (email):
- No "I hope this email finds you well" / "Just circling back" / "Just following up" openers
- No clickbait subject lines or false urgency ("Act now", "Don't miss out")
- No "I wanted to reach out" throat-clearing — open on the reason
- One clear ask; the CTA isn't buried under preamble
]

[Format: testable bullet rules. Omit this section if the variant has no tells beyond the global voice gate.]

## Examples

[Instructions: Optional. Link or cite 1-3 reference emails that exemplify this variant. Internal sent-folder references work too.]
