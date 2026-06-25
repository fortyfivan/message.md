---
slug: ""
asset: whitepaper
status: active
last-reviewed: ""
---

# [Instructions: Variant name, e.g. "Research", "Topic", "Benchmark", "Point of view", "Analyst brief"]

[Instructions: One-line description of this variant — what makes it different from siblings in this asset's `variants/` directory.]

## When to use

[Instructions:
Distinguish this variant from siblings. When does a writer reach for this variant vs. another in this asset's `variants/` directory? Examples:
- Primary research (survey, study, panel data) with novel data → research
- Strategic argument or deep dive on a market/category topic → topic
- Comparative data across vendors, segments, or time → benchmark
- Contrarian or opinionated stance with evidence → point-of-view
- Analyst-style format mimicking Gartner / Forrester / IDC structure → analyst-brief
- Standards, compliance, or technical reference with practical guidance → technical-guide / regulatory
]

[Format: 2-4 sentences. Specific triggers, not vague situations.]

## Voice notes

[Instructions:
Variant-specific voice shifts on top of MESSAGE.md Brand Guardrails + profile.md voice attributes. What changes in this variant's register that doesn't apply to the asset overall?

Examples:
- Research: detached + data-led; "the data shows" not "we believe"; methodology disclosed early; minimal product mention
- Topic: analytical + thesis-led; opens with the strategic frame; product mention reserved for late application section
- Benchmark: factual + comparative; specific numbers, peer set named explicitly; no superlatives without data
- Point-of-view: declarative + opinionated; "we believe" allowed and welcome; named author POV is the asset
- Analyst-brief: peer-of-analyst voice; structured (problem → market → vendors → take); restraint on product positioning
- Technical-guide: instructional + concrete; assumes practitioner reader; code/configuration examples where applicable
]

[Tips:
- Keep this short (3-5 bullets). Voice anchors, not full style guide.
- Whitepaper variants vary sharply in voice — research is detached; point-of-view is opinionated. Get this distinction right.]

## Structure

[Instructions:
Full section sequence for this variant. Annotate each section with its output key in `{snake_case}`. These keys become the body schema agents emit as JSON.

Example (research):
Executive Summary (1 page)                          → {exec_summary}
Methodology (sample, time window, instruments, limitations) → {methodology}
Key Findings (3-5 H2 sections, data + commentary)   → {findings}
Implications                                        → {implications}
Appendix (raw tables)                               → {appendix}
Author bio                                          → {author_bio}
Download / briefing CTA                             → {cta}
]

[Format: Each section carries a {key}. Specify approximate length per section since whitepaper length varies widely (3,000-10,000 words). Keys are stable contract — renaming one is a breaking change for downstream consumers.]

## CTA conventions

[Instructions:
Variant-specific CTA strategy. Whitepaper CTAs vary by editorial intent:
- Research: download (gated form); secondary "book a briefing with the researcher"; cross-links to related research
- Topic: download + book-an-author-conversation; cross-links to related topic papers in series
- Benchmark: download; secondary "see how you compare" (interactive tool if available); peer-network-call offer
- Point-of-view: download; subscribe-to-perspectives newsletter; speaker-booking for the author
- Analyst-brief: download; vendor briefing offer; product demo for the named vendor (when self-published vendor brief)

Cover:
- Primary CTA placement (form-as-CTA for gated; embedded for web-rendered)
- Form field count (typically lighter — 3-5 fields — since the whitepaper itself is the offer)
- Secondary CTA policy
- Cross-link / "related" section convention
]

[Tips:
- For gated whitepapers, the form IS the CTA — the rest of the page sells the gate
- Author availability for follow-up briefings is a strong secondary CTA across all variants]

## Writing checks

[Instructions:
Testable, variant-specific checks the writer must satisfy at generation time — a first writing gate on top of the global voice gate. Capture format-specific tells the global voice gate doesn't already catch; don't restate global banned phrases or Brand Guardrails. Each check must be observable, not vague.

Examples (whitepaper):
- No "in today's rapidly changing landscape" framing to open a section
- No length padding — sections exist to advance the argument, not hit a page count
- No passive hedging where a direct claim belongs ("it could be argued that")
- Conclusion advances beyond the introduction, doesn't restate it
]

[Format: testable bullet rules. Omit this section if the variant has no tells beyond the global voice gate.]

## Examples

[Instructions: Optional. Link or cite 1-3 reference whitepapers that exemplify this variant — internal or external. URLs preferred.]
