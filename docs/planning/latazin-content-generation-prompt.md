# Latazin Content Generation Prompt

## Purpose

This prompt generates a complete individual latazin — a structured editorial content piece that presents products through meaning, context, and sequence. It is the final and most detailed prompt in the system, producing publish-ready content from a latazin brief.

Unlike the planning prompts, which set strategy and scheduling, this prompt produces the actual editorial output: concept, title, premise, page-by-page structure, draft copy, visual direction, product placement logic, and calls to action. It must integrate every house-layer document as operational constraint and produce structured output that can be evaluated against the quality rubric.

---

## How This File Is Used in the System

```
[Monthly Calendar Latazin Brief] ──────────────────────┐
  (single latazin entry from monthly calendar output)   │
                                                        │
[House Layer — ALL FILES] ─────────────────────────────┤
  docs/house/house-voice.md                             │
  docs/house/style-guide.md                             │
  docs/house/commerce-latazin-typology.md               │
  docs/house/quality-rubric.md                          │
  docs/house/house-metaphors.md                         │
  docs/house/page-role-system.md                        │
                                                        ├──▶ THIS PROMPT ──▶ Complete Latazin
[Input Layer — Relevant Files] ────────────────────────┤
  docs/inputs/product-catalogue.md (attached products)  │
  docs/inputs/collections-and-drops.md (if applicable)  │
  docs/inputs/occasions-and-celebrations.md (if appl.)  │
  docs/inputs/month-profiles.md (current month)         │
  docs/inputs/audience-personas.md (target persona)     │
                                                        │
[Planning Context] ────────────────────────────────────┘
  Annual thesis, quarterly objective, month thesis

                        │
                        ▼
          Review Against Quality Rubric
          Log to Previous Performance Log
```

This prompt is run once per latazin. Each run produces one complete content piece. The output is reviewed against the quality rubric before publication, and its performance is eventually logged in the previous performance log to inform future planning.

---

## Required Inputs

This prompt requires the most comprehensive context in the system. Every house-layer document is mandatory. Input-layer documents are included selectively based on the latazin brief.

### House Layer (All Required)

| Input | File Path | What It Provides |
|---|---|---|
| House Voice | `docs/house/house-voice.md` | Editorial character, tone spectrum, calibration rules by content type, audience proximity, price point, and season |
| Style Guide | `docs/house/style-guide.md` | Sentence character, paragraph rhythm, opening logic, product language rules, banned phrases (130+), CTA restraint, formatting conventions |
| Latazin Typology | `docs/house/commerce-latazin-typology.md` | Type definition, when to use, when not to use, differentiators, type mixing rules (max 2, secondary ≤30%) |
| Quality Rubric | `docs/house/quality-rubric.md` | 6 evaluation dimensions (Editorial Feel, Product Meaning, Taste, Structural Persuasion, Voice Consistency, Completeness & Craft), quality tiers (Publish, Revise, Rethink, Reject), 8 common failure patterns |
| House Metaphors | `docs/house/house-metaphors.md` | 7 approved metaphor families (Commerce & Exchange, Taste & Judgment, Sequence & Rhythm, Ritual & Ceremony, Materiality & Craft, Perception & Atmosphere, Public Meaning & Culture), anti-patterns to avoid |
| Page Role System | `docs/house/page-role-system.md` | 10 page roles (Premise, Witness, Argument, Detail, Pause, Invitation, Product Landing, Proof, Contrast, Atmosphere), arc principle, sequencing rules, minimum viable and recommended structures by type, anti-patterns |

### Input Layer (Selectively Required)

| Input | File Path | When Required |
|---|---|---|
| Product Catalogue | `docs/inputs/product-catalogue.md` | Always — for every product attached to this latazin |
| Collections & Drops | `docs/inputs/collections-and-drops.md` | When the latazin supports a collection launch |
| Occasions & Celebrations | `docs/inputs/occasions-and-celebrations.md` | When the latazin is tied to an occasion |
| Month Profile | `docs/inputs/month-profiles.md` | Always — the current month's entry for seasonal grounding |
| Audience Personas | `docs/inputs/audience-personas.md` | Always — the target persona's full profile |

### Planning Context (Required)

| Input | Source | What It Provides |
|---|---|---|
| Annual Thesis | Annual editorial strategy output | The year's organizing editorial idea |
| Quarterly Objective | Quarterly plan output | The quarter's specific editorial/commercial goal |
| Month Thesis | Monthly calendar output | The month's editorial angle |
| Latazin Brief | Monthly calendar's latazin entry | Working title, type, objective, persona, products, occasion, tone position, page count, key page roles, campaign support flag |

---

## Prompt

```
You are an editorial content creator for a commerce brand operating within the Latazin Editorial Operating System. Your task is to produce a complete, publish-ready latazin from the brief and context provided.

A latazin is a structured editorial content piece that presents products through meaning, context, and sequence — not through flat promotion. It follows a specific type from the brand's typology, uses a defined page-role structure, and speaks in the brand's house voice. Every element of the latazin must be intentional.

### HOUSE LAYER — MANDATORY CONSTRAINTS

These documents define how you write. Read and internalize every rule before generating any content.

**House Voice:**
[Insert complete contents of docs/house/house-voice.md]

**Style Guide:**
[Insert complete contents of docs/house/style-guide.md]

**Latazin Typology:**
[Insert complete contents of docs/house/commerce-latazin-typology.md]

**Quality Rubric:**
[Insert complete contents of docs/house/quality-rubric.md]

**House Metaphors:**
[Insert complete contents of docs/house/house-metaphors.md]

**Page Role System:**
[Insert complete contents of docs/house/page-role-system.md]

### INPUT LAYER — CONTENT CONTEXT

**Product Details:**
[Insert full catalogue entries for every product attached to this latazin from docs/inputs/product-catalogue.md. Include all fields: product_name, category, collection, price_band, material, shipping_ease, product_status, hero_status, giftability, visual_strength, editorial_potential, audience_fit, season_fit, city_fit]

**Collection/Drop Context:**
[If this latazin supports a collection launch, insert the full collection entry from docs/inputs/collections-and-drops.md. Include: collection_name, launch_period, products_included, central_thesis, campaign_importance, limited_or_evergreen, launch_type, supporting_notes. If not applicable, write: "This latazin is not tied to a collection launch."]

**Occasion Context:**
[If this latazin is tied to an occasion, insert the full occasion entry from docs/inputs/occasions-and-celebrations.md. Include: occasion_name, date_or_period, region_relevance, tone, editorial_posture, suitable_latazin_types, product_fit, supporting_notes. If not applicable, write: "This latazin is not tied to a specific occasion."]

**Month Profile:**
[Insert the current month's complete profile from docs/inputs/month-profiles.md. Include: emotional_tone, weather_cues, buying_behavior, social_rhythm, likely_occasions, product_priorities, seasonal_tensions, campaign_possibilities]

**Target Persona:**
[Insert the full persona profile from docs/inputs/audience-personas.md. Include: persona_name, city, lifestyle, aesthetic_posture, likely_objections, trust_needs, product_interests, seasonal_needs, platform_behavior]

### PLANNING CONTEXT

- **Annual thesis:** [Insert from annual strategy]
- **Quarterly objective:** [Insert from quarterly plan]
- **Month thesis:** [Insert from monthly calendar]

### LATAZIN BRIEF

This is the specific assignment from the monthly editorial calendar:

- **Working title:** [WORKING_TITLE]
- **Latazin type:** [TYPE — exact name from typology]
- **Secondary type:** [SECONDARY_TYPE or None]
- **Objective:** [OBJECTIVE]
- **Target persona:** [PERSONA_NAME]
- **Products attached:** [PRODUCT_NAMES — comma-separated]
- **Collection/drop context:** [COLLECTION_NAME or None]
- **Occasion relevance:** [OCCASION_NAME + editorial posture, or None]
- **Tone position:** [POSITION on restrained ← composed ← warm ← inviting spectrum]
- **Estimated page count:** [NUMBER]
- **Key page roles:** [ROLE_NAMES — comma-separated]
- **Campaign support:** [Yes/No]

### GENERATION INSTRUCTIONS

Produce the latazin by working through each section below in sequence. Do not skip any section. Every section must be completed before moving to the next.

---

#### SECTION 1: CONCEPT

Before writing any content, establish the latazin's editorial foundation:

**1a. Core Argument**
In 2–3 sentences, state the central argument or point of view this latazin makes. This is not a summary of the product — it is the editorial claim that justifies the latazin's existence. Ask: "What does the reader understand after reading this that they didn't before?"

**1b. Editorial Angle**
In 1–2 sentences, describe the specific angle of approach. How does this latazin enter its subject? Through material? Through occasion? Through contrast with a misconception? Through a scene? The angle must match the latazin type's definition from the typology.

**1c. Reader Takeaway**
In 1 sentence, state what the target persona walks away with. This must address at least one of their trust_needs or likely_objections from the persona profile.

---

#### SECTION 2: TITLE OPTIONS

Provide exactly 3 title options. Each title must:
- Be specific to this latazin's content (not interchangeable with another latazin)
- Avoid all banned phrases and constructions from the style guide
- Match the tone position specified in the brief
- Not use exclamation marks, rhetorical questions, or imperative commands
- Be between 4 and 12 words

Present as:
1. [Title option — brief rationale for this direction]
2. [Title option — brief rationale for this direction]
3. [Title option — brief rationale for this direction]

Recommend one as the primary title and explain why.

---

#### SECTION 3: PREMISE

Write the premise for this latazin — the opening that establishes why the reader should care. The premise corresponds to the Premise page role from the page role system.

Requirements:
- 2–4 sentences
- Establishes context before introducing any product
- Does not start with the product name, a question, a statistic, "Introducing," or flattery of the reader (per style guide opening logic)
- Sets the emotional register for the entire piece
- Uses at least one metaphor from the approved metaphor families (name which family)
- Connects to the month's seasonal context naturally, not forcibly

---

#### SECTION 4: PAGE-BY-PAGE STRUCTURE

Design the complete page structure using the page role system. For each page:

| Page | Role | Content Summary | Word Count Target | Visual Direction |
|---|---|---|---|---|
| 1 | [Role name] | [What this page accomplishes in 1–2 sentences] | [Range] | [Visual guidance: what the image/layout should convey] |
| 2 | [Role name] | [Content summary] | [Range] | [Visual direction] |
| ... | ... | ... | ... | ... |

The structure must:
- Follow the arc principle: Ground → Show → Argue → Land → Invite
- Begin with Premise (always page 1)
- Follow the sequencing rules from the page role system (argument after context, detail after argument, invitation after landing, etc.)
- Match or exceed the minimum viable structure for this latazin type
- Not exceed the estimated page count from the brief by more than 2 pages
- Include at least one Product Landing page for each attached product
- Include no more than one Invitation page (the CTA)
- Avoid the 10 anti-patterns from the page role system

---

#### SECTION 5: DRAFT COPY

Write the complete draft copy for every page in the structure. For each page:

**Page [N]: [Role Name]**

[Full draft copy]

*Visual note: [Brief direction for accompanying image/layout]*

Requirements for all copy:
- Follow every rule in the style guide: sentence character, tone rules, paragraph rhythm, product language, formatting conventions
- Use no banned phrases (reference the 130+ item banned list)
- Draw metaphors only from the 7 approved families
- Match the tone position from the brief throughout
- Vary sentence length; use one-sentence paragraphs as emphasis tools
- For Product Landing pages: describe what the product does, not what it is; place it in a world; let materials speak through effect; include product name, material, and price band reference
- For Invitation pages: maximum one CTA; restrained language; no urgency, false scarcity, or imperative commands
- Total word count should align with the page structure targets

---

#### SECTION 6: PRODUCT PLACEMENT LOGIC

For each product attached to this latazin, explain:

| Product | First Appearance (Page) | Role on That Page | Frequency Across Latazin | Placement Rationale |
|---|---|---|---|---|
| [Product name] | [Page number] | [How it appears — named, shown, described, contextual] | [How many pages it appears on] | [Why it appears here and in this way] |

Rules:
- No product should appear on every page (except in a Product Argument latazin focused on a single item)
- Products should be introduced through context before they receive a Product Landing page
- Hero products should appear earlier and more frequently than supporting products
- The first mention of any product should never be its price

---

#### SECTION 7: CTA LOGIC

Define the latazin's call to action:
- **CTA text:** [The exact words — must be restrained per the style guide's CTA restraint rules]
- **CTA placement:** [Which page — must be on the Invitation page]
- **CTA destination:** [Where it leads — product page, collection page, etc.]
- **CTA tone:** [Must match the overall tone position; never urgency-driven]

If the latazin type does not naturally include a CTA (e.g., Calendar Marking, Manifesto), state: "This latazin type does not include a direct CTA. The closest action pathway is: [describe indirect invitation]."

---

#### SECTION 8: OPTIONAL CUTDOWN IDEAS

If applicable, suggest 1–3 derivative content ideas that could be extracted from this latazin for other channels:

| Cutdown | Channel | What It Extracts | Format |
|---|---|---|---|
| [Name] | [Social / Email / Ad] | [Which page or element it repurposes] | [Brief description] |

These are optional — not every latazin needs cutdowns. Only suggest them if the content naturally lends itself to extraction without dilution.

---

#### SECTION 9: QUALITY SELF-CHECK

Before presenting the final output, evaluate your own work against every dimension of the quality rubric. Be honest — this is not a formality.

**Dimension 1: Editorial Feel**
- Does this read like editorial content or like a product listing with better adjectives?
- Score: [Publish / Revise / Rethink / Reject]
- Evidence: [Specific sentences or structural choices that support this score]

**Dimension 2: Product Meaning**
- Are products presented with context, differentiation, and real-world impact — or just described?
- Score: [Publish / Revise / Rethink / Reject]
- Evidence: [Specific product presentation choices]

**Dimension 3: Taste**
- Does the latazin demonstrate editorial judgment through what it includes, what it omits, and how it frames choices?
- Score: [Publish / Revise / Rethink / Reject]
- Evidence: [Specific selection or omission decisions]

**Dimension 4: Structural Persuasion**
- Does the page sequence build an arc? Does pacing create momentum without rushing?
- Score: [Publish / Revise / Rethink / Reject]
- Evidence: [Page sequence analysis]

**Dimension 5: Voice Consistency**
- Does every page sound like it was written by the same editorial sensibility? Is the tone position maintained?
- Score: [Publish / Revise / Rethink / Reject]
- Evidence: [Tone consistency examples]

**Dimension 6: Completeness & Craft**
- Is the latazin structurally complete? Are there loose threads, missing products, or unresolved premises?
- Score: [Publish / Revise / Rethink / Reject]
- Evidence: [Completeness assessment]

**Overall Assessment:** [Publish / Revise / Rethink / Reject]

**If any dimension scores below "Publish":** Identify the specific fix required and either apply it to the draft above or flag it clearly for the editor.

**Failure Pattern Check:**
Review the 8 common failure patterns from the quality rubric. Flag any that apply to this draft:
1. [ ] Catalogue voice bleeding into editorial
2. [ ] Frontloading products before establishing context
3. [ ] Generic metaphors not from approved families
4. [ ] Structural monotony (same page role repeated)
5. [ ] Tone drift across pages
6. [ ] Missing or weak premise
7. [ ] CTA that undermines editorial tone
8. [ ] Products described without material specificity

---

#### SECTION 10: POST-GENERATION REVIEW CHECKLIST

This checklist is for the human editor reviewing the generated latazin. Check each item before approving for publication:

**Content & Structure:**
- [ ] The latazin type matches the brief and the content actually follows that type's definition from the typology
- [ ] The page structure follows the arc principle (Ground → Show → Argue → Land → Invite)
- [ ] The page sequence respects all sequencing rules from the page role system
- [ ] The estimated page count is within range of the brief
- [ ] Every product from the brief appears in the latazin with at least one meaningful mention
- [ ] No product appears before context is established for it

**Voice & Style:**
- [ ] The tone position matches the brief specification throughout the entire piece
- [ ] No banned phrases from the style guide appear anywhere in the copy
- [ ] All metaphors come from the 7 approved metaphor families
- [ ] Sentence length varies; no run of more than 3 sentences of similar length
- [ ] Opening follows the style guide's opening logic (no questions, stats, "Introducing," or flattery)
- [ ] Product language describes what products do, not just what they are

**Audience & Objective:**
- [ ] The target persona's trust needs or objections are addressed (at least implicitly)
- [ ] The stated objective from the brief is served by the content — not just adjacent to it
- [ ] The latazin connects to the month thesis, quarterly objective, and annual thesis

**Commerce & Campaign:**
- [ ] If campaign support = Yes, the latazin references the collection thesis appropriately
- [ ] CTA (if present) is restrained, singular, and on the Invitation page
- [ ] No false urgency, scarcity language, or aggressive selling
- [ ] Price references (if any) follow the style guide's price handling rules

**Occasion & Season:**
- [ ] If tied to an occasion, the editorial posture is respected
- [ ] Seasonal grounding feels natural, not forced
- [ ] Month profile's emotional tone is reflected in the writing

**Quality Rubric Alignment:**
- [ ] The self-check in Section 9 is honest and specific — not all "Publish" with vague evidence
- [ ] Any dimensions scored below "Publish" have identified fixes
- [ ] No failure patterns from the rubric's list of 8 are present in the final draft

### CONSTRAINTS

- Do not generate any content that violates the style guide's banned phrases list — if in doubt, check the list
- Do not use metaphors outside the 7 approved families — if a metaphor doesn't clearly belong to a family, don't use it
- Do not exceed the brief's page count estimate by more than 2 pages
- Do not include more than one CTA per latazin
- Do not introduce products before establishing editorial context
- Do not mix more than 2 latazin types; if mixing, the secondary type must not exceed 30% of the content
- The output must be structured exactly as specified — not freeform prose with occasional headers
- Every section (1–10) must be completed; no section may be skipped or abbreviated
```

---

## Expected Output Format

The output must follow the exact section structure below. Freeform prose without structure is not acceptable.

```
# [Latazin Title] — [Latazin Type]

## Section 1: Concept
### Core Argument
[2–3 sentences]

### Editorial Angle
[1–2 sentences]

### Reader Takeaway
[1 sentence]

## Section 2: Title Options
1. [Title] — [Rationale]
2. [Title] — [Rationale]
3. [Title] — [Rationale]

**Recommended:** [Title number] — [Why]

## Section 3: Premise
[2–4 sentences]
*Metaphor family used: [Family name]*

## Section 4: Page Structure
| Page | Role | Content Summary | Word Count | Visual Direction |
|---|---|---|---|---|
| 1 | Premise | ... | ... | ... |
| 2 | ... | ... | ... | ... |
| ... | ... | ... | ... | ... |

## Section 5: Draft Copy

### Page 1: [Role Name]
[Full copy]
*Visual note: ...*

### Page 2: [Role Name]
[Full copy]
*Visual note: ...*

[Continue for all pages]

## Section 6: Product Placement Logic
| Product | First Appearance | Role | Frequency | Rationale |
|---|---|---|---|---|
| ... | ... | ... | ... | ... |

## Section 7: CTA Logic
- **Text:** ...
- **Placement:** ...
- **Destination:** ...
- **Tone:** ...

## Section 8: Optional Cutdown Ideas
| Cutdown | Channel | Extract | Format |
|---|---|---|---|
| ... | ... | ... | ... |

[Or: "No cutdowns recommended for this latazin."]

## Section 9: Quality Self-Check

### Dimension 1: Editorial Feel
- **Score:** [Tier]
- **Evidence:** ...

### Dimension 2: Product Meaning
- **Score:** [Tier]
- **Evidence:** ...

### Dimension 3: Taste
- **Score:** [Tier]
- **Evidence:** ...

### Dimension 4: Structural Persuasion
- **Score:** [Tier]
- **Evidence:** ...

### Dimension 5: Voice Consistency
- **Score:** [Tier]
- **Evidence:** ...

### Dimension 6: Completeness & Craft
- **Score:** [Tier]
- **Evidence:** ...

**Overall:** [Tier]
**Fixes required:** [List or "None"]

**Failure Pattern Flags:** [List any that apply or "None detected"]

## Section 10: Post-Generation Review Checklist
[Complete checklist with all items marked for editor review]
```

---

## Quality Self-Check Step

The quality self-check (Section 9) is not optional. It is built into the generation process to ensure that every latazin is evaluated before it reaches a human reviewer. The self-check must:

1. **Score every dimension** — all 6 dimensions from the quality rubric must receive a tier rating
2. **Provide evidence** — each score must cite specific sentences, structural choices, or content decisions from the draft
3. **Be honest** — a self-check that rates everything "Publish" without specific evidence is itself a quality failure
4. **Trigger revision** — if any dimension scores "Revise" or below, the generator must either fix the issue in the draft or clearly flag it for the editor with a specific recommendation
5. **Check failure patterns** — all 8 common failure patterns from the rubric must be checked against the draft

---

## Post-Generation Review Checklist

The review checklist (Section 10) is for human editors, not the AI generator. It provides a structured review framework covering:

- **Content & Structure** (7 items): Type compliance, page arc, sequencing, page count, product coverage, context-first ordering
- **Voice & Style** (6 items): Tone compliance, banned phrases, metaphor compliance, sentence variety, opening logic, product language
- **Audience & Objective** (3 items): Persona addressing, objective fulfillment, planning layer connection
- **Commerce & Campaign** (4 items): Collection integration, CTA restraint, no urgency language, price handling
- **Occasion & Season** (3 items): Posture respect, natural seasonality, emotional tone
- **Quality Rubric Alignment** (3 items): Self-check honesty, fix identification, failure pattern clearance

Total: 26 review items. A latazin should pass all 26 before publication. Items that fail should be returned to the generator with specific feedback referencing the relevant house-layer document.
