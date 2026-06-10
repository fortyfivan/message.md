---
company: [Instructions: Company name. Use official capitalization.]
version: [Instructions: ISO date, YYYY-MM-DD. Update on meaningful revisions.]
maintained-by: [Instructions: Owning team, e.g., "marketing".]
last-reviewed: [Instructions: ISO date, YYYY-MM-DD.]
---

# [Instructions: Company name.]

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
- **Headquarters**: [City, region. Or "Distributed (HQ: [city])".]
- **Employees**:    [Count or range.]
- **Funding**:      [Total + most recent round, or omit.]
- **Customers**:    [Public count or range, with key names, or omit.]

---

## Glossary

*Global terminology to adhere to.*

[Instructions: Flat list of terms with usage rules. Include:
- Company specific terminology
- Named technical components and terms
- Industry abbreviations with usage rules


Do NOT include:
- Product names → `pillars/portfolio.md`
- Competitor names → `collections/competitors/`
- Customer names → `collections/stories/`
- Persona role titles → `collections/personas/`
- Category names → `collections/categories/`

Aim for 10-20 entries. More than 30 usually means the glossary is duplicating content that lives elsewhere.]

- **[Instructions: Term]** — [Instructions: Usage rule or replacement.]

---

## Brand Guardrails

*Absolute constraints that apply to every output. These are hard gates, not style preferences.*

[Instructions: List the constraints that no generated content may violate — banned phrases and claims, legal and compliance rules, trademark and naming rules, things never said about competitors or customers. Keep to 5-15 entries. Style and voice preferences belong in `pillars/profile.md`; only absolutes live here.]

[Format:
- **[Guardrail]** — [The rule, stated as a testable constraint, with the replacement or correct behavior where one exists.]]

---

## Scenarios

*Vocabulary for runtime messaging assembly. Agents infer the scenario of each session by combining dimensional values, and use them to set altitude for each task.*

### Dimensions

| Dimension        | Values                                                                                                                        |
|------------------|-------------------------------------------------------------------------------------------------------------------------------|
| Compelling event | [Instructions: Customize. Common values: analyst-report, competitor-news, customer-win, market-event, etc.]                   |
| Market moment    | [Instructions: Customize. Common values: category-disruption, regulatory-shift, consolidation, etc.]                          |
| Strategic shape  | [Instructions: Customize. Common values: new-product-introduction, strategic-event, brand-campaign, thought-leadership, etc.] |
| Content lens     | [Instructions: Customize. Common values: Awareness, Acquisition, Activation, Adoption, Advocacy, Amplification]               |

---

## Pillars

*Top-level elements that cover the company's full positioning and messaging domain.*

| Pillar        | File                             | Description                                  | Load When                                 |
|---------------|----------------------------------|----------------------------------------------|-------------------------------------------|
| **Profile**   | `messaging/pillars/profile.md`   | Key statements and brand voice.              | Always                                    |
| **Pitch**     | `messaging/pillars/pitch.md`     | Strategic narrative and talking points       | Always                                    |
| **Position**  | `messaging/pillars/position.md`  | Category claims and differentiators          | Research and understanding position       |
| **People**    | `messaging/pillars/people.md`    | Audience framing and relevant messages       | Writing for a specific audience altitude  |
| **Portfolio** | `messaging/pillars/portfolio.md` | Product overview and capabilities            | References to specific products           |
| **Proof**     | `messaging/pillars/proof.md`     | Customer wins, analyst recognition           | Backing claims with evidence              |

---

## Collections

*Individual profiles loaded on-demand for focus and relevance.*

Collection items are files named with lowercase-hyphenated slugs (e.g., `ciso.md`, `acme-corp.md`); cross-reference tables point to them by repo-relative path (e.g., `messaging/collections/personas/ciso.md`). Each item's frontmatter `aliases` list carries the alternate names that should route to it.

| Collection      | Path                                 | Description                                                        | Load When        |
|-----------------|--------------------------------------|--------------------------------------------------------------------|------------------|
| **Personas**    | `messaging/collections/personas/`    | Buyer role with altitude, pain points, and messaging guidance      | Named role       |
| **Products**    | `messaging/collections/products/`    | A product, module, platform, or add-on in the portfolio            | Named product    |
| **Competitors** | `messaging/collections/competitors/` | An alternative buyers evaluate (vendor, DIY, status quo)           | Named competitor |
| **Segments**    | `messaging/collections/segments/`    | Industry, size, region, or maturity slice with adjusted messaging  | Named segment    |
| **Solutions**   | `messaging/collections/solutions/`   | A use-case bundle composed of one or more products                 | Named use case   |
| **Stories**     | `messaging/collections/stories/`     | Customer evidence — outcome, quote, and proof                      | Named customer   |
| **Categories**  | `messaging/collections/categories/`  | Market category the company aligns with or competes in             | Category themes  |
| **Reports**     | `messaging/collections/reports/`     | Third-party research — analyst report, market study, benchmark     | Cited research   |


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