# Lenny's Wisdom

A Claude Code plugin that surfaces expert frameworks and wisdom from [Lenny's Podcast](https://www.lennyspodcast.com/) guests. Get decision support and implementation guidance matched to your specific challenges.

## What It Does

Each skill uses diagnostic questions to understand your context, then surfaces 2-3 relevant experts and their frameworks with full attribution and implementation steps.

## Skills

| Skill | Command | Description |
|-------|---------|-------------|
| Growth & Activation | `/lennys-growth` | PLG, activation, experimentation, virality, retention |
| Product Strategy | `/lennys-product-strategy` | Vision, OKRs, prioritization, roadmaps |
| Sales & GTM | `/lennys-sales` | Enterprise sales, positioning, pricing, launches |
| Storytelling | `/lennys-story` | Narratives, presentations, pitching |
| Leadership | `/lennys-leadership` | Org design, team building, decision-making |
| Career | `/lennys-career` | Job search, advancement, negotiation |
| AI & Future | `/lennys-ai` | AI products, coding with AI, future of work |
| Behavioral Design | `/lennys-behavior` | Habits, motivation, psychology |
| Founder Essentials | `/lennys-founder` | Startups, fundraising, resilience, pivots |
| Marketplaces | `/lennys-marketplace` | Two-sided networks, platform dynamics |

## Featured Experts

~95 experts from Lenny's Podcast, including:

- **Product & Growth:** Elena Verna, Casey Winters, Shishir Mehrotra, Gibson Biddle
- **Leadership:** Brian Chesky, Bill Carr, Molly Graham, Camille Fournier
- **Sales & GTM:** Jen Abel, Geoffrey Moore, Arielle Jackson, Andy Raskin
- **Storytelling:** Matthew Dicks, Nancy Duarte, Wes Kao
- **AI:** Mike Krieger, Dan Shipper, Scott Wu, Chip Huyen
- **Career:** Ethan Evans, Deb Liu, Jules Walter
- **Founders:** Eric Ries, Laura Modi, Graham Weaver
- **Behavioral:** Nir Eyal, Kristen Berman

## Installation

In Claude Code, run:

```
/plugin marketplace add saadiq/lennys-wisdom
/plugin install lennys-wisdom
```

## Usage

Invoke any skill by name:

```
/lennys-growth
```

The skill will ask diagnostic questions to understand your situation, then recommend relevant expert frameworks.

### Example Flow

```
User: /lennys-growth

Claude: What growth challenge are you facing?
- Activation/onboarding
- Retention
- Virality/referrals
- Conversion
- Experimentation

User: Activation

Claude: What's your growth model?
- Product-led
- Sales-led
- Hybrid
...

Claude: Based on your situation, here are relevant frameworks:

**Lauryn Isford** (Airtable): "Lower activation rates are better..."
[Implementation steps]

**Elena Verna** (Amplitude): "Product-led sales converts usage into enterprise..."
[Implementation steps]
```

## Attribution

All wisdom is attributed to the original [Lenny's Podcast](https://www.lennyspodcast.com/) guests. This plugin is a tribute to the incredible interviews Lenny Rachitsky has conducted. If you find value here, subscribe to his podcast!

## License

MIT
