---
slug: ""
asset: customer-story
status: active
last-reviewed: ""
---

# [Instructions: Variant name, e.g. "Anchor case study", "Mini-story", "Video-transcript companion"]

[Instructions: One-line description of this variant — what makes it different from siblings in the same asset's `variants/` directory.]

## When to use

[Instructions:
Distinguish this variant from siblings. When does a writer reach for this variant vs. another in this asset's `variants/` directory? Examples:
- Flagship reference customer; full problem→outcome narrative with metrics → anchor case study
- Short proof snippet for a logo wall, sales deck, or inline web proof → mini-story
- Written companion to a recorded video testimonial; transcript-derived → video-transcript companion
- Industry/segment-framed story for a named vertical → vertical spotlight
]

[Format: 2-4 sentences. Specific triggers, not vague situations.]

## Voice notes

[Instructions:
Variant-specific voice shifts on top of MESSAGE.md Brand Guardrails + profile.md voice attributes. What changes in this variant's register that doesn't apply to the asset overall?

Examples:
- Anchor: narrative + outcome-led; the customer is the protagonist and the product is the enabler; concrete metrics in every section; named quotes as proof anchors
- Mini-story: tight + single-outcome; one pain, one result, one quote — no narrative arc
- Video-transcript companion: preserves the customer's own phrasing from the recording; lightly edited for readability, not rewritten into marketing voice
- Vertical spotlight: speaks the segment's vocabulary — the regulatory, scale, or workflow specifics the named industry cares about
]

[Tips:
- Keep this short (3-5 bullets). Voice anchors, not full style guide.
- Only specify what's different from the asset's base register.
- If a variant doesn't have distinct voice, it probably shouldn't be its own variant.]

## Structure

[Instructions:
Full section sequence for this variant. Annotate each section with its output key in `{snake_case}`. These keys become the body schema agents emit as JSON.

Example (anchor):
Customer snapshot (who they are, industry, scale) → {snapshot}
Challenge (the pain in their words)               → {challenge}
Why they chose [product]                          → {why_us}
Implementation                                    → {implementation}
Outcome with metrics                              → {outcome}
Forward-looking quote                             → {forward_quote}
Closing CTA                                       → {cta}
]

[Format: Each section carries a {key}. Be specific about what each section delivers, including approximate length per section where it matters. Keys are stable contract — renaming one is a breaking change for downstream consumers.]

## CTA conventions

[Instructions:
Variant-specific CTA strategy — placement, link destination, button voice. CTAs vary by editorial intent: an anchor case study usually drives to a demo or a peer-reference conversation; a mini-story drives to the full case study or a logo-wall hub; a video-transcript companion drives to the video itself or a related story.

Cover:
- Where the CTA lands (inline at natural break vs. closing card vs. both)
- What it links to (specific destination type, e.g., demo calendar, full case study, related story in the same industry)
- Button/link text pattern (e.g., "See how [persona] does X" vs. generic "Learn more")
- Whether to include secondary CTA (e.g., "Or read another [industry] story")
]

[Tips:
- Specific destinations beat generic. "Schedule a 15-min walkthrough" beats "Schedule a demo."
- Match CTA to the variant's persona altitude — executive content gets exec-friendly CTAs (peer reference, analyst report), operator content gets operator CTAs (interactive demo, docs).]

## Writing checks

[Instructions:
Testable, variant-specific checks the writer must satisfy at generation time — a first writing gate on top of the global voice gate. Capture format-specific tells the global voice gate doesn't already catch; don't restate global banned phrases or Brand Guardrails. Each check must be observable, not vague.

Examples (customer story):
- No manufactured-sounding quotes — quotes read like a real person talking, attributed to a named role
- No outcome adjectives without a number ("significant improvement" → cite the metric)
- No "thrilled / excited to partner" filler framing
- Problem stated before solution; results tied to the stated problem
]

[Format: testable bullet rules. Omit this section if the variant has no tells beyond the global voice gate.]

## Examples

[Instructions: Optional. Link or cite 1-3 reference assets that exemplify this variant — internal or external. URLs preferred; brief descriptions if URLs aren't available.]
