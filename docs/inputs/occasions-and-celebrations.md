# Occasions and Celebrations

## Purpose

This file is the register of every occasion, celebration, holiday, cultural moment, and temporal marker that the brand may reference, build around, or deliberately avoid in its editorial calendar. It covers national holidays, religious observances, seasonal transitions, international awareness days, cultural events, and brand-specific milestones.

Occasions are editorial anchors. They give latazins temporal meaning — a reason to exist now rather than next week. But not every occasion deserves editorial attention, and the wrong tone applied to a sensitive moment can damage trust. This register exists so the planning layer can make informed decisions about which occasions to engage, how to engage them, and which to leave alone.

## How This File Is Used in the System

This file is consumed directly by:

- **Monthly Editorial Calendar Prompt** — to identify which occasions fall within the planning window, assess their editorial relevance, and decide whether to build latazins around them, reference them within other content, or acknowledge them without commerce.
- **Quarterly Editorial Planning Prompt** — to map occasion density across three months and ensure the calendar has rhythm rather than a string of reactive posts.
- **Annual Editorial Strategy Prompt** — to identify the year's major occasion clusters and plan editorial peaks and rest periods.
- **Latazin Content Generation Prompt** — to provide occasion context, tonal guidance, and product fit information when generating Occasion or Calendar Marking type latazins.

The planning layer uses occasion entries to calibrate editorial posture. A commerce-led occasion like a gift-giving holiday is treated differently than a community-led cultural awareness moment. The register encodes these distinctions so the planning prompts do not have to guess.

## Field Definitions

Each occasion entry includes the following fields.

### `occasion_name`
The name of the occasion as it is commonly known. Use the most widely recognized name. If the occasion has regional variations in naming, note them in `supporting_notes`.

### `date_or_period`
The specific date or date range. Use exact dates where fixed (e.g., "25 December"), or descriptive ranges where variable (e.g., "Second Sunday in May," "Late January to mid-February," "First Monday in September"). For occasions that span multiple days, give the full range.

### `region_relevance`
Which geographic or cultural regions observe this occasion. Use broad descriptors: "Global," "North America," "Western Europe," "Middle East and North Africa," "East Asia," "UK," "US," "Brazil," etc. List all regions where the brand's audience may observe this occasion.

### `tone`
The emotional register appropriate for editorial content around this occasion. Use one or two descriptive words. Examples: "warm and generous," "reflective," "celebratory," "solemn," "playful," "intimate," "civic," "reverent." This field constrains the house voice calibration for occasion-related latazins.

### `editorial_posture`
How the brand should approach this occasion editorially. Use one of:
- **commerce-led** — the occasion naturally supports product promotion and gift-driven content; audiences expect and welcome commercial engagement
- **editorial-led** — the occasion is best served by a story, argument, or cultural observation; commerce is secondary or embedded subtly
- **community-led** — the occasion belongs to a community or cause; the brand's role is to acknowledge, support, or amplify — not to sell
- **observe only** — the occasion should be noted internally for calendar awareness but does not require public editorial content
- **avoid** — the occasion is sensitive, contested, or off-brand; do not reference it in editorial content

### `suitable_latazin_types`
Which latazin types from `commerce-latazin-typology.md` are appropriate for this occasion. List all that apply. Common pairings:
- Gift-giving occasions → Occasion, Bundle/World, Shop the Look
- Cultural awareness moments → Calendar Marking, Community/Project
- Seasonal transitions → Product Argument, Bundle/World, Manifesto
- Brand milestones → Manifesto, Craft Study, Collection/Drop

### `product_fit`
Which product categories, attributes, or specific products from `product-catalogue.md` naturally align with this occasion. Use category names, product attributes (e.g., "high giftability," "seasonal: winter"), or specific product names. If no products are a natural fit, write "none — editorial only."

### `supporting_notes`
Optional. Any additional context: regional naming variations, sensitivity considerations, historical context, past brand engagement with this occasion, or notes on audience expectations. Free-form text.

## Template Entry Format

```
### [Occasion Name]

- **Date or Period:** [specific date, date range, or recurrence pattern]
- **Region Relevance:** [geographic/cultural regions]
- **Tone:** [emotional register]
- **Editorial Posture:** [commerce-led | editorial-led | community-led | observe only | avoid]
- **Suitable Latazin Types:** [list of applicable types from typology]
- **Product Fit:** [categories, attributes, or product names — or "none — editorial only"]
- **Supporting Notes:** [optional additional context]
```

## Sample Entries

> These are sample entries that demonstrate the schema and editorial posture system. Keep, adapt, delete, or expand them based on the brand's actual markets, audiences, and sensitivities.

### Mother's Day

- **Date or Period:** Second Sunday in May (US, Canada, Australia); Fourth Sunday in Lent (UK); varies by country
- **Region Relevance:** Global (dates vary significantly by region)
- **Tone:** warm and generous, intimate
- **Editorial Posture:** commerce-led
- **Suitable Latazin Types:** Occasion, Bundle/World, Shop the Look
- **Product Fit:** high giftability products, premium price band, strong visual strength; categories: bags, scarves, jewelry, homeware
- **Supporting Notes:** One of the highest gift-purchase periods of the year. Audiences expect and welcome gift guides, but generic "treat her" language should be avoided — see house voice restraint principles. Lead time: editorial content should publish 10–14 days before the date. Consider a latazin structured around the act of selection rather than the act of giving.

### Eid al-Fitr

- **Date or Period:** Variable; follows the lunar calendar and marks the end of Ramadan
- **Region Relevance:** Middle East and North Africa, South Asia, Southeast Asia, diaspora audiences globally
- **Tone:** generous, celebratory, reverent
- **Editorial Posture:** editorial-led
- **Suitable Latazin Types:** Occasion, Calendar Marking, Bundle/World
- **Product Fit:** gifting-friendly products, occasion accessories, hosting and home objects; only where the brand has genuine audience relevance
- **Supporting Notes:** Timing shifts every year. Avoid generic "festival sale" treatment unless the brand serves this audience credibly and consistently. Hospitality, visitation, dress, and acts of generosity may be more editorially appropriate than direct commerce pressure.

### First Real Autumn Weekend

- **Date or Period:** Climate-dependent; usually late September to mid-October
- **Region Relevance:** Temperate-climate markets
- **Tone:** atmospheric, grounded
- **Editorial Posture:** editorial-led
- **Suitable Latazin Types:** Product Argument, Bundle/World, Craft Study
- **Product Fit:** cold-weather accessories, textured materials, daily-carry products, home-and-hosting goods
- **Supporting Notes:** This is a seasonal transition rather than a formal holiday. It often creates stronger product relevance than a named occasion because the audience feels it physically: heavier fabrics, darker mornings, and indoor social life returning.

### Black Friday / Cyber Week

- **Date or Period:** Late November; Black Friday through Cyber Monday, sometimes extended across one week
- **Region Relevance:** North America, UK, Western Europe, increasingly global e-commerce audiences
- **Tone:** clear, disciplined
- **Editorial Posture:** commerce-led
- **Suitable Latazin Types:** Bundle/World, Product Argument, Occasion
- **Product Fit:** easy-to-ship hero products, proven gift categories, bestsellers, high-trust products with strong conversion history
- **Supporting Notes:** This occasion can quickly flatten the brand voice into generic promotion. If the brand participates, editorial value should come from selection, context, and calm decision support rather than urgency clichés. If the brand does not discount, mark the period anyway so planning can position an explicit alternative.

## Category Guidance

The register should include occasions from each of the following categories. Not every occasion needs editorial engagement — but the brand should be aware of all that its audience may observe.

### National and Public Holidays
Fixed-date or annually recurring holidays specific to the brand's primary markets. Examples: New Year's Day, Independence Day, National Day, Bank Holidays. Consider which are commerce-relevant and which are rest days when the audience is not in buying mode.

### Religious and Spiritual Observances
Major religious holidays and observance periods across the faiths represented in the brand's audience. Examples: Christmas, Easter, Eid al-Fitr, Eid al-Adha, Diwali, Lunar New Year, Hanukkah, Ramadan. Approach with care — the `editorial_posture` field is especially important here. Commerce-led content around religious observances requires cultural sensitivity.

### Seasonal Transitions
The turning points of the year that are felt physically and emotionally rather than celebrated formally. Examples: first cold weekend, clocks changing, longest day, first real autumn rain. These are powerful editorial anchors because they are universal within a climate zone and connect directly to product relevance.

### Gift-Giving Occasions
Moments defined by the act of giving. Examples: Mother's Day, Father's Day, Valentine's Day, graduation season, wedding season. These are typically commerce-led and support occasion-type latazins, gift bundles, and product arguments framed around selection.

### Cultural and Awareness Moments
International days, awareness weeks, and cultural movements that intersect with the brand's values or audience interests. Examples: International Women's Day, Earth Day, Pride Month, Mental Health Awareness Week. These require a community-led or editorial-led posture — commerce attachment should be subtle or absent.

### Fashion and Industry Calendar
Events specific to the brand's industry that may create editorial opportunities or audience interest. Examples: Fashion Week, design festivals, trade fairs, award ceremonies. These can support Craft Study, Manifesto, or Collaboration type latazins.

### Brand-Specific Milestones
The brand's own anniversaries, founding dates, collaboration launches, or community events. These are fully within the brand's control and can be scheduled with precision.

### Weekly and Monthly Rhythms
Recurring micro-occasions that structure the week or month. Examples: Monday resets, Friday wind-downs, first of the month, pay-day weekends. These are less formal but can drive social content cadence and lighter editorial moments.

## Usage Notes

- **Not every occasion needs a latazin.** The register is comprehensive by design — it captures everything the brand should be aware of. The planning prompts decide which occasions receive editorial attention based on campaign importance, product fit, and calendar density.
- **Editorial posture is the most important field.** Getting the tone wrong on a sensitive occasion is worse than ignoring it entirely. When in doubt, use `observe only` or `editorial-led` rather than `commerce-led`.
- **Region relevance prevents missteps.** A brand with a global audience must know that Mother's Day falls on different dates in different countries, that national holidays vary, and that religious observances follow different calendars. The register should reflect the brand's actual market geography.
- **Update annually.** Dates shift for lunar-calendar observances, new awareness days emerge, and the brand's relationship to certain occasions may evolve. Review the full register at the start of each annual planning cycle.
- **Cross-reference with month profiles.** The `likely_occasions` field in `month-profiles.md` should reference entries from this register. If an occasion is listed here but not reflected in the relevant month profile, the planning prompt may not surface it at the right time.
- **Product fit connects to the catalogue.** Use product names, categories, and attributes that match `product-catalogue.md`. The planning prompt uses this field to pre-filter the catalogue when building occasion-driven latazins.
