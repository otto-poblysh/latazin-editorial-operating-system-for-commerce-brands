# Quality Rubric

## Purpose

This file defines the approval standards for all editorial output produced by the Latazin system: latazins, prompts, calendars, and strategy documents.

The rubric answers four core questions:

1. Does this feel editorial rather than promotional?
2. Does this create product meaning rather than product noise?
3. Is it taste-forward?
4. Does it persuade with structure rather than hype?

Every piece of content the system generates should be evaluated against these standards before publication. The rubric is not a style preference — it is a quality gate.

---

## How this file is used in the system

- **During generation:** The latazin content generation prompt includes a self-check step where the model evaluates its own output against this rubric before presenting the final draft. This catches obvious failures before human review.
- **During review:** Human reviewers use this rubric as the primary evaluation framework. Each dimension has clear criteria so reviewers can assess consistently, regardless of the reviewer.
- **During planning:** Annual strategies, quarterly plans, and monthly calendars are evaluated against the planning-specific rubric sections to ensure strategic documents meet the same editorial standard as the content they produce.
- **During prompt refinement:** When prompts are revised, the rubric is the success criterion. A prompt change is justified only if it produces output that scores better against this rubric.

---

## Evaluation Dimensions

All content is evaluated across six dimensions. Each dimension has a clear definition, scoring criteria, and failure indicators.

---

### Dimension 1: Editorial Feel

**Definition:** The content reads as editorial rather than promotional. It sounds like it belongs in a magazine, a considered publication, or a curated storefront — not in a promotional email, a product listing, or a social media ad.

**Pass criteria:**

- [ ] Opens with a premise, observation, or context — not a product name or sales pitch
- [ ] Maintains a consistent, composed voice throughout — no sudden shifts to hype or hard sell
- [ ] Uses paragraph structure and sentence rhythm, not bullet-point feature lists
- [ ] CTAs, if present, feel like natural conclusions, not inserted sales mechanics
- [ ] The reader could engage with the writing even if they do not intend to buy
- [ ] The content rewards attention — it is not designed purely for scanning

**Fail indicators:**

- Opens with the product name, price, or a promotional hook ("Don't miss out!")
- Contains more than two CTAs, or CTAs that interrupt the editorial flow
- Uses exclamation marks as a substitute for compelling content
- Reads like a product description with extra paragraphs added around it
- Could be swapped onto any other brand's site without feeling out of place

---

### Dimension 2: Product Meaning

**Definition:** The content creates meaning around the product — it does not just describe or list the product. After reading, the reader understands not just what the product is, but why it matters, where it belongs, and what it replaces.

**Pass criteria:**

- [ ] The product is placed in a world: a season, a city, an occasion, a way of living
- [ ] At least one material or construction detail is given that the reader could not guess from a photograph alone
- [ ] The product is connected to a need, a desire, or a cultural moment — not presented in isolation
- [ ] The reader understands what changes in their life if they own this product
- [ ] The product is differentiated from alternatives, either explicitly or through the specificity of description

**Fail indicators:**

- The product is described only in adjectives ("beautiful," "stunning," "luxurious") without material grounding
- The product floats in a void — no context, no season, no occasion, no pairing
- Features are listed without being connected to experiences
- The product could be replaced with any similar product without changing the copy
- The copy tells the reader the product is meaningful without showing why

---

### Dimension 3: Taste

**Definition:** The content demonstrates taste rather than claiming it. Taste is visible in what is selected, what is omitted, what is compared, and what is referenced. It is not a label the content applies to itself.

**Pass criteria:**

- [ ] Selections are made — the content features specific products, pairings, or combinations, not everything available
- [ ] References (cultural, material, seasonal) are specific and genuinely illuminate the product
- [ ] The language itself demonstrates care — word choices are precise, not generic
- [ ] The content omits what is unnecessary — no filler, no padding, no repetition for emphasis
- [ ] The reader finishes with a clearer sense of what the brand values and why

**Fail indicators:**

- The content uses the word "curated" or "taste" without demonstrating either
- References are generic or decorative ("inspired by nature," "timeless elegance")
- The content tries to include too much — too many products, too many messages, too many adjectives
- The language is interchangeable with any mid-market brand's social media copy
- The content claims sophistication rather than exhibiting it

---

### Dimension 4: Structural Persuasion

**Definition:** The content persuades through structure — through the order in which ideas appear, the pacing between sections, the relationship between text and image, and the rhythm of the argument. It does not rely on a single sentence, a discount, or emotional manipulation.

**Pass criteria:**

- [ ] The latazin or document has a clear structural arc: opening, development, evidence, resolution
- [ ] Pages or sections serve distinct roles (premise, argument, detail, rest, invitation) — not repetitive blocks
- [ ] The product appears at the right point in the sequence — after context has been established, not before
- [ ] Pacing varies — there are moments of density and moments of rest
- [ ] The reader arrives at the product feeling informed and prepared, not ambushed or pressured

**Fail indicators:**

- The content has no discernible structure — sections could be reordered without consequence
- Every page or section does the same thing (describe product, add adjective, insert CTA)
- The product appears immediately with no context, premise, or buildup
- There is no variation in pacing — every paragraph is the same length, every section the same density
- The conclusion is a hard sell rather than a natural culmination of the editorial argument

---

### Dimension 5: Voice Consistency

**Definition:** The content maintains the Latazin editorial voice as defined in `house-voice.md`. It sounds like the system, not like generic copy, social media content, or a different brand entirely.

**Pass criteria:**

- [ ] The tone is within the operating range defined in the voice file (restrained to inviting, never cold or gushing)
- [ ] The content does not use language from the anti-pattern list in `house-metaphors.md`
- [ ] Adjectives are earned — each one adds information, not just intensity
- [ ] The reader is treated as an intelligent adult, not spoken down to or hyped at
- [ ] The content could not have been written by any brand — it reflects a specific editorial posture

**Fail indicators:**

- The tone shifts mid-piece from editorial to promotional
- Social media language appears ("obsessed," "iconic," "you need this")
- The reader is told how to feel rather than given reasons to feel
- Sentences rely on exclamation marks, ALL CAPS, or emoji for energy
- The content sounds like it was generated without voice constraints

---

### Dimension 6: Completeness and Craft

**Definition:** The content is finished, not just drafted. It has been through an editorial process (human or automated) that catches errors, tightens language, and ensures every element serves a purpose.

**Pass criteria:**

- [ ] No spelling, grammar, or punctuation errors
- [ ] No unresolved placeholder text, incomplete sections, or visible template artifacts in the content being reviewed
- [ ] Product names, prices, and details are accurate and consistent
- [ ] Image direction (if included) is specific enough to guide photography or selection
- [ ] The content is the right length for its type — not padded, not truncated

**Fail indicators:**

- Contains "[insert X here]" or similar unresolved placeholder text in the final output
- Sections are obviously padded to meet a length requirement
- Product details contradict each other or are vaguely stated
- The content feels like a first draft — functional but unpolished
- Image direction is vague ("beautiful lifestyle shot") rather than specific

---

## Rubric for Latazins

A latazin is the primary content unit of the system. It is evaluated against all six dimensions above, plus the following latazin-specific criteria.

### Structural requirements

| Element | Requirement | Pass/Fail |
|---|---|---|
| **Concept** | The latazin has a stated concept that goes beyond "showcase product X" | ☐ |
| **Title** | The title is specific, editorial, and not a product name or generic label | ☐ |
| **Premise** | The opening page establishes context before introducing any product | ☐ |
| **Page roles** | Each page serves a distinct role (per `page-role-system.md`), not a repeated format | ☐ |
| **Product placement** | Products are introduced after context, not before | ☐ |
| **Visual direction** | Image guidance is specific: mood, angle, context, environment — not just "product shot" | ☐ |
| **CTA logic** | The CTA appears at a natural conclusion point, feels earned, and uses restrained language | ☐ |
| **Arc** | The latazin has a beginning, middle, and end — it is not a flat sequence of product pages | ☐ |
| **Length** | The page count is appropriate for the latazin type and does not feel padded or rushed | ☐ |

### Quality tiers

| Tier | Description | Action |
|---|---|---|
| **Publish** | Passes all six dimensions. Structural requirements met. Voice is consistent. Demonstrates taste and editorial intelligence. | Approve for publication. |
| **Revise** | Passes most dimensions but has specific, identifiable weaknesses. Structure is sound but execution needs tightening. | Return with specific revision notes keyed to rubric dimensions. |
| **Rethink** | Fails on two or more dimensions. Structural problems or fundamental voice drift. The concept may be viable but the execution is not. | Return with structural feedback. May need re-generation from brief. |
| **Reject** | Fails on multiple dimensions. Reads as promotional, generic, or structurally incoherent. Does not represent the system's standards. | Discard. Re-evaluate the brief and prompt inputs. |

---

## Rubric for Planning Documents

Planning documents include annual strategies, quarterly plans, and monthly editorial calendars. They are evaluated differently from latazins because their purpose is strategic direction, not reader-facing prose.

### Annual strategy evaluation

| Criterion | Pass | Fail |
|---|---|---|
| **Thesis clarity** | The annual thesis is stated in one to two sentences and is specific to the brand and year | The thesis is generic ("grow the brand") or absent |
| **Quarterly differentiation** | Each quarter has a distinct strategic emphasis, not four repetitions of the same plan | All quarters say the same thing with different seasonal labels |
| **Product logic** | Products and collections are distributed across the year with stated reasoning | Products are assigned randomly or concentrated without justification |
| **Audience awareness** | Audience priorities shift across the year based on seasonal or cultural logic | Same audience description pasted into every quarter |
| **Latazin type balance** | Multiple latazin types are used across the year, with reasoning for the mix | Only one or two latazin types appear, or types are assigned without rationale |
| **Risk acknowledgment** | Key risks or uncertainties are named | The plan assumes everything will go perfectly |
| **Measurability** | Success criteria are stated for each quarter | No way to evaluate whether the plan worked |

### Quarterly plan evaluation

| Criterion | Pass | Fail |
|---|---|---|
| **Specificity** | Named products, specific latazin types, and concrete launch windows | Vague references to "key products" and "important moments" |
| **Connection to annual strategy** | The quarter clearly advances the annual thesis and addresses its assigned priorities | The quarter ignores or contradicts the annual strategy |
| **Calendar awareness** | Specific months, occasions, and cultural moments are referenced | Generic seasonal language without specific dates or events |
| **Feasibility** | The plan accounts for production capacity and does not over-schedule | More content is planned than could reasonably be produced |
| **Competitive awareness** | The plan acknowledges the commercial landscape without being reactive | The plan exists in a vacuum or is purely reactive to competitors |

### Monthly calendar evaluation

| Criterion | Pass | Fail |
|---|---|---|
| **Latazin specificity** | Each planned latazin has a type, concept, product attachment, and timing | Entries are vague ("publish something about summer") |
| **Pacing** | Content is distributed across the month with intentional rhythm, not front-loaded or random | All content clustered in one week, or evenly spaced without editorial logic |
| **Variety** | Multiple latazin types and product categories appear across the month | The month is a repetitive sequence of the same content type |
| **Occasion integration** | Relevant occasions and cultural moments are incorporated with specific content plans | Occasions are listed but not connected to specific latazins |
| **Connection to quarterly plan** | The month advances the quarter's priorities | The month ignores the quarterly plan |
| **Review questions** | The calendar includes self-assessment questions for the editorial team | No mechanism for evaluating whether the month's plan is working |

---

## Rubric for Prompts

Prompts are the instructions that drive content generation. A poorly written prompt produces content that fails the rubric, regardless of the model's capability. Prompts are evaluated on their ability to produce rubric-passing output.

### Prompt evaluation criteria

| Criterion | Pass | Fail |
|---|---|---|
| **Clarity of task** | The prompt states exactly what it wants the model to produce, in what format, and for what purpose | The prompt is vague about what output looks like |
| **Voice integration** | The prompt explicitly references or incorporates the house voice constraints | The prompt does not mention voice, leaving tone to chance |
| **Rubric awareness** | The prompt includes a self-check step or references the quality rubric | The prompt has no quality gate — it asks for output without evaluation |
| **Input specificity** | The prompt specifies what inputs the model should use (products, audiences, season, occasion) | The prompt asks the model to generate content from nothing |
| **Anti-pattern prevention** | The prompt explicitly names what the output should avoid (per metaphor and voice files) | The prompt only describes what it wants, not what it prohibits |
| **Structural guidance** | The prompt specifies the structural requirements of the output (sections, page roles, sequence) | The prompt asks for "a latazin" without structural direction |
| **Length calibration** | The prompt specifies approximate length or page count appropriate to the content type | The prompt has no length guidance, producing output that is too long or too short |
| **Testability** | The prompt's success can be evaluated against the rubric — a reviewer can tell if the output meets the prompt's intent | The prompt is so vague that almost any output could be considered a valid response |

### Prompt quality tiers

| Tier | Description | Action |
|---|---|---|
| **Production-ready** | Consistently produces output that passes the rubric across multiple runs. Integrates voice, structure, and anti-patterns. | Deploy in the system. |
| **Needs refinement** | Produces acceptable output most of the time but occasionally drifts on voice, structure, or specificity. | Revise specific sections and re-test. |
| **Needs redesign** | Produces output that regularly fails two or more rubric dimensions. Structural issues in the prompt itself. | Rewrite the prompt from the brief stage. |

---

## Common Failure Patterns

These are the most frequently observed failures across all content types. Recognizing these patterns speeds up review and helps prompt designers prevent them.

### 1. The decorated product listing

**What it looks like:** A product description with adjectives and atmospheric language layered on top, but no real editorial structure, context, or argument.

**Why it fails:** It fails on editorial feel, product meaning, and structural persuasion. The product is still a listing — it just has more words around it.

**How to fix it:** Start from the premise, not the product. Ask: what question does this latazin answer? What world does the product enter? What changes for the reader?

### 2. The tone shift

**What it looks like:** Content that starts editorially but suddenly shifts to promotional language — often near the product reveal or CTA. The opening sounds like a magazine; the closing sounds like an email blast.

**Why it fails:** It fails on voice consistency and editorial feel. The reader feels the shift and loses trust.

**How to fix it:** Ensure the CTA is written in the same voice as the rest of the piece. The closing should feel like the editorial conclusion it is, not a sales department insertion.

### 3. The adjective pile

**What it looks like:** Products described with stacked adjectives — "luxurious, buttery-soft, premium Italian leather" — where one precise detail would be more effective.

**Why it fails:** It fails on taste and voice consistency. Adjective stacking is a sign of generic copy, not editorial precision.

**How to fix it:** Pick the single most revealing detail. Replace the pile with one sentence that shows the quality rather than asserting it.

### 4. The contextless product

**What it looks like:** A product introduced without any world around it — no season, no occasion, no pairing, no cultural reference, no reason for now.

**Why it fails:** It fails on product meaning and structural persuasion. The product floats in a void, and the reader has no framework for wanting it.

**How to fix it:** Before writing about the product, answer: When would someone use this? Where? With what? Why now, specifically?

### 5. The everything latazin

**What it looks like:** A latazin that tries to include too many products, too many messages, too many themes, and too many CTAs. It has no focus.

**Why it fails:** It fails on taste (no selection), structural persuasion (no arc), and editorial feel (reads like a catalogue page).

**How to fix it:** Define the latazin's single concept. Select two to four products maximum. Build one argument, not five.

### 6. The generic strategy

**What it looks like:** A planning document that uses vague language — "leverage key moments," "engage our audience," "drive growth" — without specific products, dates, latazin types, or measurable outcomes.

**Why it fails:** It fails the planning rubric on specificity, measurability, and connection to the editorial system.

**How to fix it:** Name the products. Name the latazin types. Name the dates. Name the audiences. Replace every generic verb with a specific action.

### 7. The unconstrained generation

**What it looks like:** Generated content that reads reasonably well in isolation but has no connection to the house voice, approved metaphor families, or structural requirements.

**Why it fails:** It fails on voice consistency and often on taste. The content is generic — competent but characterless.

**How to fix it:** The prompt needs revision. Ensure voice constraints, metaphor families, and structural requirements are explicitly injected into the generation prompt.

### 8. The false depth

**What it looks like:** Content that uses philosophical or literary language to describe ordinary products, creating a mismatch between the weight of the language and the product it describes.

**Why it fails:** It fails on taste and voice consistency. The reader senses the gap between the language and the product, and trust erodes.

**How to fix it:** Match language weight to product weight. A basic t-shirt does not need existential framing. A well-made jacket with interesting construction details deserves close attention. Calibrate the depth to the product.

---

## Using the Rubric in Practice

### For reviewers

1. Read the content once without the rubric — note your instinctive reaction.
2. Read it a second time, evaluating each dimension.
3. Mark each checklist item as pass or fail.
4. Identify the primary failure dimension (if any) and write specific revision notes tied to that dimension.
5. Assign a quality tier.

### For prompt designers

1. After drafting a prompt, generate three to five sample outputs.
2. Evaluate each sample against the full rubric.
3. Identify which dimensions fail most frequently — these indicate prompt weaknesses.
4. Revise the prompt to address the weakest dimensions.
5. Re-generate and re-evaluate until samples consistently pass.

### For the generation self-check

The generation prompt should include a step where the model evaluates its own draft against a simplified version of the rubric:

1. Does this open with context, not product?
2. Is the product placed in a world?
3. Are adjectives earned?
4. Does the structure have an arc?
5. Is the voice consistent throughout?
6. Would the reader engage even without intent to buy?

If the self-check identifies failures, the model should revise before presenting the final output.

---

## Maintenance Notes

This file should be reviewed when:

- New content types or latazin types are added to the system
- Reviewers consistently disagree on quality assessments, suggesting unclear criteria
- Common failure patterns evolve as the system matures
- Prompt improvements produce output that exposes gaps in the rubric
- New evaluation dimensions emerge from production experience

The rubric should be tightened over time, not loosened. As the system matures, passing standards should rise. The goal is to make the lowest-quality approved content better than most brands' best content.
