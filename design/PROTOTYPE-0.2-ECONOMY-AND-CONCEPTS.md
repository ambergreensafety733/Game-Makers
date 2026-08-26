# GAME MAKERS: The $2 Million Race
## Prototype 0.2 — Economy & First 30 Concepts

This file establishes the first playable economy. All values are deliberately easy to handle and remain subject to playtesting.

## Accounting Scale

- Money is normally handled in **$10,000 units**.
- 1 Stock Cube represents **1,000 physical copies**.
- 1 Demand Point represents demand for approximately **1,000 copies**.
- Books may also use 1,000-sale batches.

## Core Product Formats — Prototype Values

| Format | Development Cost | Base RRP | Size | Typical Base Demand | Development Time |
|---|---:|---:|---|---:|---|
| KDP Game Book | $40K | $22 equiv. | No stock | 2–4 | 1 quarter |
| Physical Game Book | $40K | $22 equiv. | Small | 2–4 | 1 quarter |
| Card Game | $60K | $25 | Small | 3–5 | 1 quarter |
| Compact Game | $80K | $35 | Small | 3–5 | 1 quarter |
| Standard Board Game | $120K | $50 | Medium | 3–6 | 2 quarters |
| Deluxe Board Game | $180K | $70 | Large | 3–6 | 2 quarters |
| Expansion | $50K | $25–35 | Small/Medium | linked to base game | 1 quarter |

## Books

### KDP
- Approximate real-world reference: £16.99 RRP and about £7 publisher return.
- Prototype abstraction: each 1,000 KDP sales gives **$9K publisher income**.
- No stock purchase, freight, warehouse capacity or stockout management.

### Buy & Sell Physical Books
- Real-world reference: approximately £2 purchase cost and approximately £10 gross profit on a direct website/Etsy sale.
- Prototype abstraction: buy 1,000 books for **$3K**; successful direct sale batch produces **$13K contribution before general overhead/marketing**.
- Requires stock, storage and fulfilment capacity.

The exact exchange-rate relationship is not simulated; these are rounded gameplay values preserving the economic choice.

## Physical Manufacturing — Cost per 1,000 Copies

### China
| Format | Cost | Normal Lead Time |
|---|---:|---|
| Card | $5K | 2 quarters |
| Compact | $8K | 2 quarters |
| Standard | $14K | 2 quarters |
| Deluxe | $24K | 2 quarters |

### Europe
| Format | Cost | Normal Lead Time |
|---|---:|---|
| Card | $7K | 1 quarter |
| Compact | $11K | 1 quarter |
| Standard | $19K | 1 quarter |
| Deluxe | $31K | 1 quarter |

### USA
| Format | Cost | Normal Lead Time |
|---|---:|---|
| Card | $8K | 1 quarter / immediate US option |
| Compact | $13K | 1 quarter / immediate US option |
| Standard | $22K | 1 quarter / immediate US option |
| Deluxe | $35K | 1 quarter / immediate US option |

Volume discounts will later be added for 5K and 10K print runs.

## Freight — Prototype 0.2

Freight is paid per Stock Cube and depends on product size and route.

- Small: 1 Freight Unit
- Medium: 2 Freight Units
- Large: 3 Freight Units

Initial China-to-market freight: **$2K per Freight Unit per Stock Cube**.
Europe-to-UK/EU: **$1K per Freight Unit**.
USA domestic: **$1K per Freight Unit**.
Cross-Atlantic movements will normally cost **$2K per Freight Unit**.

Events can substantially change these values.

## Storage

Each company initially has **8 Warehouse Spaces** across its starting operation.

Per 1,000 copies:
- Small = 1 space
- Medium = 2 spaces
- Large = 3 spaces

Stock within capacity is covered by the company's normal warehouse overhead. Excess stock costs **$5K per excess space at Annual Accounts**, with severe excess storage subject to later escalation.

## Pricing

Each physical product normally chooses one of three price positions:

- **Budget:** Demand +2; lowest contribution per sale.
- **Standard:** no demand modifier; normal contribution.
- **Premium:** Demand −2; highest contribution per sale.

Exact channel contribution tables will be developed next so VAT/platform fees are pre-calculated rather than repeatedly calculated by players.

## Demand Formula

**Demand = Base Demand + Trend + Marketing + Reputation Bonus + Seasonal Bonus − Price Penalty − Competition Pressure**

Demand cannot normally fall below 0.

### Trend
- Low: −2
- Normal: 0
- Hot: +2
- Boom: +4

### Reputation Bonus
- Reputation 0–2: 0
- Reputation 3–5: +1
- Reputation 6–8: +2
- Reputation 9–10: +3

### Christmas
Q4 physical games normally receive **+2 Demand**. Some genres/events may modify this.

## Stockouts

If demand exceeds available stock, sell available stock and take one **SOLD OUT** token. Every third Sold Out token costs 1 Reputation, then those three tokens are discarded.

## First 30 Game Concepts

Concept cards determine theme/genre and an opportunity or challenge. Players still choose the final product format unless the concept specifically restricts it.

| # | Concept | Genre | Base Appeal | Special Design Hook |
|---:|---|---|---:|---|
| 1 | Dragon Realm | Fantasy | 4 | +1 Quality if made Standard/Deluxe |
| 2 | Family Frenzy | Family | 4 | +1 Demand as Compact game |
| 3 | Dungeon Journal | Adventure | 3 | +1 Demand as Book; easy translation |
| 4 | Party Panic | Party | 5 | Card/Compact development costs $10K less |
| 5 | Empire Builder | Strategy | 4 | Premium pricing penalty reduced by 1 at Quality 4+ |
| 6 | Pirate's Fortune | Adventure | 4 | Expansion potential +1 |
| 7 | Monster School | Children's | 4 | +1 UK/EU demand |
| 8 | Puzzle Vault | Puzzle | 3 | Book or Compact gets +1 Quality |
| 9 | Space Traders | Strategy | 4 | +1 USA demand |
| 10 | Jungle Jumble | Family | 4 | Small format gains +1 Demand |
| 11 | Wizard Academy | Fantasy | 4 | Translation cost −$10K |
| 12 | Quiz Masters | Educational | 3 | Cheap expansion/update potential |
| 13 | Haunted Hotel | Adventure | 4 | Marketing campaigns gain +1 effect in Q4 |
| 14 | Tiny Kingdoms | Strategy | 4 | Compact format uses 1 less storage space (min 1) |
| 15 | Dino Dash | Children's | 5 | Budget price gains an additional +1 Demand |
| 16 | Secret Agents | Family | 4 | Strong website/Etsy potential: +1 Direct demand |
| 17 | Galactic War | Strategy | 5 | Deluxe version costs +$20K development but starts Quality +1 |
| 18 | Spellbound Stories | Fantasy | 3 | KDP Book gets +2 Demand when Fantasy is Hot/Boom |
| 19 | Football Boss | Strategy | 4 | +1 demand in UK and Europe |
| 20 | Crazy Kitchen | Party | 4 | Influencer marketing gets +1 effect |
| 21 | Treasure Island | Adventure | 4 | May release a Book spin-off for $20K less development |
| 22 | Animal Rescue | Family | 4 | +1 Reputation if first-year sales reach 5K |
| 23 | Brain Battle | Puzzle | 4 | Educational and Puzzle trends: use the better trend |
| 24 | Robot Factory | Educational | 3 | Manufacturing-themed promotions cost $10K less |
| 25 | Kingdom at War | Fantasy | 5 | Excellent Deluxe potential; Large version +1 Base Appeal |
| 26 | Detective Files | Puzzle | 4 | Book and Card formats both gain +1 Base Appeal |
| 27 | Holiday Havoc | Party | 3 | Q4 bonus is +4 rather than +2 |
| 28 | Ocean Explorers | Educational | 4 | +1 EU demand; award campaigns cost less later |
| 29 | Zombie Escape | Adventure | 5 | Launch marketing +1, but Mature stage arrives sooner |
| 30 | My First Adventure | Children's | 4 | Book/Compact versions translate for 50% normal localisation cost |

## Concept Design Rule

A high Base Appeal concept is not automatically the best investment. Format, price, manufacturing location, competition, market trend, marketing, stock availability and overhead all affect final profitability.

## Product Quality

Prototype Quality scale: **1–5 stars**.

Base product normally starts at Quality 2. Development upgrades may add Quality:
- Professional Artwork: $20K → +1 Quality (max 5)
- Extensive Playtesting: $20K → +1 Quality for review/licensing purposes
- Premium Components: physical games only; $20K–$40K depending on size → +1 Quality, but manufacturing cost increases
- Pre-Launch Campaign: $20K → +1 Launch Marketing rather than Quality

Final balancing will prevent players simply buying Quality 5 every time.

## Next Economy Work

Prototype 0.3 should establish:
1. UK Amazon net contribution tables including simplified VAT/platform effect.
2. USA Amazon contribution tables without UK VAT.
3. Website and Etsy contribution tables.
4. Retail/wholesale economics.
5. Marketing action costs/effects.
6. Staff/service salaries and benefits.
7. Loan/interest system.
8. Factory volume discounts and capacity.
9. Licence advances/royalties.
10. Annual Accounts player aid.

These numbers will then be simulation-tested before final artwork is locked.