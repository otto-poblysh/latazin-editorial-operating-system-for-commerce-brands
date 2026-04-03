# Previous Performance Log

## Purpose

This file records what happened. Every latazin that was published, every product that was featured, every metric that was measured — captured here so the planning layer can learn from it. The performance log closes the editorial loop: what the system planned, what it produced, and what worked.

Without this file, each planning cycle starts from zero. With it, the monthly calendar prompt knows which latazin types performed well, which products drove inquiries, which pages lost readers, and which editorial angles earned trust. The system gets sharper over time because this file gives it memory.

## How This File Is Used in the System

This file is consumed directly by:

- **Monthly Editorial Calendar Prompt** — to review the previous month's results before planning the next. The prompt looks for patterns: which types performed, which products converted, which audiences engaged, and which approaches fell flat.
- **Quarterly Editorial Planning Prompt** — to assess the quarter's editorial trajectory against its stated objectives and adjust the next quarter's strategy accordingly.
- **Annual Editorial Strategy Prompt** — to evaluate the full year's performance, identify systemic strengths and weaknesses, and inform the next year's strategic direction.

The planning layer reads performance entries as editorial evidence. A latazin that generated high saves but low sales tells a different story than one with low impressions but strong inquiry-to-sale conversion. The log captures enough detail for the planning prompts to distinguish between these patterns and act on them.

## Field Definitions

Each performance entry corresponds to a single published latazin and includes the following fields.

### `month`
The month in which the latazin was published. Use format: "January 2025," "March 2025," etc.

### `latazin_title`
The published title of the latazin. Use the exact title as it appeared to the audience.

### `latazin_type`
The type from `commerce-latazin-typology.md` that this latazin was built as. Use the exact type name: Product Argument, Bundle/World, Craft Study, Occasion, Misreading Correction, Manifesto, Collection/Drop, Calendar Marking, Collaboration, Shop the Look, or Community/Project.

### `products_attached`
The products from `product-catalogue.md` that were featured in this latazin. Use exact product names. List all products, even those that appeared in supporting roles.

### `objective`
The stated editorial and commercial goal for this latazin as defined during planning. Examples: "Drive awareness of the new Studio Line," "Convert gift-seekers during Mother's Day window," "Build trust through craft transparency," "Maintain editorial presence during a quiet month."

### `impressions`
The total number of times the latazin was displayed to readers across all platforms. Use the aggregate number. If platform-specific breakdowns are important, note them in `supporting_notes`.

### `clicks`
The number of click-throughs from the latazin's distribution point (social post, newsletter, homepage feature) to the full latazin content on the brand's site.

### `saves`
The number of times readers saved or bookmarked the content. This metric indicates editorial value — content worth returning to. Platform-specific: Instagram saves, browser bookmarks, newsletter forwards.

### `shares`
The number of times readers shared the content with others. This metric indicates resonance — content worth passing along.

### `inquiries`
The number of direct product inquiries (messages, emails, comments asking about availability, sizing, pricing, or customization) attributable to this latazin.

### `sales`
The number of completed purchases attributable to this latazin. Use the best available attribution — direct link tracking, discount code redemption, or time-correlated sales spikes. If attribution is uncertain, note the methodology in `supporting_notes`.

### `strongest_page`
The page or section of the latazin that performed best — highest engagement, longest dwell time, most interaction, or most click-throughs to product. Identify it by page role (from `page-role-system.md`) or by description if page-level analytics are available.

### `weakest_point`
The page, section, or moment where the latazin lost readers or failed to convert. Identify drop-off points, low-engagement sections, or the specific weakness that prevented the latazin from achieving its objective. Be honest and specific — vague entries ("could have been better") provide no value to the planning prompts.

### `lesson`
One to three sentences capturing the actionable takeaway from this latazin's performance. What should the system do differently, repeat, or stop doing based on this result? This field is the most important input for adaptive planning — it translates raw metrics into editorial intelligence.

### `supporting_notes`
Optional. Any additional context: platform-specific breakdowns, external factors that affected performance (e.g., a competitor's launch, a news cycle, a platform algorithm change), or notes on attribution methodology.

## Template Entry Format

```
### [Latazin Title]

- **Month:** [Month Year]
- **Latazin Type:** [type from typology]
- **Products Attached:** [list of product names from catalogue]
- **Objective:** [stated goal from planning]
- **Impressions:** [number]
- **Clicks:** [number]
- **Saves:** [number]
- **Shares:** [number]
- **Inquiries:** [number]
- **Sales:** [number]
- **Strongest Page:** [page role or description]
- **Weakest Point:** [specific identification of failure point]
- **Lesson:** [1–3 sentences of actionable takeaway]
- **Supporting Notes:** [optional additional context]
```

## Sample Entry

> This is a sample entry showing the schema in use. Replace it with the brand's real post-publication data once the system is live.

### The Case for a Desk You Actually Use

- **Month:** March 2025
- **Latazin Type:** Product Argument
- **Products Attached:** The Desk Sleeve, The Pencil Roll
- **Objective:** Build awareness for the Studio Line desk accessories ahead of the spring reissue; position these as essential tools rather than luxury gifts.
- **Impressions:** 12,400
- **Clicks:** 1,860
- **Saves:** 340
- **Shares:** 95
- **Inquiries:** 22
- **Sales:** 8
- **Strongest Page:** Witness page — a photograph of the Desk Sleeve after six months of daily use, with patina visible on the leather. This page had the highest dwell time and the most saves. Readers responded to proof of longevity.
- **Weakest Point:** The Product Landing page came too early in the sequence — readers encountered the purchase prompt before the Argument page had finished building the case. Drop-off was 34% between pages 4 and 5.
- **Lesson:** For Product Argument latazins featuring unfamiliar products, delay the Product Landing page until after the full argument is delivered. The Witness page should come before the Argument page when the proof is visual and the audience does not yet know the product. Also: desk accessories perform better when framed as daily-use tools rather than workspace aesthetics — the "use" angle drove engagement; the "design" angle did not.
- **Supporting Notes:** Published on a Tuesday; newsletter open rate was 28%, above average. Instagram carousel drove 60% of impressions but only 35% of clicks — most click-throughs came from the newsletter. Consider newsletter-first distribution for Product Argument latazins targeting The Quiet Professional persona.

## Usage Notes for Adaptive Planning

- **Log every published latazin.** Even underperforming content provides data. A latazin that generated zero sales but high saves tells the planning prompt something valuable about audience interest versus purchase readiness.
- **Be honest in the `weakest_point` field.** The planning prompt uses this field to avoid repeating structural mistakes. A vague entry wastes the system's learning capacity. Name the specific page, the specific moment, the specific failure.
- **The `lesson` field drives next-month planning.** When the monthly calendar prompt reads the previous month's log, it looks at lessons first. Each lesson should be concrete enough to act on: "delay the Product Landing page," "use newsletter-first distribution," "avoid pairing these two product categories."
- **Metrics without context are noise.** Raw numbers vary wildly based on audience size, platform algorithm changes, and external factors. The `supporting_notes` field exists to provide the context that makes metrics meaningful. A latazin with 500 impressions and 12 sales tells a very different story than one with 50,000 impressions and 12 sales.
- **Track attribution methodology.** If sales attribution is based on discount codes, say so. If it is based on time-correlation, say so. The planning prompt should know how confident the data is.
- **Review the full log before each planning cycle.** The monthly prompt reads the previous month. The quarterly prompt reads the previous quarter. The annual prompt reads the full year. Ensure entries are complete and up to date before running any planning prompt.
- **Patterns matter more than individual entries.** A single underperforming latazin is a data point. Three consecutive Craft Study latazins with high saves and low sales is a pattern — one that tells the planning prompt something about how the audience relates to that type. The log's value compounds over time.
- **Connect lessons to other input files.** If a lesson reveals something about a persona's behavior, update `audience-personas.md`. If it reveals that a product's editorial potential was misjudged, update `product-catalogue.md`. The performance log is not just a record — it is a trigger for system-wide learning.
