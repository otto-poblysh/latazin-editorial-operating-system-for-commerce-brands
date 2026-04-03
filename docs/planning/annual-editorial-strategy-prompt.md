# Annual Editorial Strategy Prompt

## Purpose

This prompt generates a complete annual editorial strategy for a commerce brand operating within the Latazin Editorial Operating System. The strategy establishes the year's editorial thesis, defines quarterly themes, sets product and audience priorities, and creates a high-level content architecture that guides all downstream planning — quarterly plans, monthly calendars, and individual latazin generation.

The annual strategy is the highest-level planning document. It does not specify individual latazins. It sets direction, proportion, and emphasis so that every piece of content produced across the year serves a coherent editorial and commercial agenda.

---

## How This File Is Used in the System

```
[House Layer] ──────────────────────────────────┐
  docs/house/house-voice.md                     │
  docs/house/style-guide.md                     │
  docs/house/commerce-latazin-typology.md       │
  docs/house/quality-rubric.md                  │
  docs/house/house-metaphors.md                 │
  docs/house/page-role-system.md                │
                                                ▼
[Input Layer] ──────────────────────────────────┐
  docs/inputs/audience-personas.md              │
  docs/inputs/product-catalogue.md              │
  docs/inputs/collections-and-drops.md          │
  docs/inputs/occasions-and-celebrations.md     │
  docs/inputs/month-profiles.md                 │
  docs/inputs/previous-performance-log.md       ├──▶ THIS PROMPT ──▶ Annual Editorial Strategy
                                                │
[Brand Context] ────────────────────────────────┘
  Brand name, category, year, market position

                        │
                        ▼
          Quarterly Editorial Planning Prompt
          (docs/planning/quarterly-editorial-planning-prompt.md)
```

The annual strategy is produced once per year (or revised at mid-year). Its output feeds directly into the quarterly editorial planning prompt as a required input.

---

## Required Inputs

Before running this prompt, the following files must be populated with brand-specific data:

| Input | File Path | What It Provides |
|---|---|---|
| House Voice | `docs/house/house-voice.md` | Editorial character, tone spectrum, calibration rules |
| Style Guide | `docs/house/style-guide.md` | Sentence-level mechanics, banned phrases, formatting conventions |
| Latazin Typology | `docs/house/commerce-latazin-typology.md` | The 12 latazin types, selection guidance, sequencing rules |
| Quality Rubric | `docs/house/quality-rubric.md` | 6 evaluation dimensions, quality tiers, failure patterns |
| House Metaphors | `docs/house/house-metaphors.md` | 7 approved metaphor families, anti-patterns |
| Page Role System | `docs/house/page-role-system.md` | 10 page roles, arc principles, minimum viable structures |
| Audience Personas | `docs/inputs/audience-personas.md` | Persona profiles with objections, trust needs, product interests |
| Product Catalogue | `docs/inputs/product-catalogue.md` | Full product inventory with attributes (price band, hero status, editorial potential, season fit) |
| Collections & Drops | `docs/inputs/collections-and-drops.md` | Planned releases with launch windows, campaign importance, thesis |
| Occasions & Celebrations | `docs/inputs/occasions-and-celebrations.md` | Calendar of occasions with editorial posture and product fit |
| Month Profiles | `docs/inputs/month-profiles.md` | Emotional tone, buying behavior, seasonal tensions per month |
| Previous Performance Log | `docs/inputs/previous-performance-log.md` | Historical latazin metrics, strongest pages, lessons learned |

Additionally, the operator must supply:

- **Brand name**
- **Year being planned**
- **Brand category** (e.g., leather goods, fragrance, homeware)
- **Market position statement** (1–3 sentences on where the brand sits)
- **Any business-level mandates** (e.g., "launch DTC channel in Q3," "expand into menswear," "increase average order value by 15%")

---

## Prompt

```
You are an editorial strategist for a commerce brand that uses the Latazin Editorial Operating System. Your task is to produce a comprehensive annual editorial strategy for the upcoming year.

A latazin is a structured editorial content piece that presents products through meaning, context, and sequence — not through flat promotion. The brand publishes latazins as its primary content format.

### CONTEXT FILES

You have been provided with the following reference documents. Read and internalize all of them before producing the strategy:

**House Layer (How We Communicate):**
- House Voice: [contents of docs/house/house-voice.md]
- Style Guide: [contents of docs/house/style-guide.md]
- Latazin Typology: [contents of docs/house/commerce-latazin-typology.md]
- Quality Rubric: [contents of docs/house/quality-rubric.md]
- House Metaphors: [contents of docs/house/house-metaphors.md]
- Page Role System: [contents of docs/house/page-role-system.md]

**Input Layer (What We Have to Work With):**
- Audience Personas: [contents of docs/inputs/audience-personas.md]
- Product Catalogue: [contents of docs/inputs/product-catalogue.md]
- Collections & Drops: [contents of docs/inputs/collections-and-drops.md]
- Occasions & Celebrations: [contents of docs/inputs/occasions-and-celebrations.md]
- Month Profiles: [contents of docs/inputs/month-profiles.md]
- Previous Performance Log: [contents of docs/inputs/previous-performance-log.md]

**Brand Context:**
- Brand name: [BRAND_NAME]
- Year: [YEAR]
- Category: [BRAND_CATEGORY]
- Market position: [MARKET_POSITION]
- Business mandates: [BUSINESS_MANDATES]

### INSTRUCTIONS

Produce an annual editorial strategy that covers the full calendar year. The strategy must be specific to this brand, grounded in the product catalogue and audience personas, and respect all house-layer constraints (voice, style, approved metaphors, quality standards).

Work through the following sections in order:

**1. Annual Thesis**
Write a 2–4 sentence editorial thesis for the year. This is the single organizing idea that connects every piece of content. It should reflect:
- The brand's market position and category
- The strongest tension or opportunity visible in the audience personas
- A genuine editorial angle — not a marketing tagline

**2. Primary Business Priorities**
List 3–5 business priorities for the year, ranked by importance. For each, state:
- The priority itself
- How editorial content specifically supports it
- Which latazin types are most likely to serve this priority (reference the 12 types from the typology)

**3. Major Seasonal Arcs**
Divide the year into 3–4 major seasonal arcs (not necessarily aligned to calendar quarters). For each arc:
- Name the arc (an editorial name, not "Spring" or "Q1")
- Define its emotional register (referencing the tone spectrum from house-voice.md)
- Identify its dominant product categories
- Name the occasions that fall within it (from occasions-and-celebrations.md)
- Describe the buying behavior shift (from month-profiles.md)

**4. Quarterly Themes**
For each quarter (Q1–Q4), define:
- A theme statement (1–2 sentences)
- The dominant editorial mood
- 2–3 latazin types that should appear most frequently
- 1 latazin type to deliberately experiment with
- The primary audience persona(s) being addressed

**5. Product Emphasis by Quarter**
For each quarter, identify:
- Hero products (from the catalogue's hero_status field) that should receive dedicated latazins
- Supporting products that should appear in ensemble contexts
- Products that are seasonally irrelevant this quarter
- Any products with high editorial_potential that haven't been featured recently (check the performance log)

**6. Collection and Drop Timing**
Using the collections-and-drops.md file:
- Map each planned collection/drop to its target quarter
- Assign a campaign importance level to each (anchor, major, standard, minor)
- For anchor and major collections, recommend the latazin types that should support the launch
- Identify any quarters that lack a strong collection anchor — recommend how to fill the editorial gap

**7. Audience Priorities**
For each persona in the audience file:
- Identify which quarters they are most active or receptive
- Name their top trust need that the year's content should address
- Recommend which latazin types resonate most with their aesthetic posture and likely objections
- Flag any persona that is currently underserved by the product catalogue

**8. Content Balance by Latazin Type**
Produce a target distribution of latazin types across the year as approximate percentages. Consider:
- The 12 types from the typology
- Business priorities (some types serve commerce more directly)
- Editorial integrity (the mix must not feel promotional)
- Performance data (which types performed well or poorly in the log)
- The typology's own sequencing guidance (avoid clustering same types)

Present this as a table with columns: Latazin Type | Target % of Annual Output | Primary Quarter(s) | Rationale

**9. Strategic Experiments**
Identify 2–3 editorial experiments for the year. These are deliberate departures from the established pattern — new type combinations, new audience angles, new structural approaches. For each:
- Describe the experiment
- State the hypothesis
- Identify which quarter it should run in
- Define what success looks like
- Explain how it will be evaluated (referencing the quality rubric dimensions and performance metrics)

### CONSTRAINTS

- Do not use any language from the style guide's banned phrases list
- All tone recommendations must stay within the tone spectrum defined in house-voice.md
- All structural recommendations must be compatible with the page role system
- All metaphors used in the strategy document itself should draw from the approved metaphor families
- The strategy must be usable as a direct input to the quarterly editorial planning prompt — keep format clean and referenceable
```

---

## Expected Output Format

The output should be a structured document with the following sections, each clearly headed and internally consistent:

```
# Annual Editorial Strategy — [Brand Name] — [Year]

## 1. Annual Thesis
[2–4 sentence editorial thesis]

## 2. Primary Business Priorities
| Priority | Editorial Role | Key Latazin Types |
|---|---|---|
| ... | ... | ... |

## 3. Major Seasonal Arcs
### Arc: [Name]
- **Months:** ...
- **Emotional register:** ...
- **Dominant categories:** ...
- **Key occasions:** ...
- **Buying behavior:** ...
[Repeat for each arc]

## 4. Quarterly Themes
### Q1: [Theme statement]
- **Mood:** ...
- **Dominant types:** ...
- **Experimental type:** ...
- **Primary persona(s):** ...
[Repeat for Q2–Q4]

## 5. Product Emphasis by Quarter
### Q1
- **Hero products:** ...
- **Supporting products:** ...
- **Seasonally irrelevant:** ...
- **Underexplored high-potential:** ...
[Repeat for Q2–Q4]

## 6. Collection and Drop Timing
| Collection | Target Quarter | Campaign Importance | Supporting Latazin Types |
|---|---|---|---|
| ... | ... | ... | ... |

**Gap Analysis:** [quarters lacking anchors and recommendations]

## 7. Audience Priorities
### [Persona Name]
- **Peak quarters:** ...
- **Top trust need:** ...
- **Best latazin types:** ...
- **Catalogue gaps:** ...
[Repeat for each persona]

## 8. Content Balance by Latazin Type
| Latazin Type | Target % | Primary Quarter(s) | Rationale |
|---|---|---|---|
| Product Argument | ...% | ... | ... |
| Bundle/World | ...% | ... | ... |
| Craft Study | ...% | ... | ... |
| Occasion | ...% | ... | ... |
| Misreading Correction | ...% | ... | ... |
| Manifesto | ...% | ... | ... |
| Collection/Drop | ...% | ... | ... |
| Calendar Marking | ...% | ... | ... |
| Collaboration | ...% | ... | ... |
| Shop the Look | ...% | ... | ... |
| Community/Project | ...% | ... | ... |
| Milestone/Proof | ...% | ... | ... |

## 9. Strategic Experiments
### Experiment 1: [Name]
- **Description:** ...
- **Hypothesis:** ...
- **Target quarter:** ...
- **Success criteria:** ...
- **Evaluation method:** ...
[Repeat for each experiment]
```

---

## Quality Checks

Before finalizing the annual strategy, verify each of the following:

- [ ] **Thesis coherence:** The annual thesis connects logically to the brand's market position and audience tensions — it is not a generic aspiration
- [ ] **Business alignment:** Every business priority has a clear editorial mechanism, not just a vague content promise
- [ ] **Product coverage:** Hero products appear in at least one quarter's emphasis; no hero product is orphaned
- [ ] **Collection integration:** Every collection/drop from the collections register is mapped to a quarter; none are missing
- [ ] **Audience inclusion:** Every persona from the audience file is addressed in at least one quarter; no persona is forgotten
- [ ] **Type distribution realism:** The latazin type percentages sum to approximately 100% and no single type exceeds 30% of annual output
- [ ] **Type diversity:** At least 6 of the 12 latazin types appear in the plan with a non-trivial allocation
- [ ] **Seasonal logic:** Product emphasis aligns with month profiles (e.g., no heavy outerwear emphasis in summer months unless justified)
- [ ] **Voice compliance:** The strategy document itself uses language consistent with the house voice — composed, specific, materially grounded
- [ ] **No banned phrases:** The document contains none of the banned constructions from the style guide
- [ ] **Experiment specificity:** Each experiment has a testable hypothesis and defined success criteria, not a vague "try something new"
- [ ] **Performance integration:** Lessons from the previous performance log are visibly reflected in the strategy (types that failed are de-emphasized or restructured; types that succeeded are reinforced)
- [ ] **Downstream usability:** The document is formatted cleanly enough to be consumed by the quarterly editorial planning prompt without manual reformatting
