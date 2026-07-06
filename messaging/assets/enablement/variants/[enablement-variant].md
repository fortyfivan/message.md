---
slug: ""
asset: enablement
status: active
last-reviewed: ""
---

# [Instructions: Variant name, e.g. "Battlecard", "Playbook", "FAQ", "Message map", "Talk track", "Discovery guide", "Demo script", "Enablement script"]

[Instructions: One-line description of this variant — what makes it different from siblings in this asset's `variants/` directory. Be explicit about the boundary with adjacent variants (e.g., a discovery guide is the question set, not the playbook's qualification gate or the FAQ's rep-ready answers).]

## Voice notes

[Instructions:
Variant-specific voice shifts on top of MESSAGE.md Brand Guardrails + profile.md voice attributes. What changes in this variant's register that doesn't apply to the asset overall?

Examples:
- Battlecard: terse, scannable, honest about the competitor's real strengths; "say this" language, not analysis
- Playbook: directive and sequential — the motion, step by step
- Discovery-guide: questions a buyer answers, not a survey; phrased the way the AE actually asks them; lead the prospect to surface the gap themselves; each question carries the fit signal and the red flag so the rep can read the answer
- Talk-track / enablement-script: spoken cadence — written to be said aloud, not read
- Consultative, honest altitude throughout — diagnosing, not interrogating; route deep technical follow-ups to the SE
]

[Tips:
- Keep this short (3-5 bullets). Voice anchors, not a full style guide.
- Only specify what's different from the asset's base register.]

## Structure

[Instructions:
Full structure for this variant — the section or block pattern, with the in-field format. Annotate each section with its output key in `{snake_case}`. These keys become the body schema agents emit as JSON. Enablement carries no marketing CTA — the `{cta}` slot is the rep's next field move (a follow-up question, demo moment, asset to send, or SE / deal-desk handoff).

Example (battlecard):
Their pitch                                    → {their_pitch}
Where we win                                   → {where_we_win}
Where they're strong (honest)                  → {their_strengths}
Objection responses ("when they say X, say Y") → {objections}
Proof to cite                                  → {proof}
Trap-setting questions (the next move)         → {cta}
]

[Format: Each section carries a {key}. Be specific about what each part delivers and the in-field rendering. Keys are stable contract — renaming one is a breaking change for downstream consumers.]

## CTA conventions

[Instructions:
Enablement carries no marketing CTA — it's internal. The "next move" is a specific field action: a follow-up question, a pivot to a demo moment, an asset to send, or an SE / deal-desk handoff. Where a buyer raises a cooperating system (e.g., an incumbent ITSM / CMDB), the next move runs the cooperation reframe, never a displacement push. Never leave the rep with an answer or step they can't act on.

Document the variant's specific "next move" pattern and where it routes.]

[Tips:
- Every section should end with an action the rep can take, not just information.
- Route deep technical or pricing follow-ups to the right owner (SE, deal desk).]

## Writing checks

[Instructions:
Testable, variant-specific checks the writer must satisfy at generation time — a first writing gate on top of the global voice gate. Capture format-specific tells the global voice gate doesn't already catch; don't restate global banned phrases or Brand Guardrails. Each check must be observable, not vague.

Examples (enablement):
- Scannable — a rep mid-call finds the right section in seconds (headers, tables, bolded key phrases), not a wall of prose
- Actionable — provides exact "say this" language, not background reading
- Honest — competitor strengths acknowledged accurately; nothing understated that a researched buyer would catch
- Scenario-driven — organized around situations reps hit, not abstract categories
- Routed — every entry ends in a next move (question, demo moment, asset, or handoff), never a dead end
- Sourced — claims / pains / value map to `position.md`, `proof.md`, `people.md`; nothing invented
- Naming accuracy — every product / term matches the MESSAGE.md Glossary; cooperating systems handled as cooperation, not displacement
- (Discovery-guide) every question is askable as phrased and carries both a fit signal and a red-flag signal
]

[Format: testable bullet rules. Omit this section if the variant has no tells beyond the global voice gate.]

## Examples

[Instructions: Optional. Link or cite 1-3 reference assets that exemplify this variant — internal or external. URLs preferred.]
