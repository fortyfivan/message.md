---
slug: ""
asset: one-pager
status: active
last-reviewed: ""
---

# [Instructions: Variant name, e.g. "Sales", "Battlecard", "Datasheet"]

[Instructions: One-line description of this variant — what makes it different from siblings in this asset's `variants/` directory.]

## Voice notes

[Instructions:
Variant-specific voice shifts on top of MESSAGE.md Brand Guardrails + profile.md voice attributes. What changes in this variant's register that doesn't apply to the asset overall?

Examples:
- Sales: champion-forwardable; benefit-led; concrete proof points; no jargon a director wouldn't use
- Battlecard: declarative + specific; competitor named explicitly; no hedge language ("we believe", "we think")
- Datasheet: factual + scannable; capability tables; no marketing flourish
- Partner-overview: joint-first-person ("together we...") with clean dual-logo handling
]

[Tips:
- Keep this short (3-5 bullets). Voice anchors, not full style guide.
- Only specify what's different from the asset's base register.]

## Structure

[Instructions:
Full section sequence for this variant. Annotate each section with its output key in `{snake_case}`. These keys become the body schema agents emit as JSON.

Example (sales):
Header (persona + value prop)  → {header}
The problem (2-3 sentences)    → {problem}
The solution (2-3 sentences)   → {solution}
Differentiators (3 bullets)    → {differentiators}
Use cases (3 bullets)          → {use_cases}
Proof (1-2 customers + metric) → {proof}
CTA                            → {cta}
]

[Format: Each section carries a {key}. Be specific about what each section delivers, including approximate length/space per section since one-pagers are space-constrained. Keys are stable contract — renaming one is a breaking change for downstream consumers.]

## CTA conventions

[Instructions:
Variant-specific CTA strategy. One-pager CTAs vary by editorial intent:
- Sales: "Book a 30-min walkthrough" with calendar link — or "Share with [stakeholder role]" for champion-handoff scenarios
- Battlecard: "Schedule a competitive deep-dive" or "Request a head-to-head demo" — calendar + competitor-context
- Datasheet: "Review the docs" + technical-overview link; secondary "Request a trial" for evaluators
- Partner-overview: joint CTA ("Get started with [Company] + [Partner]") — calendar or partner-portal

Cover:
- Where the CTA lands (footer card vs. header callout)
- Calendar link vs. form vs. external link policy
- Whether the variant supports a secondary CTA]

[Tips:
- One primary CTA — adding a second dilutes
- Match CTA to who the reader will forward this to (champion → internal pitch; technical evaluator → docs)]

## Writing checks

[Instructions:
Testable, variant-specific checks the writer must satisfy at generation time — a first writing gate on top of the global voice gate. Capture format-specific tells the global voice gate doesn't already catch; don't restate global banned phrases or Brand Guardrails. Each check must be observable, not vague.

Examples (one-pager):
- No feature dump — every feature ties to an outcome the reader cares about
- No "best-in-class / industry-leading" claims without backing
- No dense paragraphs where scannable bullets belong
- Fits one page; nothing padded to fill space
]

[Format: testable bullet rules. Omit this section if the variant has no tells beyond the global voice gate.]

## Examples

[Instructions: Optional. Link or cite 1-3 reference assets that exemplify this variant — internal or external. URLs preferred; brief descriptions if URLs aren't available.]
