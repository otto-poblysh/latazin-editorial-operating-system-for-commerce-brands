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

## Example Persona

> This is a placeholder to demonstrate format. Replace with personas specific to the brand's actual audience.

### The Quiet Professional

- **City:** Lives in a walkable European city with good public transit, independent coffee shops, and a few reliable restaurants she rotates between. The neighborhood has a bookshop she visits on Saturdays.
- **Lifestyle:** Works in a knowledge-economy role — design, architecture, publishing, or cultural institution. Commutes on foot or by bicycle. Cooks at home more often than she eats out. Hosts small dinners rather than large parties. Travels two or three times a year, usually to cities she already knows. Reads before bed. Keeps a tidy home but does not obsess over interiors.
- **Aesthetic Posture:** Quietly confident. She knows what she likes and does not need trends to validate it. Drawn to materials and construction over logos and novelty. Prefers things that improve with use. Suspicious of anything that tries too hard to look effortless. Respects craft but does not fetishize it — she wants to use things, not display them.
- **Likely Objections:** "I already have a bag I like — why would I replace it?" "The photographs look beautiful, but will the color actually look like that?" "I do not want to buy from a brand that will change its aesthetic next season."
- **Trust Needs:** Consistent editorial voice over time — she notices when a brand's tone shifts to chase a trend. Material specificity in product descriptions — she reads them closely. Clear, honest sizing and color information. Evidence that the brand values longevity over volume.
- **Product Interests:** Bags (mid to premium), leather goods, desk accessories, travel-adjacent items. Drawn to the Studio Line and core leather goods. Responds to products described through use rather than aspiration.
- **Seasonal Needs:** Buys for herself in early autumn (new work bag, cold-weather accessories) and in January (quiet self-investment after the holidays). Buys gifts in November and early December, but starts looking in October. Least active in summer — traveling, not shopping.
- **Platform Behavior:** Follows a small number of brands on Instagram but rarely engages publicly. Saves posts to revisit later. Clicks through to the website to read full product descriptions. Discovers new brands through friends' recommendations or editorial features in publications she trusts. Does not use TikTok. Reads newsletters if they are well-written and infrequent.

## Usage Notes

- **Personas are portraits, not segments.** A segment says "women 30–40, urban, income bracket X." A persona says "she walks to work, reads product descriptions like restaurant menus, and notices when a brand changes its tone." The planning prompts need the latter to calibrate voice and story.
- **Three to five personas is usually sufficient.** More than five creates fragmentation that the editorial calendar cannot serve. Fewer than three risks writing for only one type of reader. Each persona should be genuinely distinct — if two personas would respond to the same latazin in the same way, they are probably one persona.
- **Objections and trust needs are the most actionable fields.** These fields tell the generation prompt what the latazin must address. A Product Argument latazin for a persona who worries about color accuracy needs different proof pages than one for a persona who worries about longevity.
- **Platform behavior shapes distribution, not content.** The latazin itself should be excellent regardless of platform. But knowing that a persona saves posts for later affects how the monthly calendar sequences content, and knowing that a persona reads newsletters affects where the latazin is distributed.
- **Update as audience understanding deepens.** Personas should evolve as the brand learns from performance data, customer conversations, and market shifts. Review personas at the start of each annual planning cycle and adjust when the `previous-performance-log.md` reveals patterns that existing personas do not explain.
- **Name personas consistently across all files.** The persona names defined here are used as references in `product-catalogue.md` (audience fit), in the monthly calendar, and in latazin briefs. If a persona name changes, update all references.
