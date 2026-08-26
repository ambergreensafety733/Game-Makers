# GAME MAKERS: The $2 Million Race
## Prototype 0.6 — Deterministic Competitive Market Model

This model turns player decisions into sales without dice. It is designed to be visible, fast to resolve, and strategically rich.

## 1. Market Demand Pools

Each territory has visible quarterly demand by genre. Example UK Q4 demand:

- Fantasy 12K
- Family 10K
- Party 8K
- Strategy 8K
- Adventure 7K
- Puzzle 6K
- Children's 9K
- Educational 5K

Demand values are modified by the annual Market Outlook and current known Forecast cards.

## 2. Product Appeal Score

Each active product calculates a visible Appeal score for its current territory/channel.

**Appeal = Base Appeal + Quality + Marketing + Reputation Bonus + Trend Bonus + Price Appeal + Channel Bonus + Awards/Bestseller − Saturation Penalty**

### Base Appeal
From the Concept card, normally 3–5.

### Quality
- Quality 1 = +0
- Quality 2 = +1
- Quality 3 = +2
- Quality 4 = +3
- Quality 5 = +4

### Reputation Bonus
- Reputation 0–2 = +0
- Reputation 3–5 = +1
- Reputation 6–8 = +2
- Reputation 9–10 = +3

### Trend Bonus
- Low = −2
- Normal = 0
- Hot = +2
- Boom = +4

### Price Appeal
- Budget = +2
- Standard = 0
- Premium = −2

### Marketing
Marketing cards/actions give their stated visible modifier, typically +1 to +4.

### Awards/Bestseller
- Bestseller token = +1
- Award token = +1

## 3. Channel Bonuses

Each sales channel has a different strength.

### Amazon
- +2 Appeal from platform reach.
- High capacity.
- Lower contribution than direct channels.

### Website
- No automatic Appeal bonus.
- Demand cap determined by Website Level.
- Direct-community marketing can increase Website Appeal.

### Etsy
- +1 Appeal for Books, Card Games and Compact Games.
- Normally capped at lower demand.

### Retail
- Contract-driven rather than general Appeal competition.

### KDP
- Separate fixed-demand route for eligible books.

## 4. Saturation Penalty

Too many competing products in the same genre reduce everyone's efficiency.

In one territory/channel/genre:
- 1–2 competing products: no penalty
- 3 products: each gets −1 Appeal
- 4+ products: each gets −2 Appeal

This discourages everyone simply chasing the current Boom genre.

## 5. Sales Resolution

For each territory, resolve one genre at a time.

### Step 1 — Establish Market Capacity
Take the visible Genre Demand for the quarter.

Example: UK Fantasy Q4 = 12K.

### Step 2 — Rank Products by Appeal
Highest to lowest.

### Step 3 — Allocate Demand
Each product has a natural Sales Claim based on Appeal:

- Appeal 14+ = up to 6K demand
- Appeal 11–13 = up to 5K
- Appeal 8–10 = up to 4K
- Appeal 5–7 = up to 3K
- Appeal 2–4 = up to 2K
- Appeal 0–1 = up to 1K

Starting with highest Appeal, allocate up to its Sales Claim, limited by stock and channel capacity. Continue until the market demand pool is exhausted.

## 6. Ties

If Appeal ties:
1. Lower consumer price ranks first.
2. If tied, higher Quality.
3. If tied, higher Reputation.
4. If still tied, split remaining demand as evenly as possible.

No die roll.

## 7. Stock Constraint

A physical product cannot sell more than available stock in that territory.

If its Sales Claim is 5K but it has only 3K stock:
- it sells 3K
- takes one SOLD OUT token if unmet demand remained
- unused market demand passes to the next competitor

This makes a competitor's stockout an opportunity for other players.

## 8. Website Capacity

Website Level limits sales regardless of Appeal:
- Level 1 = max 1K/product/quarter
- Level 2 = max 2K
- Level 3 = max 4K
- Level 4 = max 6K

This means the Website can be very profitable but must be deliberately developed.

## 9. Etsy Capacity

Normal cap = 2K/product/quarter.
Eligible niche bonuses can raise this to 3K–4K.

## 10. Amazon Capacity

Amazon has no normal product cap other than market demand and stock.

This keeps Amazon as the volume channel.

## 11. Product Life Cycle

A product's Appeal also changes with age.

### Launch Quarter
+1 Appeal if a Launch action was used this quarter.

### Growth
No modifier.

### Mature
−1 Appeal.

### Decline
−2 Appeal.

An Expansion, New Edition or major campaign can move a Mature/Declining product one stage back temporarily according to later rules.

## 12. Competition Example

UK Fantasy Q4 Market Capacity = 12K.

### Dragon Forge — Kingdoms of Fire
Base 5
Quality 4 = +3
Reputation 4 = +1
Fantasy Hot = +2
Standard Price = 0
Amazon = +2
Marketing = +2
Saturation (3 products) = −1
Total Appeal = **14**
Sales Claim = 6K
Stock = 8K

### Silver Owl — Mystic Realms
Base 4
Quality 5 = +4
Reputation 5 = +1
Fantasy Hot = +2
Premium Price = −2
Amazon = +2
Marketing = +1
Saturation = −1
Total Appeal = **11**
Sales Claim = 5K
Stock = 6K

### MeepleWorks — Tiny Dragons
Base 4
Quality 2 = +1
Reputation 2 = 0
Fantasy Hot = +2
Budget Price = +2
Amazon = +2
Marketing = 0
Saturation = −1
Total Appeal = **10**
Sales Claim = 4K
Stock = 10K

Resolve:
1. Dragon Forge sells 6K. Market remaining = 6K.
2. Silver Owl sells 5K. Market remaining = 1K.
3. MeepleWorks sells 1K despite a 4K claim because the market is almost exhausted.

Result: Silver Owl's premium product earns strong margin, Dragon Forge dominates volume, and MeepleWorks is punished for entering an overcrowded market too late.

## 13. Price Competition Example

Suppose next quarter Fantasy demand falls to 8K.

MeepleWorks can respond by:
- keeping Budget price and aiming to outrank rivals on value
- moving to Standard to improve contribution
- redirecting stock to USA
- increasing marketing
- accepting a retail contract
- licensing the game abroad
- reducing future production

This is the intended decision texture: several viable responses, no random sales roll.

## 14. Market Entry Timing

A player may launch into a genre that is currently Normal or Low to avoid Saturation.

If competitors chase Party Boom and four Party products enter the market, Saturation may make a well-positioned Family or Puzzle product more profitable.

## 15. Multi-Channel Allocation

Before Sales Resolution, players allocate available inventory between open channels/territories.

Example: 8K UK stock of one game could be assigned:
- 5K Amazon
- 2K Website
- 1K Retail reserve

Once allocated for the quarter, stock cannot be moved until quarter end unless an Operations ability permits it.

This makes channel planning meaningful.

## 16. Territory Allocation

Stock must be physically located in UK, EU or USA inventory before ordinary sales.

Players decide where to send incoming production.

A product can be popular in the USA but useless there if all stock was sent to the UK.

## 17. Forecasting Competitors

Prices, products, stock levels and current factory orders are public.

Hidden information should mainly be each player's next chosen action and optional bids.

This allows players to infer competitors' likely moves while retaining uncertainty from human decisions.

## 18. Market Share Bonus

A product that sells the most units in its genre/territory for two consecutive quarters gains a **Market Leader** token.

Working effect:
- +1 Appeal in that territory while it remains Market Leader.

Lose the token if another product outsells it in the next quarter.

This creates momentum but also gives rivals a visible target.

## 19. Avoiding Runaway Leaders

Market Leaders gain only a small +1 advantage.

Growing companies also face:
- higher general overhead at revenue thresholds
- larger inventory commitments
- more staff salaries
- more market-entry costs
- greater exposure to storage

Success creates scale advantages but also increases management pressure.

## 20. Player Count Scaling

### 2 Players
Reduce each genre Market Capacity by approximately 20% to keep competition meaningful.

### 3 Players
Use standard Market Capacity.

### 4 Players
Increase Market Capacity by approximately 15%, but keep Factory/Retail/Licence competition tight.

Exact scaling will be simulation-tested.

## 21. Beginner Mode Simplification

For first-time players:
- Ignore Saturation.
- Ignore Product Life Cycle until Year 2.
- Use only UK in Year 1.
- Use Amazon and Website only initially.

The core Appeal and stock-allocation system remains unchanged.

## 22. Strategic Outcomes This Model Should Produce

Good players should be rewarded for:
- entering less crowded genres
- accurately forecasting demand
- choosing the right price
- matching stock to expected sales
- investing in Quality only where margin justifies it
- timing marketing
- building Website capacity gradually
- expanding into USA/EU at the right time
- exploiting competitor stockouts
- avoiding warehouse-heavy overproduction

## 23. Prototype 0.7 Next

Create a full Year-1 worked scenario for 4 players, including:
- starting concepts
- Q1–Q4 choices
- manufacturing orders
- forecast row
- pricing and marketing
- stock allocation
- sales resolution
- annual accounts

Then use that worked year to identify any rules that feel too complex before building the printable prototype.