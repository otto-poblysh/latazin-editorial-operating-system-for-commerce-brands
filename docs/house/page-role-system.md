# Page Role System

## Purpose

This file defines the roles a page can play inside a latazin. A latazin is not a sequence of blank pages filled with content — it is a structured argument where every page serves a specific function. Without assigned roles, pages blur into each other, the argument flattens, and the latazin reads as a decorated product listing.

The page role system prevents two fundamental failures: pages that do the same thing consecutively (repetition) and pages that do nothing at all (filler). It ensures that every page advances the reader's understanding, shifts their perspective, or earns the next page's right to exist.

This file works in direct coordination with `commerce-latazin-typology.md` (which determines what types of latazins exist) and `style-guide.md` (which governs sentence-level execution within each page).

---

## How This File Is Used in the System

- **During generation:** The model receives page role assignments as part of the latazin brief or generates them as a structural step before writing. Each page's content is constrained by its assigned role — a premise page cannot do the work of an argument page, and a detail page cannot perform as an invitation.
- **During review:** Reviewers check that each page fulfils its assigned role and that the sequence of roles creates a coherent arc. A latazin where every page is an argument page, or where a detail page precedes the premise, is a structural failure.
- **During planning:** Planning documents may specify page-count ranges and required roles for different latazin types, ensuring that structural expectations are set before generation begins.
- **During prompt design:** Prompts embed role definitions and sequencing rules to prevent the model from producing structurally flat content.

---

## Complete Role Definitions

### 1. Premise

**What it does:** Establishes the reason the latazin exists. The premise page tells the reader what question, observation, or situation this content addresses. It grounds the reader before any product, argument, or detail appears. Without a premise, the latazin starts in the middle.

**When to use it:**
- Always. Every latazin needs a premise, whether it occupies a full page or the first section of the opening page.
- It is the first substantive page in any latazin (after a title card or cover image, if present).

**How to execute:**
- Open with a context the reader recognises — a season, a moment, a problem, a shift in how things are done
- State or imply the editorial question the latazin will answer
- Do not mention specific products on the premise page (exceptions: Product Argument latazins may name the product in the premise if the product *is* the premise)
- Keep the tone composed to warm. The premise earns attention through relevance, not excitement
- Aim for one strong paragraph or two short ones. The premise should be tight — it opens a door, it does not furnish the room

**Common mistakes:**
- Starting with the product instead of the context
- Writing a premise that could apply to any latazin ("We're excited to share something special")
- Making the premise too long — it becomes an essay before the argument begins
- Skipping the premise entirely and opening with a product image or detail

---

### 2. Witness

**What it does:** Shows evidence. A witness page presents something the reader can see, touch, or verify — a photograph, a scene, a close-up, a real-world setting. It says "look at this" before saying "here's what it means." The witness page earns trust through demonstration.

**When to use it:**
- After the premise, to ground the abstract in the concrete
- When a product, material, or setting needs to be *shown* before it is discussed
- In Craft Studies, to document process or materials
- In Community/Project latazins, to introduce real people or places

**How to execute:**
- Lead with image. The visual is the primary content; copy supports, it does not duplicate
- Use short, specific captions or observational copy: "The seam runs doubled across the shoulder. It takes thirty minutes longer per unit."
- Do not interpret the image in abstract terms. Describe what is visible and let the reader draw meaning
- The witness page builds the case for the argument page that follows

**Common mistakes:**
- Using a witness page as a product beauty shot with no editorial intent
- Writing long copy that competes with the image instead of supporting it
- Placing a witness page without a clear relationship to the premise or the argument
- Using stock-style imagery that fails to witness anything specific

---

### 3. Argument

**What it does:** Makes the case. The argument page is where the latazin takes a position and supports it. It is the editorial core — the page where the "why" is stated, defended, and made convincing. Not every latazin has an explicit argument page (image-forward types may distribute the argument across other roles), but most do.

**When to use it:**
- After the premise and at least one witness or context-setting page
- When the latazin needs to state a position ("This is the only bag worth considering for summer," "Handmade does not mean handmade the way you think")
- In Product Arguments, Misreading Corrections, and Manifestos, the argument page is central
- In Occasion and Collection/Drop types, the argument may be lighter but still present

**How to execute:**
- State the position clearly in the opening sentence of the page
- Support with specific evidence: materials, process, comparison, context, observed detail
- Build the case in 2–4 paragraphs with varied rhythm (see `style-guide.md`)
- Do not hedge. The argument page is where the latazin earns or loses authority
- Close the page with a sentence that lands — it should feel like a conclusion, even if the latazin continues

**Common mistakes:**
- Stating a position without evidence (assertion without argument)
- Stacking multiple unrelated arguments on one page (unfocused)
- Using the argument page to list product features instead of building a case
- Writing an argument so mild it says nothing ("This is a really well-made product")

---

### 4. Detail

**What it does:** Zooms in. The detail page examines a specific element — a material, a construction technique, a design choice, a single component — at close range. It rewards the reader who stays with specificity that broader pages cannot provide.

**When to use it:**
- After an argument or witness page has established the broader context
- When a specific feature, material, or decision deserves deeper examination
- In Craft Studies and Product Arguments, where precision builds credibility
- When the latazin needs to slow down and reward close attention

**How to execute:**
- Focus on one element per detail page. "The clasp" or "the lining" or "the glaze," not "the details"
- Use precise, material language: weight, texture, dimension, origin, comparison to alternatives
- If technical, translate for the reader: "Full-grain" means nothing alone; "Full-grain — the outermost surface, where the hide is densest" is information
- Pair with a close-up image when possible
- Keep copy lean. The detail page is about precision, not volume

**Common mistakes:**
- Cramming multiple details onto one page (becomes a feature list)
- Using vague language ("attention to detail," "quality craftsmanship") instead of specific observation
- Placing detail pages before the argument — detail without context is noise
- Making the detail page feel like a product specification sheet

---

### 5. Pause / Image-Only Rest

**What it does:** Creates breathing room. The pause page interrupts the editorial flow with a full-bleed image, a moment of visual stillness, or a minimal text-and-image combination that asks nothing of the reader except to look. It is a structural rest — a deliberate silence in the argument.

**When to use it:**
- Between two dense argument or detail pages
- After an emotionally or informationally heavy section
- When the latazin needs a tonal shift and the transition should be felt, not explained
- In longer latazins (8+ pages) where sustained reading requires visual relief

**How to execute:**
- Full-bleed image with no copy, or image with a single sentence or phrase
- The image should be editorially chosen — it creates atmosphere, not decoration
- No product callouts, price tags, or CTAs on a pause page
- The image should relate to the latazin's world but not repeat a previous page's image
- Duration: one page. A pause that extends to two consecutive pages is a structural gap, not a rest

**Common mistakes:**
- Using the pause page as filler — an image with no relationship to the editorial arc
- Placing a pause page at the beginning (before the reader has anything to rest from)
- Using a pause page to insert a promotional banner or unrelated cross-sell
- Including copy-heavy content disguised as a "visual break"

---

### 6. Invitation

**What it does:** Extends the editorial logic to the reader's life. The invitation page bridges the latazin's world and the reader's world. It does not hard-sell — it suggests, implies, or gently directs. "This exists. Here's how to find it." The invitation earns its place through the editorial work that precedes it.

**When to use it:**
- Near the end of the latazin, after the argument is complete
- When the latazin has a clear commercial intent and needs a graceful transition to action
- When the CTA (if present) needs editorial framing rather than appearing as a bare button
- In Occasion latazins, where the invitation connects the moment to the product

**How to execute:**
- Use warm, restrained language: "The collection is available now" rather than "Shop the collection!"
- Frame the invitation as a natural continuation: "If this is how you think about [the topic], the [product] is here"
- One CTA per invitation page, maximum. Often zero — the invitation is implicit
- The invitation page should feel like the latazin's final generous gesture, not a sales trap

**Common mistakes:**
- Placing the invitation too early (before the argument is complete — it feels premature)
- Using urgent or promotional language that breaks the editorial tone
- Including multiple products, links, or actions on the invitation page (overwhelm)
- Making the invitation page indistinguishable from a product landing page

---

### 7. Product Landing

**What it does:** Presents the product directly — name, image, key details, price (if appropriate). The product landing page is where commerce meets editorial. It exists to give the reader a clear, clean encounter with the product after the editorial argument has done its work.

**When to use it:**
- In Product Arguments, after the argument and detail pages
- In Bundle/World and Shop the Look latazins, as the page where individual products are clearly presented
- In Collection/Drop latazins, as the page where the collection's pieces are individually visible
- Not in every latazin — Calendar Markings, Manifestos, and some Community/Project latazins may have no product landing page

**How to execute:**
- Clean product image with clear visibility of the product
- Product name, one or two sentences of contextual description (not the full argument — that was made earlier)
- Price, if included, stated as fact (see `style-guide.md` handling of price)
- Link to product page, if applicable, presented without urgency
- Keep the page structured and uncluttered — the product has been argued for; this page delivers it

**Common mistakes:**
- Placing the product landing page before the editorial argument (catalogue logic)
- Overloading the page with copy that repeats the argument already made
- Including multiple products with no visual hierarchy or editorial ordering
- Making the product landing page indistinguishable from a standard e-commerce product tile

---

### 8. Proof

**What it does:** Provides external validation. The proof page brings in evidence from outside the editorial argument — sales figures, press recognition, customer testimony, third-party endorsement, or verifiable performance data. It shifts the voice from the brand's assertion to the world's confirmation.

**When to use it:**
- In Milestone/Proof latazins, as the structural centrepiece
- In Product Arguments, when the product has earned credible external validation
- After the argument page, as reinforcement (not before — proof without argument is empty)
- When the brand's claim needs third-party support to be convincing

**How to execute:**
- Use specific, verifiable evidence: "4,200 units sold in three weeks" rather than "incredibly popular"
- Direct customer quotes, attributed and unedited
- Press quotes with publication name and date
- Awards or recognition with the granting body named
- Keep the tone factual. Proof is evidence, not celebration. Let the numbers and quotes speak
- One or two proof points per page. Stacking diminishes credibility

**Common mistakes:**
- Using vague social proof ("Loved by thousands") instead of specific data
- Editing customer quotes to sound more like the brand's voice
- Placing proof before the argument (the reader hasn't been given context for what the proof means)
- Using proof as the emotional climax of the latazin (it should reinforce, not peak)

---

### 9. Contrast

**What it does:** Introduces a counterpoint. The contrast page shows what exists without the product, what the alternative looks like, what the previous standard was, or what the common approach gets wrong. It creates meaning through difference — the product or position gains definition by being placed against what it is not.

**When to use it:**
- In Misreading Correction latazins, where the misreading is the contrast to the corrected understanding
- In Product Arguments, where the product is best understood against its alternatives
- In Manifestos, where the brand's position is sharpened by identifying what it rejects
- When the latazin needs to create tension or stakes before resolving them

**How to execute:**
- Be fair. The contrast is not a straw man — describe the alternative honestly
- Use specific examples: "Most bags in this category use bonded leather because it's cheaper to source" rather than "Other brands cut corners"
- The contrast page creates the problem or gap that the subsequent argument or product resolves
- Place before the argument or product landing page, so the resolution follows naturally
- Keep the tone observational, not dismissive

**Common mistakes:**
- Naming competitors directly (the contrast should be about approaches, not brands)
- Making the contrast unfairly one-sided (undermines credibility)
- Spending more time on the contrast than on the resolution (the latazin becomes negative)
- Using the contrast page as an excuse for generic "most people get this wrong" language

---

### 10. Atmosphere

**What it does:** Builds mood. The atmosphere page creates an immersive, sensory environment that the reader inhabits briefly. It uses language and imagery to establish a feeling — seasonal, spatial, emotional, or sensory — that colours everything that follows. It is not an argument, and it is not a pause. It actively constructs a world.

**When to use it:**
- In Bundle/World latazins, where the world is the editorial product
- In Occasion latazins, where the moment needs to be felt, not just described
- At the beginning of a latazin (after the premise) to immerse the reader before the argument
- In longer latazins, between sections, to re-establish the editorial world

**How to execute:**
- Use sensory, concrete language: light quality, temperature, texture, sound, spatial arrangement
- The atmosphere page describes a scene or state, not an idea: "Linen on the table. The window is open. The wind does what it does"
- Images and copy work together to create immersion — neither dominates
- Do not explain the atmosphere's purpose. The reader does not need to know why the mood is being built
- Keep it short. Atmosphere is effective in concentrated doses; extended, it becomes self-indulgent

**Common mistakes:**
- Using atmosphere as decoration — beautiful but disconnected from the latazin's argument
- Writing atmosphere copy that is vague ("a vibe," "an energy," "a feeling") instead of specific
- Stacking multiple atmosphere pages consecutively (mood without structure)
- Confusing atmosphere with aspiration ("imagine yourself in a beautiful home") — atmosphere is present tense, not aspirational

---

## Page Sequencing Guidance

### The Arc Principle

Every latazin has an arc. Pages are not interchangeable — their order creates meaning. The fundamental arc is:

**Ground → Show → Argue → Land → Invite**

This translates to:

1. **Premise** — Establish why we are here
2. **Witness / Atmosphere** — Show the world or the evidence
3. **Argument / Detail / Contrast** — Make the case
4. **Product Landing / Proof** — Deliver the product or evidence
5. **Invitation** — Extend to the reader's life

Not every latazin uses every role, and not every latazin follows this exact sequence. But deviation should be deliberate, not accidental.

### Sequencing Rules

- **Premise always comes first** (or second, after a title/cover page). There is no exception. A latazin that starts with a product landing page has no editorial value.
- **Argument comes after context.** The reader needs grounding (premise, witness, atmosphere) before the argument will land. An argument on page one is a claim without foundation.
- **Detail follows argument.** Zooming in before the broad case is made confuses the reader — they don't know what they are looking at or why it matters.
- **Product landing follows argument or detail.** The product appears after it has been contextualised, argued for, or examined. Never before.
- **Proof follows argument.** External validation reinforces a case already made. Proof before argument is a testimonial page, not editorial.
- **Pause pages require something to pause from.** They appear between dense sections, never at the beginning or end.
- **Invitation comes near the end.** It is the latazin's closing gesture. Placing it in the middle undermines both the remaining content and the invitation itself.
- **Contrast comes before resolution.** A contrast page after the argument and product landing creates an awkward anticlimax.

### Permitted Sequences (Examples)

| Sequence | Suited for |
|---|---|
| Premise → Witness → Argument → Detail → Product Landing → Invitation | Product Argument (standard) |
| Premise → Atmosphere → Witness → Argument → Product Landing → Invitation | Bundle/World, Occasion |
| Premise → Witness → Detail → Detail → Argument → Product Landing | Craft Study |
| Premise → Contrast → Argument → Proof → Invitation | Misreading Correction |
| Premise → Argument → Pause → Argument → Invitation | Manifesto |
| Premise → Atmosphere → Product Landing → Product Landing → Pause → Product Landing → Invitation | Shop the Look |
| Premise → Witness → Argument → Proof → Invitation | Milestone/Proof |
| Premise → Atmosphere → Witness → Witness → Invitation | Calendar Marking |
| Premise → Witness → Argument → Detail → Witness → Product Landing → Invitation | Collaboration |

---

## Minimum and Recommended Page Structures

### Minimum Viable Structures (by Type)

Every latazin type has a minimum set of page roles required for structural integrity. Below the minimum, the latazin cannot fulfil its type's intent.

| Latazin Type | Minimum Pages | Required Roles |
|---|---|---|
| Product Argument | 4 | Premise, Argument, Product Landing, Invitation |
| Bundle/World | 5 | Premise, Atmosphere, Product Landing ×2, Invitation |
| Craft Study | 5 | Premise, Witness, Detail, Argument, Product Landing |
| Occasion | 4 | Premise, Atmosphere, Product Landing, Invitation |
| Misreading Correction | 4 | Premise, Contrast, Argument, Invitation |
| Manifesto | 3 | Premise, Argument, Invitation |
| Collection/Drop | 5 | Premise, Argument, Product Landing ×2, Invitation |
| Calendar Marking | 3 | Premise, Atmosphere or Witness, Invitation |
| Collaboration | 5 | Premise, Witness, Argument, Product Landing, Invitation |
| Shop the Look | 4 | Premise, Product Landing ×2, Invitation |
| Community/Project | 4 | Premise, Witness, Argument or Proof, Invitation |
| Milestone/Proof | 4 | Premise, Argument, Proof, Invitation |

### Recommended Structures (by Type)

Recommended structures represent the ideal page count and role distribution for a strong latazin of each type.

| Latazin Type | Recommended Pages | Recommended Role Sequence |
|---|---|---|
| Product Argument | 6–8 | Premise → Witness → Argument → Detail → Pause → Product Landing → Invitation |
| Bundle/World | 7–10 | Premise → Atmosphere → Witness → Product Landing → Pause → Product Landing → Product Landing → Atmosphere → Invitation |
| Craft Study | 6–9 | Premise → Witness → Detail → Detail → Pause → Argument → Product Landing → Invitation |
| Occasion | 5–7 | Premise → Atmosphere → Argument → Product Landing → Pause → Product Landing → Invitation |
| Misreading Correction | 5–7 | Premise → Contrast → Argument → Detail → Proof → Invitation |
| Manifesto | 5–7 | Premise → Argument → Pause → Argument → Witness → Invitation |
| Collection/Drop | 6–10 | Premise → Atmosphere → Argument → Product Landing → Product Landing → Pause → Product Landing → Invitation |
| Calendar Marking | 3–5 | Premise → Atmosphere → Witness → Atmosphere → Invitation |
| Collaboration | 6–8 | Premise → Witness → Argument → Detail → Witness → Product Landing → Invitation |
| Shop the Look | 5–8 | Premise → Atmosphere → Product Landing → Product Landing → Pause → Product Landing → Product Landing → Invitation |
| Community/Project | 5–7 | Premise → Witness → Witness → Argument → Proof → Invitation |
| Milestone/Proof | 5–7 | Premise → Argument → Proof → Witness → Proof → Invitation |

---

## Anti-Patterns (Bad Page Sequencing)

### 1. The Catalogue Sequence

**Pattern:** Product Landing → Product Landing → Product Landing → Product Landing

**Why it fails:** No premise, no argument, no context. The reader is presented with products but given no reason to care. This is a catalogue page, not a latazin. Every product landing page requires preceding editorial work (premise, argument, atmosphere, witness) to justify its presence.

### 2. The Premature Product

**Pattern:** Premise → Product Landing → Argument → Detail

**Why it fails:** The product appears before the argument is made. The reader sees the product before understanding why it matters. The argument, arriving after the product, reads as retroactive justification — a sales rationalisation, not an editorial position.

### 3. The Endless Argument

**Pattern:** Premise → Argument → Argument → Argument → Argument → Invitation

**Why it fails:** Multiple consecutive argument pages without relief — no witness, no detail, no pause, no product. The reader is lectured without evidence, variation, or rest. The latazin reads as an essay, not editorial commerce content.

### 4. The False Start

**Pattern:** Atmosphere → Atmosphere → Premise → Argument

**Why it fails:** Two consecutive atmosphere pages before the premise delay the reader's orientation. The reader experiences mood without understanding context. One atmosphere page after the premise is immersion; two atmosphere pages before the premise is confusion.

### 5. The Buried Premise

**Pattern:** Product Landing → Witness → Premise → Argument

**Why it fails:** The premise is buried on page three or later. The reader encounters products and images without context. By the time the premise arrives, the reader has already formed their own (likely wrong) interpretation of the latazin's purpose.

### 6. The Afterthought Invitation

**Pattern:** Premise → Argument → Invitation → Detail → Product Landing

**Why it fails:** The invitation arrives in the middle, then the latazin continues. The reader receives the "closing gesture" and then encounters more content. This undermines both the invitation (premature) and the remaining content (anticlimactic).

### 7. The Proof-First Failure

**Pattern:** Proof → Premise → Argument → Product Landing

**Why it fails:** Proof before context is meaningless — "4,200 sold in three weeks" means nothing if the reader doesn't yet know what the product is or why it matters. Proof reinforces an argument already made; it cannot precede one.

### 8. The Pauseless Marathon

**Pattern:** Premise → Argument → Detail → Detail → Argument → Detail → Product Landing → Product Landing → Invitation

**Why it fails:** Nine pages with no visual rest. The reader experiences fatigue. Dense content requires structural relief. Any latazin over six pages should include at least one pause or atmosphere page.

### 9. The Role Repetition

**Pattern:** Witness → Witness → Witness → Witness

**Why it fails:** Four consecutive witness pages become a photo gallery, not editorial content. Each page shows evidence but no page interprets it. The reader sees but does not understand. Witness pages need argument, detail, or atmosphere pages between them to create meaning.

### 10. The Disconnected Contrast

**Pattern:** Premise → Argument → Product Landing → Contrast → Invitation

**Why it fails:** The contrast arrives after the product has already been presented. It introduces a problem or alternative that the reader has already moved past. Contrast creates tension that the argument resolves — placing it after the resolution creates anticlimax.

---

## Maintenance Notes

Review this file when:

- New latazin types are added to the typology that may require new page roles or different minimum structures
- Generated content consistently misuses page roles, suggesting definitions or sequencing rules need clarification
- New page roles emerge from editorial practice that are not covered by the existing ten roles
- The quality rubric (`quality-rubric.md`) is updated to include structural criteria that reference page roles
- Reviewer feedback indicates that page role boundaries are unclear (e.g., confusion between atmosphere and pause, or between witness and detail)
- Latazin page counts change significantly due to platform or format changes, requiring adjusted minimum and recommended structures
