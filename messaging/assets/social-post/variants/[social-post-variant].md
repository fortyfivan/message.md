---
slug: ""
asset: social-post
status: active
last-reviewed: ""
---

# [Instructions: Variant name, e.g. "LinkedIn", "Twitter/X post", "Twitter/X thread", "Reddit"]

[Instructions: One-line description of this variant — which platform/form factor and what makes it different from siblings.]

## Voice notes

[Instructions:
Variant-specific voice shifts on top of MESSAGE.md Brand Guardrails + profile.md voice attributes. What changes in this variant's register that doesn't apply to the asset overall?

Examples:
- LinkedIn: confident-but-not-cocky; professional but human; opens with a specific scenario or claim, not a generic observation
- Twitter/X post: tight + declarative; no hedging; one idea per tweet; humor or surprise welcome where on-brand
- Twitter/X thread: opener carries the whole argument; each subsequent tweet adds evidence or specificity; numbering optional
- Reddit: practitioner-voice; show your work; expect challenge — write defensively but not defensively-defensively
]

[Tips:
- Platforms reward different registers. The variant's voice should sound native to its platform.
- If a variant doesn't have a distinctly different voice from siblings, it probably doesn't need its own variant.]

## Structure

[Instructions:
Full section sequence (or character/word constraints) for this variant. Annotate each section with its output key in `{snake_case}`. These keys become the body schema agents emit as JSON.

Example (LinkedIn):
Hook (line 1, ≤120 chars — before "see more") → {hook}
Setup (lines 2-4)                             → {setup}
Substance (1-3 short paragraphs)              → {substance}
Hashtags (≤3, at the end)                     → {hashtags}
Close (question, takeaway, or CTA)            → {cta}
]

[Format: Each section carries a {key} (or character constraints). Be specific about each platform's quirks. Keys are stable contract — renaming one is a breaking change for downstream consumers.]

## CTA conventions

[Instructions:
Variant-specific CTA strategy. Social CTAs vary by platform and intent:
- LinkedIn: question-based ("What's your team's approach to X?") or low-friction ask ("Reply with your take" / "Repost if this resonates"); single specific link
- Twitter/X post: usually no explicit CTA (the post IS the CTA); occasional link to a long-form anchor
- Twitter/X thread: closer tweet carries the CTA — long-form link, follow-up question, or reply-to-thread prompt
- Reddit: no link in title; genuine question or "happy to dive deeper" in body; mods will remove anything that reads as marketing

Cover:
- Whether/where the CTA lands
- Link policy (none, one, end-only)
- Tone of the ask (question vs. imperative)
- Whether secondary CTA is allowed]

[Tips:
- Avoid generic "Learn more" — it's dead weight on every platform
- Match CTA intensity to platform norms (LinkedIn tolerates more direct asks than Reddit)]

## Writing checks

[Instructions:
Testable, variant-specific checks the writer must satisfy at generation time — a first writing gate on top of the global voice gate. Capture platform/format-specific tells the global voice gate doesn't already catch; don't restate global banned phrases or Brand Guardrails. Each check must be observable, not vague.

Examples (LinkedIn):
- No engagement-bait closers ("Agree?", "Thoughts?", "Who else has seen this?")
- No broetry — one-sentence paragraphs stacked for scroll-bait
- Hook lands in the first 120 chars, before the "see more" fold
- CTA reads native to the feed, not like a promo banner

Examples (Twitter/X post):
- Single idea; no thread-bait ("a 🧵") on a standalone post
- No hashtag stuffing (0–1 hashtag, not 3+)
]

[Format: testable bullet rules. Omit this section if the variant has no tells beyond the global voice gate.]

## Examples

[Instructions: Optional. Link or cite 1-3 reference posts that exemplify this variant. URLs preferred.]
