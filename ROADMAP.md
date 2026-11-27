# Ads roadmap

ads.flisk.si is where advertisers manage ads that show across Flisk products.
First placements: **ranker** (ranker.flisk.si) and **grow** (grow.flisk.si).

## Now: the manager UI

- [ ] Sign in with the shared Flisk login.
- [ ] Create, edit, pause and delete an ad: title, short text, link, logo.
- [ ] Pick placements: ranker, grow (one or both).
- [ ] Per-ad stats: impressions, clicks, CTR, by placement and by day.
- [ ] Admin review queue: an ad shows only after it is approved.

## Next: serve ads into ranker and grow

- [ ] Small public endpoint that returns the ad for a placement (cached at the edge, no cookies).
- [ ] Ranker: a clearly labelled "Sponsored" slot in the list.
- [ ] Grow: a "Sponsored" tool or service in the plan, matched to the pasted product's audience.
- [ ] Count impressions and clicks without tracking people (no third-party scripts).

## Then: brands from ranker

Ranker lists products; a **brand** is the company or maker behind one or more of them.

- [ ] Create a brand page from ranker entries: logo, link, the products it owns.
- [ ] Brands are mainly for listings around **launches**: a brand launching a product gets a launch listing (ranker + grow) it can boost with an ad.
- [ ] Claim a brand: the maker proves ownership (GitHub org or domain) and then manages its ads here.
- [ ] Launch calendar: upcoming launches by brand, shown on ranker.

## Budgets and payments (with founder)

founder.flisk.si already has monthly spend caps per kind (`llm`, `ads`, `infra`, `mail`); `ads` starts at $0, so ads are off until the owner sets a cap.

- [ ] Each campaign has a daily and a monthly budget; it stops serving the moment either is spent.
- [ ] Founder can buy ads here: a spend is approved against founder's `ads` cap and reserved at once, so two approvals cannot go over the cap together.
- [ ] The founder brain never starts ad spend by itself; the owner approves every ad budget.
- [ ] Payments: top up a prepaid balance (card), invoices, refunds of unspent balance.
- [ ] Spend report per campaign and per placement, matching what founder shows.

## Quality, north star and scale

- [ ] North star: paid clicks that reach a launch page each week (tracked as a number, no personal data).
- [ ] GEL on the repo from day one (`gel init`), every guard set to block; the GEL score shows in the README.
- [ ] Ad serving is a cached edge endpoint, so ranker and grow traffic spikes never hit the database on every view.
- [ ] Rate limits and fraud checks on clicks (repeat clicks and bots are not billed).

## Later

- [ ] More placements (chat, pages, tools).
- [ ] Ad formats beyond a text card (logo strip, launch banner).

## Rules

- Every ad is labelled "Sponsored". Company names always show their logo.
- No personal tracking; stats are counts only.
