# Audience Personas

## Purpose

This file defines the kinds of people the brand is writing toward and selling to. Each persona is not a demographic segment — it is a portrait of taste, lifestyle, and purchasing posture. Personas describe how people live, what they value, how they discover products, what makes them hesitate, and what earns their trust.

The editorial system does not write for "women aged 28–45." It writes for a person who walks to work through a specific kind of neighborhood, who buys deliberately, who reads a product description the way she reads a restaurant menu — looking for signals of care and specificity. Personas make that precision possible.

## How This File Is Used in the System

This file is consumed directly by:

- **Monthly Editorial Calendar Prompt** — to ensure the month's latazin mix addresses different audience segments rather than speaking to the same persona repeatedly.
- **Latazin Content Generation Prompt** — to calibrate voice, product emphasis, objection handling, and CTA logic for the intended reader.
- **Quarterly Editorial Planning Prompt** — to balance audience coverage across the quarter and identify underserved personas.
- **Annual Editorial Strategy Prompt** — to confirm that the brand's editorial program serves its full audience, not just its most visible segment.

The planning layer uses persona entries to make two kinds of decisions: who is this latazin for, and how should it speak to them? A persona with high trust needs and a deliberate buying posture requires different editorial treatment than one who is impulse-driven and visually motivated.

## Field Definitions

Each persona includes the following fields.

### `persona_name`
A short, evocative name that captures the persona's essential character. Not a demographic label — a portrait in two or three words. Examples: "The Quiet Professional," "The Intentional Gifter," "The Weekend Curator." The name should be memorable enough to use as shorthand across all planning documents.

### `city`
The type of place this persona lives or the urban context they inhabit. Not a specific city name unless the brand is geographically focused — instead, describe the character of the place. Examples: "A walkable European city with independent shops and public transit," "A mid-sized coastal town with a seasonal tourist economy," "A dense creative district in a major capital."

### `lifestyle`
How this persona lives day to day. Consider: work rhythm, domestic life, social habits, cultural consumption, travel patterns, relationship to home and public space. Write in present tense, as observation. This is not aspirational marketing — it is an honest description of how this person spends their time.

### `aesthetic_posture`
How this persona relates to beauty, design, and material quality. Not what they like — how they approach the act of looking and choosing. Consider: are they minimalist or layered? Do they follow trends or ignore them? Do they care about provenance? Do they buy for longevity or for the pleasure of the new? Are they confident in their taste or still forming it?

### `likely_objections`
What stops this persona from buying. Not generic objections ("too expensive") — specific, character-driven hesitations. Examples: "Worries that the product will look different in person than in photographs," "Needs to understand the maker's process before trusting a premium price," "Has been disappointed by other brands that looked editorial but delivered poorly."

### `trust_needs`
What the brand must demonstrate to earn this persona's confidence. Consider: material proof, process transparency, editorial voice consistency, social proof, return policy, shipping reliability, cultural alignment. What does trust look like for this specific person?

### `product_interests`
Which product categories, attributes, or collections this persona gravitates toward. Use category names and attributes from `product-catalogue.md`. This field drives product-to-persona matching in the planning layer.

### `seasonal_needs`
How this persona's relationship to the brand changes across the year. Consider: when do they buy most? What occasions drive their purchases? Do they shop seasonally or year-round? Are there months where they are more receptive to discovery and months where they only buy what they already know?

### `platform_behavior`
How this persona discovers, consumes, and shares content. Consider: which platforms do they use? Do they read long-form or scan? Do they save posts for later? Do they share with friends? Do they follow brands or discover through others? Do they click through to websites or stay on-platform? This field affects latazin distribution strategy and format decisions.

## Template Persona Format

```
### [Persona Name]

- **City:** [description of urban/geographic context]
- **Lifestyle:** [daily rhythm, habits, social patterns]
- **Aesthetic Posture:** [relationship to design, quality, and taste]
- **Likely Objections:** [specific hesitations that prevent purchase]
- **Trust Needs:** [what the brand must demonstrate]
- **Product Interests:** [categories, attributes, or collections from catalogue]
- **Seasonal Needs:** [how buying behavior shifts across the year]
- **Platform Behavior:** [content discovery, consumption, and sharing patterns]
```

## Sample Personas

> These personas are sample portraits that demonstrate the format and level of specificity the system expects. Replace, rename, merge, or localize them to fit the brand's real customer base.

### The Quiet Professional

- **City:** Lives in a walkable European city with good public transit, independent coffee shops, and a few reliable restaurants she rotates between. The neighborhood has a bookshop she visits on Saturdays.
- **Lifestyle:** Works in a knowledge-economy role — design, architecture, publishing, or cultural institution. Commutes on foot or by bicycle. Cooks at home more often than she eats out. Hosts small dinners rather than large parties. Travels two or three times a year, usually to cities she already knows. Reads before bed. Keeps a tidy home but does not obsess over interiors.
- **Aesthetic Posture:** Quietly confident. She knows what she likes and does not need trends to validate it. Drawn to materials and construction over logos and novelty. Prefers things that improve with use. Suspicious of anything that tries too hard to look effortless. Respects craft but does not fetishize it — she wants to use things, not display them.
- **Likely Objections:** "I already have a bag I like — why would I replace it?" "The photographs look beautiful, but will the color actually look like that?" "I do not want to buy from a brand that will change its aesthetic next season."
- **Trust Needs:** Consistent editorial voice over time — she notices when a brand's tone shifts to chase a trend. Material specificity in product descriptions — she reads them closely. Clear, honest sizing and color information. Evidence that the brand values longevity over volume.
- **Product Interests:** Bags (mid to premium), leather goods, desk accessories, travel-adjacent items. Drawn to the Studio Line and core leather goods. Responds to products described through use rather than aspiration.
- **Seasonal Needs:** Buys for herself in early autumn (new work bag, cold-weather accessories) and in January (quiet self-investment after the holidays). Buys gifts in November and early December, but starts looking in October. Least active in summer — traveling, not shopping.
- **Platform Behavior:** Follows a small number of brands on Instagram but rarely engages publicly. Saves posts to revisit later. Clicks through to the website to read full product descriptions. Discovers new brands through friends' recommendations or editorial features in publications she trusts. Does not use TikTok. Reads newsletters if they are well-written and infrequent.

### The Intentional Gifter

- **City:** Lives between a major city and a family-oriented suburb or commuter town. Comfortable ordering online but still values the logic of local ritual — birthdays, hosted dinners, annual returns to the same kinds of occasions.
- **Lifestyle:** Buys for others as a form of judgment and care, not obligation. Keeps a running mental list of upcoming occasions. Often shops early, but can become intensely deadline-aware when life crowds the calendar. Wants gifts to feel exact, not lavish for the sake of it.
- **Aesthetic Posture:** Likes objects that feel thoughtful, useful, and well made. Less interested in fashion novelty than in whether something looks chosen. Responds to coherence, packaging restraint, and clear rationale.
- **Likely Objections:** "I do not want to give something that feels generic." "I need to trust that this will arrive on time and look as good in person as it does online." "If this needs too much explanation, it is probably the wrong gift."
- **Trust Needs:** Shipping clarity, reliable delivery windows, clean visual presentation, and precise editorial framing around who a product is for and why. Wants the brand to help with selection, not overwhelm with options.
- **Product Interests:** Small leather goods, home objects, giftable accessories, limited seasonal edits, products with high giftability and easy shipping
- **Seasonal Needs:** Most active around Mother's Day, Father's Day, graduations, November, and early December. Also responsive to thank-you and host-gift moments in spring and summer.
- **Platform Behavior:** Saves gift ideas on Instagram and Pinterest, forwards newsletter links to siblings or partners, and often arrives via search when looking for a specific kind of gift. More likely to convert quickly once trust is established.

### The Weekend Curator

- **City:** Lives in a dense neighborhood in a large city and uses the city heavily — exhibitions, restaurants, markets, short train trips, and friends' apartments form the texture of their week.
- **Lifestyle:** Works hard during the week but treats weekends as editorial space: what to wear, what to carry, what to bring to a dinner, which part of the city to walk through. Buys to refine a way of living rather than to solve a purely practical need.
- **Aesthetic Posture:** Responds to atmosphere, composition, and cultural signals. Open to newness if it feels selected, not trend-chasing. Likes products that belong to a world and can be read socially without being loud.
- **Likely Objections:** "This looks nice, but is there enough substance behind it?" "Is the brand truly considered, or just borrowing editorial language?" "Will I still like this once the novelty of the image wears off?"
- **Trust Needs:** Strong visual direction backed by material proof, consistent voice, cultural references that feel earned, and products shown in context rather than isolation.
- **Product Interests:** Bags, travel-adjacent pieces, hosting objects, occasion accessories, visually strong products, bundle-friendly categories
- **Seasonal Needs:** Most responsive in spring and autumn, when city life feels busiest and most visible. Summer interest centers on travel and social movement; winter interest shifts toward home-and-hosting worlds.
- **Platform Behavior:** Discovers brands through Instagram, newsletters, tastemaker features, and friends' recommendations. Saves visually strong content and is willing to read longer pieces if the opening premise is sharp.

## Usage Notes

- **Personas are portraits, not segments.** A segment says "women 30–40, urban, income bracket X." A persona says "she walks to work, reads product descriptions like restaurant menus, and notices when a brand changes its tone." The planning prompts need the latter to calibrate voice and story.
- **Three to five personas is usually sufficient.** More than five creates fragmentation that the editorial calendar cannot serve. Fewer than three risks writing for only one type of reader. Each persona should be genuinely distinct — if two personas would respond to the same latazin in the same way, they are probably one persona.
- **Objections and trust needs are the most actionable fields.** These fields tell the generation prompt what the latazin must address. A Product Argument latazin for a persona who worries about color accuracy needs different proof pages than one for a persona who worries about longevity.
- **Platform behavior shapes distribution, not content.** The latazin itself should be excellent regardless of platform. But knowing that a persona saves posts for later affects how the monthly calendar sequences content, and knowing that a persona reads newsletters affects where the latazin is distributed.
- **Update as audience understanding deepens.** Personas should evolve as the brand learns from performance data, customer conversations, and market shifts. Review personas at the start of each annual planning cycle and adjust when the `previous-performance-log.md` reveals patterns that existing personas do not explain.
- **Name personas consistently across all files.** The persona names defined here are used as references in `product-catalogue.md` (audience fit), in the monthly calendar, and in latazin briefs. If a persona name changes, update all references.
