# Quarterly Editorial Planning Prompt

## Purpose

This prompt translates the annual editorial strategy into a specific, actionable plan for a single quarter. It takes the year-level thesis, priorities, and type allocations and narrows them into a 13-week editorial architecture with defined objectives, product focus, audience targeting, and campaign alignment.

The quarterly plan is the bridge between strategic direction and calendar-level execution. It does not specify individual latazins day-by-day — that is the monthly calendar's job. It establishes the quarter's editorial identity, dominant content types, product priorities, and risk awareness so that each month within the quarter is planned with coherent intent.

---

## How This File Is Used in the System

```
[Annual Editorial Strategy] ──────────────────────┐
  (output of annual-editorial-strategy-prompt.md)  │
                                                   │
[House Layer] ─────────────────────────────────────┤
  docs/house/commerce-latazin-typology.md          │
  docs/house/house-voice.md                        │
  docs/house/quality-rubric.md                     │
  docs/house/style-guide.md                        │
  docs/house/house-metaphors.md                    │
                                                   ├──▶ THIS PROMPT ──▶ Quarterly Plan
[Input Layer] ─────────────────────────────────────┤
  docs/inputs/product-catalogue.md                 │
  docs/inputs/collections-and-drops.md             │
  docs/inputs/occasions-and-celebrations.md        │
  docs/inputs/month-profiles.md                    │
  docs/inputs/audience-personas.md                 │
  docs/inputs/previous-performance-log.md          │
                                                   │
[Operator Input] ──────────────────────────────────┘
  Which quarter, any mid-year adjustments

                        │
                        ▼
          Monthly Editorial Calendar Prompt
          (docs/planning/monthly-editorial-calendar-prompt.md)
```

The quarterly plan is produced four times per year. Each quarter's output feeds into the monthly editorial calendar prompt as a required input for the three months within that quarter.

---

## Required Inputs

| Input | Source | What It Provides |
|---|---|---|
| Annual Editorial Strategy | Output of `annual-editorial-strategy-prompt.md` | Annual thesis, quarterly themes, product emphasis, collection timing, audience priorities, type distribution targets, strategic experiments |
| Latazin Typology | `docs/house/commerce-latazin-typology.md` | 12 latazin types, type selection guidance, mixing and sequencing rules |
| House Voice | `docs/house/house-voice.md` | Tone spectrum, voice calibration by content type and audience |
| Quality Rubric | `docs/house/quality-rubric.md` | 6 evaluation dimensions, quality tiers, failure patterns |
| Style Guide | `docs/house/style-guide.md` | Sentence-level rules, banned phrases, formatting |
| House Metaphors | `docs/house/house-metaphors.md` | Approved metaphor families for thematic framing |
| Product Catalogue | `docs/inputs/product-catalogue.md` | Product inventory with hero status, editorial potential, season fit, price band |
| Collections & Drops | `docs/inputs/collections-and-drops.md` | Launches scheduled for this quarter with campaign importance and thesis |
| Occasions & Celebrations | `docs/inputs/occasions-and-celebrations.md` | Occasions falling within the quarter with editorial posture and product fit |
| Month Profiles | `docs/inputs/month-profiles.md` | Emotional tone, buying behavior, and seasonal tensions for each month in the quarter |
| Audience Personas | `docs/inputs/audience-personas.md` | Persona profiles with seasonal needs and product interests |
| Previous Performance Log | `docs/inputs/previous-performance-log.md` | Recent latazin performance, strongest pages, lessons |

Additionally, the operator must supply:

- **Which quarter** (Q1, Q2, Q3, or Q4) and the specific months it covers
- **Any mid-year adjustments** to the annual strategy (e.g., a new product launch moved up, a collaboration confirmed, a market shift)
- **Budget or capacity constraints** (e.g., "we can produce a maximum of 8 latazins this quarter")

---

## Prompt

```
You are an editorial planner for a commerce brand operating within the Latazin Editorial Operating System. Your task is to produce a detailed quarterly editorial plan for a specific quarter.

A latazin is a structured editorial content piece that presents products through meaning, context, and sequence. The brand publishes latazins as its primary content format across 12 defined types.

### CONTEXT FILES

Read and internalize all of the following before producing the plan:

**Annual Strategy:**
[Insert the complete annual editorial strategy output]

**House Layer:**
- Latazin Typology: [contents of docs/house/commerce-latazin-typology.md]
- House Voice: [contents of docs/house/house-voice.md]
- Quality Rubric: [contents of docs/house/quality-rubric.md]
- Style Guide: [contents of docs/house/style-guide.md]
- House Metaphors: [contents of docs/house/house-metaphors.md]

**Input Layer:**
- Product Catalogue: [contents of docs/inputs/product-catalogue.md]
- Collections & Drops: [contents of docs/inputs/collections-and-drops.md]
- Occasions & Celebrations: [contents of docs/inputs/occasions-and-celebrations.md]
- Month Profiles: [contents of docs/inputs/month-profiles.md]
- Audience Personas: [contents of docs/inputs/audience-personas.md]
- Previous Performance Log: [contents of docs/inputs/previous-performance-log.md]

**Operator Input:**
- Quarter: [Q1/Q2/Q3/Q4] ([MONTH_1], [MONTH_2], [MONTH_3])
- Mid-year adjustments: [ANY_ADJUSTMENTS or "None"]
- Capacity: [MAX_LATAZINS_THIS_QUARTER or "No hard limit"]

### INSTRUCTIONS

Produce a quarterly editorial plan that translates the annual strategy into specific, actionable direction for this quarter. The plan must be grounded in the actual product catalogue, respect the annual strategy's type distribution targets, and account for every collection launch and occasion falling within the quarter.

Work through the following sections in order:

**1. Quarter Objective**
Write a 2–3 sentence objective for this quarter. It must:
- Connect to the annual thesis
- Reflect the quarterly theme set in the annual strategy
- Name the specific commercial or editorial outcome this quarter must achieve
- Be measurable or at minimum observable

**2. Dominant Categories**
Identify the 2–4 product categories (from the product catalogue) that dominate this quarter. For each:
- Name the category
- Explain why it leads this quarter (seasonal fit, collection launch, audience demand, strategic priority)
- List the specific products from the catalogue that fall within it

**3. Dominant Latazin Types**
From the 12 types in the typology, identify:
- The 2–3 types that should appear most frequently this quarter
- For each, explain why it serves this quarter's objective
- The 1 experimental type from the annual strategy's experiment slate (if scheduled for this quarter)
- Any types that should be explicitly avoided or minimized this quarter, with rationale

Cross-reference the annual strategy's type distribution table. If the quarter's mix deviates from the annual target, explain why.

**4. Seasonal Framing**
Using the month profiles for the three months in this quarter:
- Describe the quarter's overall emotional arc (how does the mood shift from month 1 to month 3?)
- Identify the dominant seasonal tension that editorial content should address
- Name 2–3 sensory or behavioral cues that should appear in content (from the month profiles' weather_cues and social_rhythm fields)
- Recommend the position on the house voice's tone spectrum that best fits this quarter

**5. Campaign Priorities**
Map every collection/drop launching this quarter:
- Collection name, launch period, campaign importance level
- The central thesis of the collection (from collections-and-drops.md)
- Recommended latazin types to support the launch
- How many latazins should support this collection (proportional to campaign importance: anchor = 3–5, major = 2–3, standard = 1–2, minor = 1)
- Timing: pre-launch, launch week, post-launch editorial

If no collection launches this quarter, describe the editorial strategy for a collection-free quarter (emphasis on product arguments, craft studies, occasion pieces, or evergreen content).

**6. Product Focus**
For this quarter, produce a product priority list:
- **Tier 1 — Dedicated latazin required:** Products that should receive their own latazin (typically hero products with high editorial potential launching or peaking this quarter)
- **Tier 2 — Featured within ensemble:** Products that should appear within Bundle/World, Shop the Look, or Occasion latazins but do not need standalone treatment
- **Tier 3 — Background presence:** Products that may appear in product landing pages within other latazins but are not the editorial focus
- **Not this quarter:** Products that are seasonally irrelevant or strategically deprioritized

For Tier 1 products, suggest the latazin type most suited to each.

**7. Launch Windows**
Identify the optimal timing windows within the quarter for:
- Collection/drop launches (aligned with collections-and-drops.md launch periods)
- Occasion-driven content (aligned with occasions-and-celebrations.md dates)
- High-traffic publishing moments (from month profiles' buying behavior fields)
- Quiet periods suitable for editorial-led or experimental content

Present this as a simple 13-week timeline showing which weeks are launch-heavy, occasion-driven, or editorially open.

**8. City Priorities**
Using the audience personas' city fields and the product catalogue's city_fit attribute:
- Identify 2–3 city contexts that should dominate this quarter's visual and editorial framing
- Explain why each city fits the quarter's seasonal mood and product emphasis
- Note any cities that should be de-emphasized this quarter

**9. Key Risks**
Identify 3–5 risks to this quarter's editorial plan:
- Content fatigue risks (e.g., too many similar latazin types in sequence)
- Product risks (e.g., a hero product with weak visual strength carrying too much weight)
- Timing risks (e.g., occasion clustering creating scheduling pressure)
- Voice risks (e.g., campaign-heavy quarter pulling tone toward promotional)
- Audience risks (e.g., a key persona underserved by the quarter's product emphasis)

For each risk, propose a specific mitigation.

**10. Proof Goals**
Define 3–5 measurable goals for this quarter, drawing on the metrics framework from the previous performance log:
- At least one editorial metric (saves, shares — indicating content resonance)
- At least one commercial metric (inquiries, sales — indicating purchase intent)
- At least one structural metric (strongest page analysis — indicating content architecture quality)
- At least one learning goal (a specific question this quarter's performance should answer)

For each goal, state:
- The metric
- The target (absolute number or directional improvement)
- Which latazins or content types are expected to drive it

### CONSTRAINTS

- The total number of latazins proposed must not exceed the operator's stated capacity
- All latazin type recommendations must reference the 12 types from the typology by their exact names
- Seasonal framing must use approved metaphor families only
- Product references must use exact product names from the catalogue
- Occasion references must use exact occasion names from the occasions register
- The plan must be directly consumable by the monthly editorial calendar prompt without reformatting
- Do not use any banned phrases from the style guide
```

---

## Expected Output Format

```
# Quarterly Editorial Plan — [Brand Name] — [Year] [Quarter]

## 1. Quarter Objective
[2–3 sentence objective]

## 2. Dominant Categories
### [Category Name]
- **Why it leads:** ...
- **Products:** ...
[Repeat for each category]

## 3. Dominant Latazin Types
| Type | Frequency | Rationale |
|---|---|---|
| [Primary type 1] | High | ... |
| [Primary type 2] | High | ... |
| [Experimental type] | Low (1 instance) | ... |

**Types to minimize:** ...
**Deviation from annual target:** [explanation if applicable]

## 4. Seasonal Framing
- **Emotional arc:** [Month 1] → [Month 2] → [Month 3]
- **Dominant tension:** ...
- **Sensory cues:** ...
- **Recommended tone position:** ...

## 5. Campaign Priorities
### [Collection Name] — [Campaign Importance]
- **Launch period:** ...
- **Thesis:** ...
- **Supporting latazin types:** ...
- **Latazin count:** ...
- **Timing:** Pre-launch / Launch / Post-launch
[Repeat for each collection]

## 6. Product Focus
### Tier 1 — Dedicated Latazin
| Product | Suggested Latazin Type | Timing |
|---|---|---|
| ... | ... | ... |

### Tier 2 — Featured in Ensemble
- ...

### Tier 3 — Background Presence
- ...

### Not This Quarter
- ...

## 7. Launch Windows
| Week | Type | Key Activity |
|---|---|---|
| Week 1 | ... | ... |
| Week 2 | ... | ... |
| ... | ... | ... |
| Week 13 | ... | ... |

## 8. City Priorities
| City Context | Rationale | Quarter Fit |
|---|---|---|
| ... | ... | ... |

## 9. Key Risks
| Risk | Category | Mitigation |
|---|---|---|
| ... | Content fatigue | ... |
| ... | Product | ... |
| ... | Timing | ... |
| ... | Voice | ... |
| ... | Audience | ... |

## 10. Proof Goals
| Metric | Type | Target | Driver |
|---|---|---|---|
| ... | Editorial | ... | ... |
| ... | Commercial | ... | ... |
| ... | Structural | ... | ... |
| ... | Learning | ... | ... |
```

---

## Quality Checks

Before finalizing the quarterly plan, verify each of the following:

- [ ] **Annual alignment:** The quarter objective explicitly connects to the annual thesis — not a standalone idea
- [ ] **Theme consistency:** The quarterly theme matches what was set in the annual strategy for this quarter; any deviation is explained
- [ ] **Product completeness:** Every hero product seasonally relevant to this quarter appears in at least one tier
- [ ] **Collection coverage:** Every collection/drop launching this quarter is mapped with latazin type recommendations and timing
- [ ] **Occasion integration:** Every occasion from the occasions register falling within this quarter is accounted for; editorial posture (commerce-led, editorial-led, community-led, observe only, avoid) is respected
- [ ] **Type distribution:** The proposed latazin type mix is roughly proportional to the annual strategy's type distribution target for this quarter
- [ ] **Type sequencing:** No more than two consecutive latazins of the same type are proposed; the typology's anti-patterns are avoided
- [ ] **Capacity compliance:** The total latazin count does not exceed the operator's stated capacity
- [ ] **Persona coverage:** At least one content initiative specifically addresses each persona identified as active this quarter in the annual strategy
- [ ] **Risk specificity:** Each risk is concrete and tied to this quarter's actual plan — not generic editorial platitudes
- [ ] **Proof measurability:** Each proof goal has a named metric and a target that can actually be measured with available tools
- [ ] **Voice fidelity:** The plan document itself maintains the house voice — composed, specific, not promotional
- [ ] **No banned language:** No phrases from the style guide's banned list appear in the plan
- [ ] **Downstream readiness:** The plan is structured clearly enough to be consumed by the monthly editorial calendar prompt without reinterpretation
