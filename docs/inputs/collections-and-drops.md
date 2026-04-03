# Collections and Drops

## Purpose

This file is the register of every grouped product release the brand plans, has launched, or intends to launch. A collection is not a latazin — it is a brand-defined grouping of products that share a thesis, a launch moment, or a design logic. The editorial system then decides how to tell that story.

Collections and drops shape the editorial calendar from the supply side. They determine what is available, when, and with what level of strategic importance. Without this register, the planning layer cannot distinguish between a major seasonal launch and a quiet restock — and the editorial weight assigned to each will be wrong.

## How This File Is Used in the System

This file is consumed directly by:

- **Annual Editorial Strategy Prompt** — to map the year's major launch moments and identify editorial peaks and valleys.
- **Quarterly Editorial Planning Prompt** — to align editorial arcs with collection timelines and determine which collections anchor each quarter.
- **Monthly Editorial Calendar Prompt** — to schedule collection-specific latazins, assign supporting content around launch windows, and coordinate pre-launch, launch, and post-launch coverage.
- **Latazin Content Generation Prompt** — to provide collection context, thesis, and product groupings when generating Collection/Drop type latazins.

The planning layer treats each collection entry as an editorial event with a timeline, a narrative core, and a set of constraints. A limited drop with high campaign importance will receive different editorial treatment than an evergreen restocking of a core line.

## Field Definitions

Each collection or drop entry includes the following fields.

### `collection_name`
The official name of the collection or drop as the brand defines it. Use the brand's own naming — do not rename for editorial convenience.

### `launch_period`
The target launch window. Use a specific month or date range. Examples: "March 2025," "Late September 2025," "15–22 November 2025." If the collection has a rolling release, note the start date and expected cadence.

### `products_included`
A list of product names from `product-catalogue.md` that belong to this collection. Use exact product names as they appear in the catalogue. If the full product list is not finalized, note which entries are confirmed and which are tentative.

### `central_thesis`
One to three sentences describing the idea behind this collection. Not a marketing tagline — a clear statement of what connects these products and why they belong together. This thesis will feed directly into latazin premise development.

### `campaign_importance`
How much editorial weight this collection should receive relative to the brand's other releases. Use one of:
- **anchor** — a defining release for the season or year; receives maximum editorial support
- **major** — a significant release that warrants dedicated latazins and calendar presence
- **standard** — a regular release; featured but does not dominate the calendar
- **minor** — a quiet addition; mentioned within other latazins rather than leading its own

### `limited_or_evergreen`
Whether the collection is time-bound or permanently available. Use one of:
- **limited** — finite production run or restricted availability window
- **seasonal** — returns periodically but is not available year-round
- **evergreen** — permanently available; part of the brand's core offering

### `launch_type`
The format of the release. Use one of:
- **full collection** — multiple products released together under a unified identity
- **capsule** — a small, focused release (typically 2–5 products)
- **single drop** — one product or a very tight grouping released as an event
- **restock** — return of previously sold-out products
- **expansion** — new additions to an existing collection

### `supporting_notes`
Any additional context that affects editorial planning. This may include: collaboration partners, production constraints, shipping timelines, regional availability, press embargo dates, or connections to occasions and celebrations. Free-form text — keep it factual and concise.

## Template Entry Format

```
### [Collection Name]

- **Launch Period:** [month, date range, or rolling schedule]
- **Products Included:** [list of product names from product-catalogue.md]
- **Central Thesis:** [1–3 sentences: what connects these products and why they belong together]
- **Campaign Importance:** [anchor | major | standard | minor]
- **Limited or Evergreen:** [limited | seasonal | evergreen]
- **Launch Type:** [full collection | capsule | single drop | restock | expansion]
- **Supporting Notes:** [additional context affecting editorial planning]
```

## Sample Entry

> This is a sample entry showing the schema in use. Replace it with the brand's actual collections and drops or duplicate it as a starting pattern.

### Studio Line — Spring Reissue

- **Launch Period:** March 2025
- **Products Included:** The Everyday Folio, The Desk Sleeve, The Pencil Roll, The Studio Tote
- **Central Thesis:** The Studio Line returns with the same construction and the same materials, because the best tools do not need reinvention. This reissue adds two new sizes to the Desk Sleeve and introduces a lighter weight canvas option across all pieces.
- **Campaign Importance:** major
- **Limited or Evergreen:** seasonal
- **Launch Type:** expansion
- **Supporting Notes:** Canvas option uses deadstock fabric from Italian mill — limited to approximately 200 units across all products. Photography scheduled for late February. Consider pairing with a Craft Study latazin on the mill relationship.

## Usage Notes

- **Collections are not latazins.** A collection is a brand-defined grouping. A latazin is an editorial object. The planning layer decides how many latazins a collection needs — sometimes one, sometimes several, sometimes none if the collection is better served as a supporting mention inside another story.
- **Thesis drives editorial direction.** The `central_thesis` field is the single most important input for the generation prompt when building Collection/Drop type latazins. Write it clearly and honestly — what the collection actually is, not what the brand hopes it sounds like.
- **Campaign importance must be calibrated honestly.** If every collection is marked `anchor`, the calendar has no rhythm. Most brands have one or two anchor releases per year. The rest should be distributed across `major`, `standard`, and `minor`.
- **Update before each planning cycle.** Add new collections, adjust launch periods, and update product lists as they are finalized. The planning prompts can only work with what is recorded here.
- **Cross-reference with product catalogue.** Product names in `products_included` must match entries in `product-catalogue.md`. If a product appears here but not in the catalogue, the system cannot pull its editorial attributes.
- **Use `supporting_notes` for anything that changes how the story is told.** A collaboration with a specific artisan, a production limitation, a connection to a cultural moment — these details shape the editorial approach even if they do not fit neatly into the structured fields.
