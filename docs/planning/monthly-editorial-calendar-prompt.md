# Monthly Editorial Calendar Prompt

## Purpose

This prompt generates a complete monthly editorial calendar — the operational document that specifies exactly which latazins will be produced, when they will publish, what products they feature, which latazin type each uses, and how they connect to the quarter's priorities and the month's cultural context.

The monthly calendar is where strategy becomes execution. It is the final planning layer before individual latazin generation begins. Every latazin that enters production must appear on this calendar with a defined type, objective, product attachment, and timing.

---

## How This File Is Used in the System

```
[Annual Editorial Strategy] ──────────────────────────┐
  (output of annual-editorial-strategy-prompt.md)      │
                                                       │
[Quarterly Editorial Plan] ────────────────────────────┤
  (output of quarterly-editorial-planning-prompt.md)   │
                                                       │
[House Layer] ─────────────────────────────────────────┤
  docs/house/commerce-latazin-typology.md              │
  docs/house/house-voice.md                            │
  docs/house/quality-rubric.md                         │
  docs/house/style-guide.md                            │
  docs/house/house-metaphors.md                        │
  docs/house/page-role-system.md                       │
                                                       ├──▶ THIS PROMPT ──▶ Monthly Calendar
[Input Layer] ─────────────────────────────────────────┤
  docs/inputs/product-catalogue.md                     │
  docs/inputs/collections-and-drops.md                 │
  docs/inputs/occasions-and-celebrations.md            │
  docs/inputs/month-profiles.md                        │
  docs/inputs/audience-personas.md                     │
  docs/inputs/previous-performance-log.md              │
                                                       │
[Previous Month Output] ───────────────────────────────┘
  Last month's calendar + performance notes

                        │
                        ▼
          Latazin Content Generation Prompt
          (docs/planning/latazin-content-generation-prompt.md)
```

The monthly calendar is produced once per month, ideally in the final week of the preceding month. Each latazin on the calendar becomes a brief that feeds into the latazin content generation prompt.

---

## Required Inputs

This prompt consumes the most context of any prompt in the system. Every input must be present for the calendar to be well-formed.

| Input | Source | What It Provides |
|---|---|---|
| Annual Editorial Strategy | Output of `annual-editorial-strategy-prompt.md` | Annual thesis, seasonal arcs, type distribution targets |
| Quarterly Editorial Plan | Output of `quarterly-editorial-planning-prompt.md` | Quarter objective, dominant types, product tiers, campaign priorities, launch windows, proof goals |
| Previous Month Calendar | Last month's calendar output + performance notes | What was published, what performed, what was learned, what was deferred |
| Latazin Typology | `docs/house/commerce-latazin-typology.md` | 12 latazin types with selection guidance, mixing rules, sequencing rules |
| House Voice | `docs/house/house-voice.md` | Tone calibration for this month's emotional context |
| Quality Rubric | `docs/house/quality-rubric.md` | Evaluation dimensions to ensure planned latazins are set up for quality |
| Style Guide | `docs/house/style-guide.md` | Constraints that affect feasibility of planned content |
| House Metaphors | `docs/house/house-metaphors.md` | Approved metaphor families for thematic framing |
| Page Role System | `docs/house/page-role-system.md` | Structural requirements that affect latazin scope and complexity |
| Product Catalogue | `docs/inputs/product-catalogue.md` | Full product inventory with all attributes |
| Collections & Drops | `docs/inputs/collections-and-drops.md` | Any collections launching this month |
| Occasions & Celebrations | `docs/inputs/occasions-and-celebrations.md` | Occasions falling within this month with editorial posture |
| Month Profile | `docs/inputs/month-profiles.md` | This month's emotional tone, weather cues, buying behavior, social rhythm, seasonal tensions |
| Audience Personas | `docs/inputs/audience-personas.md` | Persona seasonal needs and product interests |
| Previous Performance Log | `docs/inputs/previous-performance-log.md` | Historical performance data for pattern recognition |

Additionally, the operator must supply:

- **Month and year** being planned
- **Which quarter** this month falls within
- **Any last-minute changes** (product delays, occasion cancellations, new collaborations)
- **Production capacity** (how many latazins can be produced this month)
- **Carry-overs** from last month (latazins deferred, products that need coverage)

---

## Prompt

```
You are an editorial calendar planner for a commerce brand operating within the Latazin Editorial Operating System. Your task is to produce a complete monthly editorial calendar for a specific month.

A latazin is a structured editorial content piece that presents products through meaning, context, and sequence. Each latazin uses one of 12 defined types and follows a page-role structure. The calendar you produce will directly determine what content enters production.

### CONTEXT FILES

Read and internalize all of the following. Every file matters — the calendar must integrate constraints and opportunities from all sources.

**Planning Context:**
- Annual Editorial Strategy: [insert complete annual strategy output]
- Quarterly Editorial Plan: [insert complete quarterly plan for the relevant quarter]
- Previous Month Calendar and Notes: [insert last month's calendar output and any performance observations]

**House Layer:**
- Latazin Typology: [contents of docs/house/commerce-latazin-typology.md]
- House Voice: [contents of docs/house/house-voice.md]
- Quality Rubric: [contents of docs/house/quality-rubric.md]
- Style Guide: [contents of docs/house/style-guide.md]
- House Metaphors: [contents of docs/house/house-metaphors.md]
- Page Role System: [contents of docs/house/page-role-system.md]

**Input Layer:**
- Product Catalogue: [contents of docs/inputs/product-catalogue.md]
- Collections & Drops: [contents of docs/inputs/collections-and-drops.md]
- Occasions & Celebrations: [contents of docs/inputs/occasions-and-celebrations.md]
- Month Profile: [contents of docs/inputs/month-profiles.md — this month's entry only]
- Audience Personas: [contents of docs/inputs/audience-personas.md]
- Previous Performance Log: [contents of docs/inputs/previous-performance-log.md]

**Operator Input:**
- Month: [MONTH] [YEAR]
- Quarter: [Q1/Q2/Q3/Q4]
- Production capacity: [NUMBER] latazins
- Last-minute changes: [CHANGES or "None"]
- Carry-overs from last month: [CARRY_OVERS or "None"]

### INSTRUCTIONS

Produce a monthly editorial calendar that translates the quarterly plan into specific, scheduled latazin briefs. The calendar must account for the month's emotional character, its occasions, product seasonality, collection launches, and lessons from the previous month.

Work through the following sections in order:

**1. Month Thesis**
Write a 1–3 sentence editorial thesis for this month. It must:
- Connect to the quarterly objective and annual thesis
- Reflect the month's emotional tone from the month profile
- Name the specific editorial angle that makes this month distinct from the one before and after it
- Feel like an editorial point of view, not a content plan summary

**2. Weekly Content Arcs**
Divide the month into its calendar weeks (typically 4–5 weeks). For each week, define:
- A brief arc description (1 sentence — what is this week's editorial role within the month?)
- The emotional register for the week (referencing the house voice tone spectrum)
- Whether this is a launch week, occasion week, or open editorial week
- The primary audience persona being addressed this week

The weekly arcs should create a discernible rhythm — not four identical weeks.

**3. Proposed Latazins**
For each latazin planned this month, provide a complete brief entry. The number of latazins must match or fall within the stated production capacity.

For each latazin, specify:

| Field | Description |
|---|---|
| **Working title** | A descriptive editorial title (not final — for planning purposes) |
| **Latazin type** | One of the 12 types from the typology (exact name) |
| **Secondary type** | If type-mixing applies (max 2 types, secondary ≤30%), name it; otherwise "None" |
| **Objective** | What this latazin must accomplish — editorial and/or commercial |
| **Target persona** | Primary audience persona this latazin addresses |
| **Products attached** | Specific products from the catalogue (by exact name) |
| **Collection/drop context** | If supporting a launch, name the collection; otherwise "None" |
| **Occasion relevance** | If tied to an occasion, name it and its editorial posture; otherwise "None" |
| **Publish week** | Which week of the month |
| **Estimated page count** | Based on the page role system's minimum viable and recommended structures for this type |
| **Key page roles** | The primary page roles this latazin should employ (from the 10 page roles) |
| **Tone position** | Where on the tone spectrum (restrained ← composed ← warm ← inviting) |
| **Campaign support** | Yes/No — is this part of a collection campaign? |
| **Risk notes** | Any concerns about this latazin (weak product visuals, tight timing, experimental type, etc.) |

**4. Campaign Support Items**
If any collection/drop launches this month, map the campaign support structure:
- Pre-launch latazin(s): Which latazins build anticipation?
- Launch latazin(s): Which latazins coincide with the drop?
- Post-launch latazin(s): Which latazins extend the conversation after launch?
- Non-latazin support: Any social cutdowns, email features, or ad references that should derive from the latazins?

If no collection launches this month, write: "No active campaigns this month. Editorial-led calendar."

**5. Launch Support Items**
For any product launches (not full collections) happening this month:
- Product name and launch date
- Which existing latazin on the calendar incorporates this product?
- If no latazin covers it, explain why (not all products warrant a latazin) or flag it as a gap

**6. Occasion Integration**
For each occasion falling within this month (from the occasions register):
- Occasion name and date
- Editorial posture (commerce-led, editorial-led, community-led, observe only, avoid)
- Which latazin on the calendar addresses it (if any)?
- If the posture is "observe only" or "avoid," confirm no latazin is planned around it
- Tone guidance specific to this occasion

**7. Content Balance Check**
Produce a summary table showing the month's content balance:

| Dimension | This Month | Quarter Target | Status |
|---|---|---|---|
| Latazin types used | [list] | [from quarterly plan] | On track / Adjust |
| Hero products featured | [count] | [from quarterly plan] | On track / Gap |
| Personas addressed | [list] | [from quarterly plan] | On track / Gap |
| Commerce-led vs. editorial-led ratio | [X:Y] | [from quarterly plan] | On track / Adjust |
| Occasions covered | [count] | [from monthly occasions] | Complete / Missing |

**8. Review Questions**
List 3–5 specific questions that the editorial team should discuss before approving this calendar:
- These should surface genuine tensions, trade-offs, or uncertainties
- They should reference specific latazins, products, or timing decisions on the calendar
- They should not be generic ("Is the mix right?") — they must be pointed ("Does the Craft Study on [product] in week 3 risk feeling redundant after last month's Product Argument on the same material?")

### CONSTRAINTS

- Total latazins must not exceed stated production capacity
- No more than two consecutive latazins of the same type across weeks
- Every Tier 1 product from the quarterly plan's product focus (if relevant to this month) must appear on the calendar
- Occasion editorial postures must be respected — if the posture is "avoid," no latazin may reference that occasion
- The month thesis must connect to the quarterly objective — it cannot be a standalone idea
- All latazin types must be referenced by exact names from the typology
- All product names must match the product catalogue exactly
- All occasion names must match the occasions register exactly
- The calendar must be directly usable as input for the latazin content generation prompt — each entry must contain enough context to brief a latazin
```

---

## Expected Output Format

```
# Monthly Editorial Calendar — [Brand Name] — [Month] [Year]

## 1. Month Thesis
[1–3 sentence editorial thesis]

## 2. Weekly Content Arcs

### Week 1: [Date Range]
- **Arc:** [1-sentence description]
- **Register:** [Position on tone spectrum]
- **Week type:** [Launch / Occasion / Open editorial]
- **Primary persona:** [Persona name]

### Week 2: [Date Range]
...

### Week 3: [Date Range]
...

### Week 4: [Date Range]
...

[Week 5 if applicable]

## 3. Proposed Latazins

### Latazin 1: [Working Title]
| Field | Value |
|---|---|
| **Type** | [Exact type name] |
| **Secondary type** | [Type name or None] |
| **Objective** | [Specific objective] |
| **Target persona** | [Persona name] |
| **Products attached** | [Product names] |
| **Collection/drop** | [Collection name or None] |
| **Occasion** | [Occasion name + posture or None] |
| **Publish week** | [Week number] |
| **Est. page count** | [Number] |
| **Key page roles** | [Role names] |
| **Tone position** | [Spectrum position] |
| **Campaign support** | [Yes/No] |
| **Risk notes** | [Concerns or None] |

### Latazin 2: [Working Title]
...

[Repeat for all latazins]

## 4. Campaign Support Items
### [Collection Name] Campaign
- **Pre-launch:** [Latazin title(s)]
- **Launch:** [Latazin title(s)]
- **Post-launch:** [Latazin title(s)]
- **Non-latazin support:** [Notes]

[Or: "No active campaigns this month. Editorial-led calendar."]

## 5. Launch Support Items
| Product | Launch Date | Covered By | Notes |
|---|---|---|---|
| ... | ... | ... | ... |

[Or: "No standalone product launches this month."]

## 6. Occasion Integration
| Occasion | Date | Posture | Latazin Coverage | Tone Guidance |
|---|---|---|---|---|
| ... | ... | ... | ... | ... |

## 7. Content Balance Check
| Dimension | This Month | Quarter Target | Status |
|---|---|---|---|
| Types used | ... | ... | ... |
| Hero products | ... | ... | ... |
| Personas | ... | ... | ... |
| Commerce:Editorial | ... | ... | ... |
| Occasions covered | ... | ... | ... |

## 8. Review Questions
1. [Specific, pointed question about a calendar decision]
2. [Specific, pointed question about a trade-off]
3. [Specific, pointed question about timing or sequencing]
4. [Specific, pointed question about product coverage]
5. [Specific, pointed question about audience balance]
```

---

## Quality Checks

Before finalizing the monthly calendar, verify each of the following:

- [ ] **Thesis connection:** The month thesis traces a clear line from annual thesis → quarterly objective → this month's angle; it is not generic
- [ ] **Capacity compliance:** The number of proposed latazins does not exceed production capacity
- [ ] **Type variety:** No latazin type appears more than twice on the calendar unless the quarter explicitly calls for it; no two consecutive weeks use the same type
- [ ] **Product coverage:** Every Tier 1 product assigned to this month in the quarterly plan appears on at least one latazin; no Tier 1 product is orphaned
- [ ] **Collection integration:** Every collection launching this month has pre-launch, launch, and/or post-launch latazin coverage proportional to its campaign importance
- [ ] **Occasion respect:** Every occasion this month is accounted for; editorial postures are honored (commerce-led occasions have latazins, "avoid" occasions have none)
- [ ] **Persona rotation:** At least two different personas are addressed across the month; no persona monopolizes the calendar
- [ ] **Weekly rhythm:** The four weeks have distinct arcs — not four identical weeks of "publish a latazin"
- [ ] **Previous month learning:** At least one decision on the calendar is visibly informed by last month's performance or lessons (e.g., "shifting away from X type after weak engagement last month")
- [ ] **Brief completeness:** Each latazin entry contains all 14 fields — no field is left blank or marked "TBD" (risk notes may say "None" if no risks are identified)
- [ ] **Downstream usability:** Each latazin brief contains enough context (type, objective, products, persona, tone, page roles) to be passed directly to the latazin content generation prompt
- [ ] **Voice compliance:** The calendar document itself is written in the house voice — factual, composed, specific
- [ ] **No banned language:** No phrases from the style guide's banned list appear anywhere in the calendar
- [ ] **Balance check honesty:** The content balance table accurately reflects what's on the calendar — gaps are flagged, not hidden
- [ ] **Review questions specificity:** Each review question references a specific latazin, product, or decision — not a generic quality concern
