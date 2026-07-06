---
slug: ""
asset: landing-page
status: active
last-reviewed: ""
---

# [Instructions: Variant name, e.g. "Campaign destination", "Product page", "Webinar", "Event", "Gated asset"]

[Instructions: One-line description of this variant — what makes it different from siblings in this asset's `variants/` directory.]

## Voice notes

[Instructions:
Variant-specific voice shifts on top of MESSAGE.md Brand Guardrails + profile.md voice attributes. What changes in this variant's register that doesn't apply to the asset overall?

Examples:
- Campaign-destination: matches the campaign's voice (outbound = urgent + specific; nurture = educational + trust-building); hero is the offer, not the brand
- Product-page: capability-led + evergreen; less time-sensitive; deeper proof; matches the product's persona altitude
- Webinar: speaker credibility leads; date/time prominent for live; outcome-led ("what you'll learn") not feature-led
- Event: format clarity (conference / booth / session / keynote); travel-relevant details prominent
- Gated-asset: offer-led; the gate is justified ("what you get on the other side")
]

[Tips:
- Keep this short (3-5 bullets). Voice anchors, not full style guide.
- Only specify what's different from the asset's base register.]

## Structure

[Instructions:
Full section sequence for this variant — one row per block, in page order. Every block shares one fixed item shape across every landing-page variant (declared in the asset's `## Output schema`): `type`, `heading`, `body`, optional `image_url`. This table declares what varies per variant — the sequence and each block's content — not new keys per block. For flat-HTML CMSs the body collapses to a single `body` key instead of a `sections[]` array — note that here if it applies. Sequence position is stable contract; reordering or removing a row is a breaking change for downstream consumers.

Example (campaign-destination):]

| # | `type` | `heading` guidance | `body` guidance | `image_url` |
|---|--------|---------------------|------------------|--------------|
| 1 | hero | Offer, above the fold | CTA framing (CTA itself rendered per CTA conventions) | Hero image/video optional |
| 2 | problem | Persona pain, named | — | — |
| 3 | solution | — | 1-2 paragraphs | — |
| 4 | differentiators | — | 3 cards | Card icons optional |
| 5 | proof | — | Single quote/stat | Logo optional |
| 6 | cta_repeat | — | Repeats the hero CTA | — |

[Format: one row per block in page order (`sections[]` index, or the flat-body equivalent). Populate `image_url` only where that block uses one — otherwise `—`. Reordering/inserting/removing rows is a breaking change for downstream consumers.]

## CTA conventions

[Instructions:
Variant-specific CTA strategy. Landing-page CTAs vary significantly:
- Campaign-destination: one CTA, repeated (hero + footer); matches the campaign's funnel-stage ask
- Product-page: get-started CTA (free trial / book demo); secondary "talk to sales" for enterprise; pricing link if transparent
- Webinar (live): "Register" / "Save your seat" + datetime confirmation; calendar download (.ics) optional
- Webinar (on-demand): "Watch now" / "Get the recording" — no datetime
- Event: "Register" / "Reserve your seat"; for partner-hosted events, partner-portal link
- Gated-asset: form is the CTA; specify form field count (typically ≤5 top-of-funnel, ≤3 retargeting); progressive profiling if returning visitor

Cover:
- Where the CTA lands (hero + footer is typical; form-as-CTA for gated)
- What it links to (calendar, form handler, on-demand URL, etc.)
- Button text pattern
- Whether secondary CTA is allowed (default: no — multi-CTA dilutes conversion)
]

[Tips:
- Specific destinations beat generic. "Schedule a 15-min walkthrough" beats "Schedule a demo."
- One primary CTA per variant — adding a second dilutes conversion.]

## Writing checks

[Instructions:
Testable, variant-specific checks the writer must satisfy at generation time — a first writing gate on top of the global voice gate. Capture format-specific tells the global voice gate doesn't already catch; don't restate global banned phrases or Brand Guardrails. Each check must be observable, not vague.

Examples (landing page):
- No hero superlatives ("the world's leading", "#1 platform") without proof
- No empty benefit-speak ("unlock", "supercharge", "seamless", "next-level")
- No fabricated social proof ("Trusted by thousands") without a real number or named logo
- Headline names the outcome, not the category
]

[Format: testable bullet rules. Omit this section if the variant has no tells beyond the global voice gate.]

## Examples

[Instructions: Optional. Link or cite 1-3 reference assets that exemplify this variant — internal or external. URLs preferred.]
