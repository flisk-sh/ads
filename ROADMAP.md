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

## Later

- [ ] Self-serve payments.
- [ ] More placements (chat, pages, tools).
- [ ] Ad formats beyond a text card (logo strip, launch banner).

## Rules

- Every ad is labelled "Sponsored". Company names always show their logo.
- No personal tracking; stats are counts only.
