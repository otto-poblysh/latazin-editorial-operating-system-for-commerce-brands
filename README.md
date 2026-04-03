# Latazin Editorial Operating System for Commerce Brands

A structured editorial system for helping commerce brands create taste-forward, story-led, high-conversion content with Latazin.

This repository exists to turn product marketing into editorial practice.

Instead of treating products as isolated catalogue entries, this system helps brands publish them as stories, worlds, arguments, occasions, collaborations, and cultural artifacts. It is designed for commerce brands that want to sell through taste, context, and meaning — not just through flat product listings.

---

## What this repository is for

This repository is the operating system behind the editorial side of Latazin for commerce brands.

It helps teams define:

- how a brand should sound
- what kinds of latazins it should create
- how products, collections, occasions, and campaigns should be organized
- how annual and quarterly editorial strategy should be generated
- how monthly editorial calendars should be produced
- how individual latazins should be developed from strategic inputs

This is not just a prompt library. It is a structured system of editorial logic, planning, and generation.

---

## Core idea

Latazin is not built around product listings as the primary customer surface.

The public surface is the **latazin**.

Products live inside stories.

That means a commerce brand on Latazin should not ask:

- “How do we post products?”
- “How do we upload a catalogue?”

It should ask:

- What world does this product belong to?
- What kind of argument does this product make?
- What occasion, ritual, or identity does it serve?
- What kind of reader should this story persuade?
- What sequence of latazins should shape perception over time?

This repository exists to answer those questions systematically.

---

## Who this is for

This system is for:

- fashion brands
- accessories brands
- footwear brands
- fragrance and beauty brands
- art and collectible brands
- book, print, and culture-led commerce brands
- luxury-adjacent and taste-forward small businesses
- editorial strategists building systems for commerce storytelling
- teams operating Latazin-powered storefronts and kiosks

It is especially relevant for brands that sell:

- non-perishable products
- relatively lightweight goods
- visually expressive goods
- culturally meaningful goods
- premium or luxury-adjacent goods
- products that benefit from context, narrative, and sequencing

---

## What this repository contains

The system is organized into four layers:

1. **House documents**  
   These define the editorial worldview, voice, metaphors, style, and approval standards.

2. **Input documents**  
   These define what exists to talk about: products, collections, months, occasions, audiences, and prior performance.

3. **Planning documents**  
   These generate annual strategy, quarterly planning, and monthly editorial calendars.

4. **Generation documents**  
   These generate the actual content for each individual latazin.

---

## Repository structure

```text
latazin-editorial-operating-system-for-commerce-brands/
├── README.md
├── docs/
│   ├── house/
│   │   ├── house-metaphors.md
│   │   ├── house-voice.md
│   │   ├── quality-rubric.md
│   │   ├── style-guide.md
│   │   ├── commerce-latazin-typology.md
│   │   └── page-role-system.md
│   ├── inputs/
│   │   ├── product-catalogue.md
│   │   ├── collections-and-drops.md
│   │   ├── month-profiles.md
│   │   ├── occasions-and-celebrations.md
│   │   ├── audience-personas.md
│   │   └── previous-performance-log.md
│   ├── planning/
│   │   ├── annual-editorial-strategy-prompt.md
│   │   ├── quarterly-editorial-planning-prompt.md
│   │   ├── monthly-editorial-calendar-prompt.md
│   │   └── latazin-content-generation-prompt.md
│   └── references/
│       ├── campaign-pattern-library.md
│       ├── reference-library.md
│       └── examples/
├── templates/
│   ├── annual-plan-template.md
│   ├── quarterly-plan-template.md
│   ├── monthly-calendar-template.md
│   ├── latazin-brief-template.md
│   └── launch-strategy-template.md
├── brands/
│   ├── _sample-brand/
│   └── sterling-stitches/
├── prompts/
│   ├── system/
│   ├── planning/
│   └── generation/
└── CHANGELOG.md
```

---

## The house layer

The house layer defines how the system thinks and sounds.

These files are meant to remain relatively stable across brands.

### `house-metaphors.md`
Defines the metaphor families the system prefers.

These metaphors should belong to the world of commerce, taste, sequence, ritual, materiality, perception, atmosphere, and public meaning.

This file exists to prevent lazy, generic, or mismatched language.

### `house-voice.md`
Defines the overall character of the writing.

This should answer:

- How does Latazin sound?
- What kind of intelligence should it project?
- What kind of restraint should it maintain?
- How should it differ from generic e-commerce copy?

### `quality-rubric.md`
Defines the standards for approving a latazin, prompt, calendar, or strategy.

This should help answer:

- Does this feel editorial rather than promotional?
- Does this create product meaning rather than product noise?
- Does it feel taste-forward?
- Does it persuade with structure rather than hype?

### `style-guide.md`
Defines the writing rules.

This should govern:

- sentence character
- tone
- paragraph rhythm
- opening logic
- product language
- cliché avoidance
- CTA restraint
- handling of price, urgency, and proof

### `commerce-latazin-typology.md`
Defines the types of latazins the system can create.

This is one of the most important files in the repo.

It should document the major classes of commerce latazins, such as:

- Product Argument
- Bundle / World
- Craft Study
- Occasion
- Misreading Correction
- Manifesto
- Collection / Drop
- Calendar Marking
- Collaboration
- Shop the Look
- Community / Project
- Milestone / Proof

Each type should explain:

- what it does
- when to use it
- what it is best for
- what weak use cases look like
- how it differs from related types

### `page-role-system.md`
Defines the roles a page can play inside a latazin.

This helps the system avoid treating a latazin as a series of blank pages.

Typical page roles may include:

- premise
- witness
- argument
- detail
- pause / image-only rest
- invitation
- product landing
- proof
- contrast
- atmosphere

---

## The input layer

The input layer defines what exists for the system to think with.

These files change more often and may vary by brand.

### `product-catalogue.md`
A structured product register.

Each product should ideally include:

- product name
- category
- collection
- price band
- material
- shipping ease
- product status
- hero status
- giftability
- visual strength
- editorial potential
- audience fit
- season fit
- city fit

### `collections-and-drops.md`
A register of grouped releases across time.

Each entry may include:

- collection name
- launch period
- products included
- central thesis
- campaign importance
- whether limited or evergreen
- launch type
- supporting notes

### `month-profiles.md`
An interpretive file for each month.

This should not just list months by name.

It should describe:

- emotional tone
- weather cues
- buying behavior
- social rhythm
- likely occasions
- product priorities
- seasonal tensions
- campaign possibilities

### `occasions-and-celebrations.md`
A register of national, international, seasonal, religious, and brand-relevant moments.

Each entry may include:

- name of occasion
- date or period
- region relevance
- tone
- whether commerce-led, editorial-led, or community-led
- suitable latazin types
- product fit

### `audience-personas.md`
Defines the kinds of people the brand is writing and selling toward.

Each audience may include:

- city
- lifestyle
- aesthetic posture
- likely objections
- trust needs
- product interests
- seasonal needs
- platform behavior

### `previous-performance-log.md`
Captures what happened in prior months.

This is critical for adaptive planning.

Each record may include:

- month
- latazin title
- latazin type
- products attached
- objective
- impressions
- clicks
- saves
- shares
- inquiries
- sales
- strongest page
- weakest point
- lesson

---

## The planning layer

The planning layer uses the house documents and input documents to create editorial direction across time.

### `annual-editorial-strategy-prompt.md`
This file should generate the annual editorial strategy.

It should produce:

- the annual thesis
- primary business priorities
- major seasonal arcs
- quarterly themes
- product emphasis by quarter
- collection/drop timing
- audience priorities
- content balance by latazin type
- strategic experiments to try

### `quarterly-editorial-planning-prompt.md`
This file translates the annual plan into a quarter.

It should produce:

- quarter objective
- dominant categories
- dominant latazin types
- seasonal framing
- campaign priorities
- product focus
- launch windows
- city priorities
- key risks
- proof goals

### `monthly-editorial-calendar-prompt.md`
This file creates the monthly calendar from all relevant context.

It should use:

- previous month data
- annual strategy
- quarterly plan
- products catalogue
- collections register
- month profile
- occasions register
- audience file

It should produce:

- month thesis
- weekly content arcs
- proposed latazins
- latazin type for each
- products attached
- occasion relevance
- campaign support items
- launch support items
- review questions

---

## The generation layer

The generation layer creates the actual content for one latazin.

### `latazin-content-generation-prompt.md`
This file generates individual latazins.

It should take in:

- brand context
- selected latazin type
- objective
- audience
- products attached
- collection/drop context
- month and occasion context
- house voice
- style guide
- quality rubric
- page role system

It should produce:

- concept
- title options
- premise
- page-by-page structure
- draft copy
- visual direction
- product placement logic
- CTA logic
- optional ad or social cutdown ideas
- self-check against the quality rubric

---

## Recommended templates

The `templates/` folder should include reusable working documents.

### `annual-plan-template.md`
A human-readable structure for the annual strategy.

### `quarterly-plan-template.md`
A usable planning sheet for a quarter.

### `monthly-calendar-template.md`
A monthly planning format for content operations.

### `latazin-brief-template.md`
A pre-generation brief for one latazin.

This may include:

- objective
- audience
- product(s)
- type
- trigger
- occasion
- message tension
- desired reader effect

### `launch-strategy-template.md`
A strategy and checklist template for launching a Latazin website or campaign.

---

## Brand instances

The `brands/` directory should contain brand-specific implementations of the system.

The goal is to keep the editorial operating system separate from any one brand.

### Why this matters

The core system should remain reusable.

Brand-specific files should live in their own folders so that:

- Sterling Stitches can have its own product and campaign files
- another brand can be added later without changing the core logic
- the system can become multi-brand over time

Example:

```text
brands/
├── _sample-brand/
└── sterling-stitches/
    ├── products/
    ├── collections/
    ├── calendars/
    ├── latazins/
    └── campaigns/
```

---

## How to use this repository

### Step 1 — Define the house
Complete the files in `docs/house/`.

This establishes the taste, language, typology, and approval system.

### Step 2 — Populate the inputs
Complete the files in `docs/inputs/` or create brand-specific versions inside `brands/<brand-name>/`.

This gives the system material to work with.

### Step 3 — Generate the annual strategy
Use `annual-editorial-strategy-prompt.md` to create the yearly editorial direction.

### Step 4 — Generate the quarterly plan
Use `quarterly-editorial-planning-prompt.md` to narrow the annual strategy into an operating quarter.

### Step 5 — Generate the monthly calendar
Use `monthly-editorial-calendar-prompt.md` to create a month-specific editorial plan.

### Step 6 — Generate individual latazins
Use `latazin-content-generation-prompt.md` to generate specific stories.

### Step 7 — Review with the rubric
Check generated work against:

- house voice
- style guide
- quality rubric
- typology fit
- page role logic

### Step 8 — Log performance
Update `previous-performance-log.md` after publication and campaign activity.

This closes the loop and improves future planning.

---

## Editorial philosophy

This repository is built on a few core beliefs.

### 1. Products should not appear as naked inventory
The buyer should meet them through meaning, context, and sequence.

### 2. Commerce copy can be editorial without becoming vague
Taste-forward does not mean abstract. It means the brand knows how to show, tell, pace, and frame.

### 3. Not every commerce story is a product story
Brands also need stories for:

- collections
- drops
- calendars
- seasons
- collaborations
- milestones
- projects
- community participation
- proof
- public life

### 4. A good latazin is not a slideshow
It is a structured argument with rhythm, imagery, restraint, and intent.

### 5. Planning matters as much as writing
A brand does not need random content volume. It needs a coherent editorial sequence across time.

---

## Design principles behind the system

This operating system should favor:

- clarity over cleverness
- structure over improvisation
- sequence over content dumping
- context over catalogue logic
- restraint over hype
- meaning over generic “storytelling”
- product legibility over product noise

---

## What this repository is not

This is not:

- a generic social media content calendar
- a Canva caption system
- a product listing engine
- a beginner e-commerce playbook
- a moodboard archive with no operating logic
- a generic “brand storytelling” framework

It is a structured editorial operating system for commerce brands using Latazin.

---

## Initial priorities for this repository

The first major milestone is to complete these files:

### House
- `house-metaphors.md`
- `house-voice.md`
- `quality-rubric.md`
- `style-guide.md`
- `commerce-latazin-typology.md`
- `page-role-system.md`

### Inputs
- `product-catalogue.md`
- `collections-and-drops.md`
- `month-profiles.md`
- `occasions-and-celebrations.md`
- `audience-personas.md`
- `previous-performance-log.md`

### Planning
- `annual-editorial-strategy-prompt.md`
- `quarterly-editorial-planning-prompt.md`
- `monthly-editorial-calendar-prompt.md`

### Generation
- `latazin-content-generation-prompt.md`

### Templates
- `latazin-brief-template.md`
- `launch-strategy-template.md`

---

## Suggested roadmap

### Phase 1 — Foundation
Define the house documents and typology.

### Phase 2 — Inputs
Create product, collection, calendar, audience, and performance files.

### Phase 3 — Planning system
Draft annual, quarterly, and monthly planning prompts.

### Phase 4 — Generation system
Draft and refine the individual latazin generation prompt.

### Phase 5 — Brand implementation
Create the first live brand folder, starting with Sterling Stitches.

### Phase 6 — Feedback loop
Use real outputs and performance to refine the house rules, prompts, and templates.

---

## Contribution logic

When updating this repository:

- keep house files stable and intentional
- avoid mixing brand-specific details into system-level documents
- prefer explicit structure over vague notes
- document why a prompt or template changed
- update the changelog when major logic changes occur

---

## Long-term vision

The long-term goal is not just to help brands “make content.”

It is to give commerce brands an editorial operating system that makes them:

- easier to read
- easier to trust
- easier to desire
- easier to remember
- easier to buy from

Latazin should help brands publish product worlds, not just product posts.

---

## Status

Early-stage repository.  
System architecture and core files are being defined.

---

## License

TBD

---

## Maintainer

Created by the team behind Latazin / Poblysh.
