---
slug: ""
asset: web-copy
status: active
last-reviewed: ""
---

# [Instructions: Variant name, e.g. "Product page", "Solution page", "Comparison page", "Topic page", "Landing page"]

[Instructions: One-line description of this variant — what makes it different from siblings in this asset's `variants/` directory.]

## Voice notes

[Instructions:
Variant-specific voice shifts on top of MESSAGE.md Brand Guardrails + profile.md voice attributes. What changes in this variant's register that doesn't apply to the asset overall?

Examples:
- Product-page: capability-led, evergreen, deeper proof; matches the product's persona altitude
- Comparison-page: factual and fair; contrast without disparagement; every claim is defensible
- Topic-page: authoritative and educational — the reader is learning, not being sold to; calibrate altitude to who searches the term; frame challenges in the practitioner's vocabulary; the one commercial section explains the approach, not the product
- Landing-page: offer-led; the page has one job; matches the campaign's funnel-stage ask
]

[Tips:
- Keep this short (3-5 bullets). Voice anchors, not a full style guide.
- Only specify what's different from the asset's base register.]

## Structure

[Instructions:
Full section sequence for this variant — one row per block, in page order, with approximate length per block where it matters. Every block shares one fixed item shape across every web-copy variant (declared in the asset's `## Output schema`): `type`, `heading`, `body`, optional `image_url`. This table declares what varies per variant — the sequence and each block's content — not new keys per block. Sequence position is stable contract; reordering or removing a row is a breaking change for downstream consumers.

SEO/GEO note: primary keyword in H1, first sentence of any definition block, and meta description; write H2/H3 headers as standalone searchable phrases.

Example (product-page):]

| # | `type` | `heading` guidance | `body` guidance | `image_url` |
|---|--------|---------------------|------------------|--------------|
| 1 | hero | Capability + outcome | — | Hero image optional |
| 2 | capabilities | — | Grid/table of key capabilities | Icons optional |
| 3 | how_it_works | — | — | Diagram optional |
| 4 | proof | — | Inline quote/metric | Logo optional |
| 5 | integrations | — | — | Logo grid optional |
| 6 | cta | Get-started | — | — |

[Format: one row per block in page order (`sections[]` index). Populate `image_url` only where that block uses one — otherwise `—`. Reordering/inserting/removing rows is a breaking change for downstream consumers.]

## CTA conventions

[Instructions:
Variant-specific CTA strategy — placement, destination, button voice. Web CTAs vary by intent:
- Product-page: get-started CTA (demo / trial); secondary "talk to an architect" for enterprise
- Solution-page: outcome-framed demo CTA tied to the use case
- Comparison-page: "see it in your environment" / migration or eval CTA
- Topic-page: soft CTA only — the educational content carries the page; end the commercial section with a low-pressure next step (learn more, related story); exec-targeted topics flex to executive briefing / peer reference
- Landing-page: one CTA, repeated (hero + footer); form-as-CTA for gated offers

Cover where the CTA lands, what it links to, the button-text pattern, and whether a secondary CTA is allowed (default: one primary action per page).]

[Tips:
- Specific destinations beat generic. "Schedule a technical demo" beats "Contact sales."
- Match CTA altitude to the page's audience — director-level operator CTAs vs. CISO-level exec CTAs.]

## Writing checks

[Instructions:
Testable, variant-specific checks the writer must satisfy at generation time — a first writing gate on top of the global voice gate. Capture format-specific tells the global voice gate doesn't already catch; don't restate global banned phrases or Brand Guardrails. Each check must be observable, not vague.

Examples (web copy):
- Passes the 5-second test: H1 + first subhead convey what the page is and who it's for
- Headers tell the story: reading only the H1/H2s conveys the value proposition
- One primary CTA per section; no competing actions at the same scroll depth
- Proof sits inline next to the claim, not deferred to another page
- Naming accuracy: every product/term matches the MESSAGE.md Glossary
- (Topic-page) Definition block is a 2–4 sentence, snippet-extractable answer to the core question; commercial section is ≤20% of length and no longer than any educational section
- (Comparison-page) Every competitive claim is factual and defensible
]

[Format: testable bullet rules. Omit this section if the variant has no tells beyond the global voice gate.]

## Examples

[Instructions: Optional. Link or cite 1-3 reference assets that exemplify this variant — internal or external. URLs preferred.]
