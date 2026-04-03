# Product Catalogue

## Purpose

The product catalogue is the structured register of every product the brand sells or intends to sell. It is not a storefront listing — it is an editorial inventory. Each entry captures not just what a product is, but what it means: how it photographs, who it speaks to, when it belongs, and what kind of story it can carry.

The catalogue exists so that planning prompts can assign products to latazins — the editorial stories, arguments, and worlds that form the brand's public surface (see `commerce-latazin-typology.md` for the full typology) — with precision. Without it, editorial calendars guess at what to feature. With it, every latazin knows exactly what it has to work with — and what it should leave out.

## How This File Is Used in the System

This file is consumed directly by:

- **Monthly Editorial Calendar Prompt** — to determine which products are available for assignment, which are seasonal priorities, and which have untapped editorial potential.
- **Latazin Content Generation Prompt** — to pull material details, price positioning, audience fit, and visual direction into individual latazin briefs.
- **Quarterly Editorial Planning Prompt** — to identify hero products, collection anchors, and gaps in the editorial lineup.

The planning layer treats each product entry as a set of editorial signals. A product marked as having high visual strength and strong giftability will surface differently than one marked as niche, education-dependent, and hard to ship. The catalogue shapes not just what gets featured, but how, when, and for whom.

## Field Definitions

Each product entry includes the following fields. All fields are required unless noted otherwise.

### `product_name`
The full product name as it appears in the brand's own catalogue. Use the brand's naming convention — do not abbreviate or editorialize.

### `category`
The product type. Examples: bag, wallet, scarf, candle, notebook, jacket, jewelry, homeware. Use the brand's own category taxonomy where one exists.

### `collection`
The collection or line this product belongs to, if any. Use `standalone` for products not part of a named collection. A product may belong to more than one collection — list all, separated by commas.

### `price_band`
The relative price positioning within the brand's own range. Use one of:
- **entry** — the brand's most accessible price point
- **mid** — the middle of the range
- **premium** — the upper end of the range
- **signature** — the highest tier, often one-of-a-kind or made-to-order

### `material`
The primary material or materials. Be specific — "Italian vegetable-tanned leather" is useful; "leather" is not. Material specificity drives editorial copy and trust signals.

### `shipping_ease`
How simple the product is to ship. This affects commerce feasibility for certain latazin types and campaign windows. Use one of:
- **easy** — standard packaging, no fragility concerns, ships anywhere
- **moderate** — requires careful packaging or has size constraints
- **difficult** — fragile, oversized, restricted regions, or requires special handling

### `product_status`
The current availability state. Use one of:
- **active** — currently available for purchase
- **pre-order** — announced but not yet shipping
- **limited** — available in restricted quantities
- **archive** — no longer produced but may appear in editorial context
- **seasonal** — available only during specific periods

### `hero_status`
Whether this product is a brand-defining piece that can anchor a latazin on its own. Use one of:
- **hero** — a flagship product; can carry a Product Argument latazin solo
- **supporting** — strong but works best alongside other products
- **ensemble** — contributes to a world or bundle but does not lead

### `giftability`
How naturally the product functions as a gift. This drives occasion-based latazin planning and seasonal calendars. Use one of:
- **high** — obvious gift potential; needs little explanation
- **moderate** — giftable with context or positioning
- **low** — personal purchase; unlikely gift choice

### `visual_strength`
How well the product photographs and presents in editorial layouts. Use one of:
- **strong** — distinctive form, texture, or color; commands attention in layout
- **moderate** — photographs well with good styling and context
- **weak** — functional or understated; needs editorial framing to land visually

### `editorial_potential`
How much story the product can carry. A product with high editorial potential has a process, origin, material story, or cultural reference worth exploring. Use one of:
- **high** — rich backstory, craft process, cultural significance, or design philosophy
- **moderate** — some narrative value; works well when paired with a theme
- **low** — straightforward product; best featured within a bundle or as a supporting mention

### `audience_fit`
Which audience persona or personas this product most naturally serves. Use the persona names defined in `audience-personas.md`. List all that apply, separated by commas. If the product has universal appeal, use `broad`.

### `season_fit`
Which seasons or periods the product is most relevant. Use one or more of:
- **spring**, **summer**, **autumn**, **winter**
- **year-round** — no seasonal dependency
- **transitional** — fits between-season moments (e.g., early autumn, late winter)

### `city_fit`
Which city contexts or lifestyle settings the product belongs to. This is not geographic targeting — it is an editorial signal about the world the product inhabits. Examples: "European urban," "coastal resort," "studio and home," "evening city." Use the brand's own language where possible.

## Template Entry Format

```
### [Product Name]

- **Category:** [category]
- **Collection:** [collection name or `standalone`]
- **Price Band:** [entry | mid | premium | signature]
- **Material:** [specific material description]
- **Shipping Ease:** [easy | moderate | difficult]
- **Product Status:** [active | pre-order | limited | archive | seasonal]
- **Hero Status:** [hero | supporting | ensemble]
- **Giftability:** [high | moderate | low]
- **Visual Strength:** [strong | moderate | weak]
- **Editorial Potential:** [high | moderate | low]
- **Audience Fit:** [persona names, comma-separated, or `broad`]
- **Season Fit:** [spring, summer, autumn, winter, year-round, transitional]
- **City Fit:** [lifestyle/setting description]
```

## Example Entry

> This is a placeholder to demonstrate format. Replace with actual brand products.

### The Everyday Folio

- **Category:** bag
- **Collection:** Studio Line
- **Price Band:** mid
- **Material:** Italian vegetable-tanned leather, brass hardware, cotton twill lining
- **Shipping Ease:** easy
- **Product Status:** active
- **Hero Status:** hero
- **Giftability:** moderate
- **Visual Strength:** strong
- **Editorial Potential:** high
- **Audience Fit:** The Quiet Professional, The Intentional Gifter
- **Season Fit:** year-round
- **City Fit:** European urban, studio and home

## Usage Notes

- **Completeness matters.** Every product the brand sells should have an entry. Planning prompts cannot assign products they do not know about. Gaps in the catalogue create gaps in the calendar.
- **Update before each planning cycle.** New products, status changes, and archive decisions should be reflected before running quarterly or monthly planning prompts.
- **Be honest about visual strength and editorial potential.** Not every product is a hero. The system works best when it knows which products need editorial support and which can carry a latazin alone.
- **Audience fit depends on personas.** This field only works once `audience-personas.md` is populated. Until then, use `broad` or descriptive placeholders.
- **Material specificity is non-negotiable.** The house voice depends on concrete, material language. A catalogue entry that says "premium fabric" gives the generation prompt nothing to work with. Name the fabric, the weight, the origin, the finish.
- **Do not editorialize in this file.** The catalogue is a register, not a pitch. Save persuasion for the latazin itself. Entries should be factual, precise, and structured — the planning prompts will generate the editorial interpretation.
