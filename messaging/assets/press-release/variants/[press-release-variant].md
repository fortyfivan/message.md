---
slug: ""
asset: press-release
status: active
last-reviewed: ""
---

# [Instructions: Variant name, e.g. "Company news", "Product launch", "Partnership"]

[Instructions: One-line description of this variant — what makes it different from siblings in this asset's `variants/` directory.]

## Voice notes

[Instructions:
Variant-specific voice shifts on top of MESSAGE.md Brand Guardrails + profile.md voice attributes. What changes in this variant's register that doesn't apply to the asset overall?

Examples:
- Company-news: factual + milestone-framed; significance carried by facts (amount raised, the named hire's track record, the customer's scale), not adjectives
- Product-launch: capability + outcome-led; name what it does and for whom; no hype superlatives in the lede; body links to the product page / docs
- Partnership: balanced billing — both parties' value, not a one-sided pitch; joint framing where apt ("together, the companies…"); a quote from each side
]

[Tips:
- Keep this short (3-5 bullets). Voice anchors, not a full style guide.
- Only specify what's different from the asset's base register.]

## Structure

[Instructions:
The shared wire-format spine, with per-variant emphasis, as a single table read by both the writer and downstream production: `Guidance` is the content brief (what each section delivers); `Key` is the `{snake_case}` field a downstream consumer reads. `headline`/`subhead`/`dateline`/`boilerplate` double as the Output schema metadata head — keep them consistent. A press release carries no marketing CTA, so the `cta` row is the media-contact close. Keys are stable contract — renaming one is a breaking change for downstream consumers.

Per-variant emphasis:
- Company-news: lede states the milestone + why-now; second quote often an investor/board member (funding) or the named executive (appointment)
- Product-launch: lede names the product and the problem it solves; detail describes the capability; second quote a customer or design partner; body links to the product page / docs
- Partnership: lede frames the joint value; detail gives both parties balanced billing; two quotes, one per partner; boilerplate for both companies
]

| # | Section | Guidance | Key |
|---|---------|----------|-----|
| 1 | Headline | Declarative, factual, ≤12 words | `headline` |
| 2 | Subhead | Secondary line clarifying scope/significance | `subhead` |
| 3 | Dateline | `CITY — Month Day, Year —` | `dateline` |
| 4 | Lede | 1 paragraph — who, what, why now | `lede` |
| 5 | Detail | 2-3 paragraphs — context, capability, market frame | `detail` |
| 6 | Executive quote | Attributed to a company leader | `exec_quote` |
| 7 | Second quote | Optional — a second perspective | `second_quote` |
| 8 | Boilerplate | Pulled from `profile.md` boilerplate | `boilerplate` |
| 9 | Media contact | The close; name and email | `cta` |

[Format: one row per section, in emission order. `Guidance` is prose (what each section delivers); `Key` is `{snake_case}`, stable contract.]

## CTA conventions

[Instructions:
Press releases don't carry marketing CTAs. The "next step" is the media contact. Hyperlinks in the body point to source materials rather than conversion endpoints — a product page or docs for a launch, a customer story for a company-news win, a partner page for a partnership. Document any exceptions.]

[Tips:
- No "Schedule a demo" / "Contact sales" CTAs — those belong on marketing assets, not the wire.
- Link to substantiating material, not funnel destinations.]

## Writing checks

[Instructions:
Testable, variant-specific checks the writer must satisfy at generation time — a first writing gate on top of the global voice gate. Capture format-specific tells the global voice gate doesn't already catch; don't restate global banned phrases or Brand Guardrails. Each check must be observable, not vague.

Examples (press release):
- No hype adjectives anywhere ("revolutionary", "groundbreaking", "best-in-class"), not just the lede
- No "is proud / thrilled / excited to announce" filler — open on the news
- Quotes sound like a named human said them, not like marketing copy
- Every significance claim is attributed or backed by a fact, not asserted
- Boilerplate matches profile.md verbatim; not paraphrased
]

[Format: testable bullet rules. Omit this section if the variant has no tells beyond the global voice gate.]

## Examples

[Instructions: Optional. Link or cite 1-3 reference releases that exemplify this variant — internal or external. URLs preferred.]
