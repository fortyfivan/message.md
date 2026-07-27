---
company: "[Instructions: Company name. Use official capitalization.]"
version: "[Instructions: ISO date, YYYY-MM-DD. Update on meaningful revisions.]"
maintained-by: "[Instructions: Owning team.]"
last-reviewed: "[Instructions: ISO date, YYYY-MM-DD.]"
---

# [MESSAGE.md - Company name]

[Instructions: One-paragraph overview, under 75 words. What the company does, who it serves, why it exists. Declarative; no generic adjectives.]

---

## Attributes

*Market framing to set the right altitude for messaging and content generation*

[Instructions: Set relevant company attributes and select value(s) - not a hard list, choose what's relevant]

- **Company type**:         [B2B SaaS / B2B / B2C / B2D / B2G / nonprofit / open-source / hybrid]
- **Company stage**:        [Pre-seed / seed / series A / series B / series C+ / growth / pre-IPO / public / mature]
- **Primary market**:       [Category or industry. Be specific.]
- **Position in market**:   [Challenger / leader / category-defining / niche specialist / disruptor / consolidator]
- **Regions in operation**: [Primary geographies. Use tier framing if broad.]
- **Business model**:       [Subscription / transactional / licensing / advertising / open-source / hybrid]

---

## Facts

*Stable company identity attributes for direct reference*

[Instructions: Set relevant company facts and select value(s) - not a hard list, choose what's relevant]

- **Founded**:      [Year founded, optional light origin story]
- **Headquarters**: [City, region, or distributed]
- **Employees**:    [Count or range]
- **Funding**:      [Total + most recent round, or omit]
- **Customers**:    [Public count or range, with key names, or omit]

---

## Glossary

*Global terminology to adhere to.*

[Instructions: Flat list of terms with usage rules. Include:
- Company specific terminology
- Product naming conventions
- Named technical components and terms
- Industry abbreviations with usage rules

Aim for 10-20 entries at most. More than 30 usually means the glossary is duplicating content that lives elsewhere (i.e. collection profiles).]

- **[Instructions: Term]** — [Instructions: Usage rule or replacement.]

---

## Brand Guardrails

*Absolute constraints that apply to every output. These are hard gates, not style preferences.*

[Instructions: List the constraints that no generated content may violate — banned phrases and claims, legal and compliance rules, trademark and naming rules, things never said about competitors or customers. Keep to 5-15 entries.]

[Format:
- **[Guardrail]** — [The rule, stated as a testable constraint, with the replacement or correct behavior where one exists.]]

---

## Scenarios

*Vocabulary for runtime messaging assembly. Agents infer the scenario of each session by combining dimensional values, and use them to set altitude for each task.*

[Instructions: Customize the values for each dimension. Values are descriptive vocabulary — how each dimension shapes loading and posture is defined once in the agent instruction block (`CLAUDE.md`/`AGENTS.md`), not authored per value.]

| Dimension        | Values                                                                                                                        |
|------------------|-------------------------------------------------------------------------------------------------------------------------------|
| Compelling event | [Instructions: Customize. Common values: Analyst Report, Competitor News, Customer Win, Market Event, etc.]                   |
| Market moment    | [Instructions: Customize. Common values: Category Disruption, Regulatory Shift, Consolidation, etc.]                          |
| Strategic shape  | [Instructions: Customize. Common values: New Product Introduction, Strategic Event, Brand Campaign, Thought Leadership, etc.] |
| Content lens     | [Instructions: Customize. Common values: Awareness, Acquisition, Activation, Adoption, Advocacy, Amplification]               |

---

## Pillars

*Top-level elements that cover the company's full positioning and messaging domain.*

| Pillar        | File                             | Description                                        | Load When                        |
|---------------|----------------------------------|----------------------------------------------------|----------------------------------|
| **Profile**   | `messaging/pillars/profile.md`   | Key statements and brand voice.                    | Always                           |
| **Pitch**     | `messaging/pillars/pitch.md`     | Strategic narrative, UVPs, and differentiators     | Always                           |
| **Position**  | `messaging/pillars/position.md`  | Market landscape, category claims, and positioning | Competitive or category framing  |
| **People**    | `messaging/pillars/people.md`    | Audience framing and relevant messages             | Writing for a specific audience  |
| **Portfolio** | `messaging/pillars/portfolio.md` | Product overview and capabilities                  | References to specific products  |
| **Proof**     | `messaging/pillars/proof.md`     | Customer wins, analyst recognition                 | Backing claims with evidence     |

---

## Collections

*Individual profiles loaded on-demand for focus and relevance.*

Collection items are files named with lowercase-hyphenated slugs (e.g., `ciso.md`, `acme-corp.md`); cross-reference tables point to them by repo-relative path (e.g., `messaging/collections/personas/ciso.md`). Each item's frontmatter `aliases` list carries the alternate names that should route to it.

Each item file's frontmatter is the source of truth for its attributes (type, tier, status, etc.); the reference tables in pillars are routing indexes derived from it. When a table and an item's frontmatter disagree, the item file wins — update the table.

The `Known Entities` column lists the canonical name of every profile file in that collection's directory. It is the recognition vocabulary for the `Load When` trigger — this file is always loaded, so it is the only place an agent can match a name before any pillar or collection has loaded. Aliases in profile frontmatter still route alternate names to the same profile. Update the column whenever a profile is added, renamed, or removed — the same maintenance rule as the pillar routing tables.

[Instructions: Populate the Known Entities cells with the canonical names of the profile files in each collection's directory, comma-separated. Keep the cells in sync as profiles are added, renamed, or removed.]

| Collection      | Path                                 | Description                                                        | Known Entities                             | Load When        |
|-----------------|--------------------------------------|--------------------------------------------------------------------|--------------------------------------------|------------------|
| **Personas**    | `messaging/collections/personas/`    | Buyer role with altitude, pain points, and messaging guidance      | [Names of each profile in this directory]  | Named role       |
| **Products**    | `messaging/collections/products/`    | A product, module, platform, or add-on in the portfolio            | [Names of each profile in this directory]  | Named product    |
| **Competitors** | `messaging/collections/competitors/` | An alternative buyers evaluate (vendor, DIY, status quo)           | [Names of each profile in this directory]  | Named competitor |
| **Segments**    | `messaging/collections/segments/`    | Industry, size, region, or maturity slice with adjusted messaging  | [Names of each profile in this directory]  | Named segment    |
| **Solutions**   | `messaging/collections/solutions/`   | A use-case bundle composed of one or more products                 | [Names of each profile in this directory]  | Named use case   |
| **Stories**     | `messaging/collections/stories/`     | Customer evidence — outcome, quote, and proof                      | [Names of each profile in this directory]  | Named customer   |
| **Categories**  | `messaging/collections/categories/`  | Market category the company aligns with or competes in             | [Names of each profile in this directory]  | Category themes  |
| **Reports**     | `messaging/collections/reports/`     | Third-party research — analyst report, market study, benchmark     | [Names of each profile in this directory]  | Cited research   |


---

## Assets

*Catalog of asset types and variant specs that the messaging system builds on-demand*

[Instructions: Populate `messaging/assets/` directory and fill the values in this table]

| Content type       | Path                               | Available variants                                      |
|--------------------|------------------------------------|---------------------------------------------------------|
| **Blog Post**      | `messaging/assets/blog-post/`      | [All variants in the respective `variants/` directory]  |
| **Customer Story** | `messaging/assets/customer-story/` | [All variants in the respective `variants/` directory]  |
| **Email**          | `messaging/assets/email/`          | [All variants in the respective `variants/` directory]  |
| **Landing Page**   | `messaging/assets/landing-page/`   | [All variants in the respective `variants/` directory]  |
| **One-Pager**      | `messaging/assets/one-pager/`      | [All variants in the respective `variants/` directory]  |
| **Press Release**  | `messaging/assets/press-release/`  | [All variants in the respective `variants/` directory]  |
| **Social Post**    | `messaging/assets/social-post/`    | [All variants in the respective `variants/` directory]  |
| **Whitepaper**     | `messaging/assets/whitepaper/`     | [All variants in the respective `variants/` directory]  |
| **Web Copy**       | `messaging/assets/web-copy/`       | [All variants in the respective `variants/` directory]  |
| **Slide Deck**     | `messaging/assets/slide-deck/`     | [All variants in the respective `variants/` directory]  |
| **Enablement**     | `messaging/assets/enablement/`     | [All variants in the respective `variants/` directory]  |


---

*Progressive loading rules for pillars, collections, and assets are defined in `CLAUDE.md`.*