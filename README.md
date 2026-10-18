# 003 deTour

A navigation app that puts the experience ahead of speed. It suggests curated detours along a route that lead to hidden local gems, sending visitors to small businesses outside the busiest centres.

*"The detour becomes the memory."*

> **Draft for review.** Lines tagged *(proposed)* are Claude's suggestions, not yet agreed. Section 10 lists the questions to settle before building.

## Status

**Focus: parked.** Not one of the featured prototypes for now. The featured three are 001, 002 and 004.

Working prototype with a video demo, presented at a hackathon in September 2026 with a pitch deck. This repo is empty so far.

## 1. Problem statement

Navigation apps optimise for the fastest route. Travellers miss the places that make a trip memorable, and small local businesses off the main routes never get found. Meanwhile, cities spend heavily on supporting small businesses and spreading tourism, with few tools that change where people actually go.

## 2. Target audience

- **Users:** leisure travellers, such as road-trippers, tourists and weekend drivers, who have time to spare.
- **Paying customers:**
  - Cities and municipalities (B2G).
  - Local small businesses (B2B).
  - Regional small-business support organisations such as chambers of commerce (B2G2B).

## 3. Value proposition

- **For travellers:** a better journey, not just a faster one.
- **For cities:** a way to send visitor spending to the small businesses they already fund support for, so existing budgets go further.
- **For businesses:** being found by people who are already passing by.

## 4. Core functionality

- Route planning with suggested detours along the way. Each detour shows the extra time and what you'll find.
- Curated gems with a short story and photos.
- Accept or skip a detour while on the trip.
- A memory log of the detours you took *(proposed)*.
- For businesses: boost a listing for €5–20 a month.

## 5. Key user journeys

1. **Traveller:** enters a destination, sees three detours that each add 15 minutes or less, picks one, visits it, and it's saved to their trip.
2. **Business:** claims and boosts its listing.
3. **City:** sees a dashboard of visits to small businesses in the districts it's targeting.

## 6. Non-goals

*(proposed)*
- Not a turn-by-turn navigation engine; route guidance is handed to Google Maps or Apple Maps.
- Not a review platform.
- No commuter routing.

## 7. Feasibility

- Routing comes from map APIs, which cost money at scale.
- The hard part is curated content, not code.
- City deals involve long public procurement cycles.

## 8. Assumptions and risks

- **Chicken and egg:** cities pay only if travellers use it, and travellers stay only if the gems are good.
- **Content supply:** who finds, checks and keeps the gems up to date? That's an ongoing operating cost.
- **Proving value to cities:** showing that a visit happened, and that it increased a business's revenue, is hard.

## 9. Success metrics

*(proposed)*
- Detour acceptance rate.
- Detours completed per trip.
- Repeat use within 30 days.
- For the B2G case: visits to small businesses in target districts.

## 10. Open questions and challenges

1. **Is "Google doesn't care about small businesses" true?**
   - Google earns a lot from local business ads, and Maps already shows places along a route.
   - The defensible edge is more likely curation and alignment with city policy than having the feature at all.
2. **Who comes first?**
   - B2G is the main revenue idea, but cities buy proof.
   - A pilot with one tourism body, such as one route along the Garden Route or the Cape winelands, may come before any city contract.
3. **Who curates the gems?** Locals, the businesses themselves, tourism bodies or AI drawing on reviews? Each option leads to a different product.
4. **How does it relate to 002 Hitchhiker's Guide to the City?** If the two overlap, they could merge into one stronger product.
5. **When do people have time?** Most trips are commutes or on a deadline. How often does someone actually have 20 spare minutes?

## 11. Tech approach

- Expo (React Native), the portfolio standard.
- A map and routing API.
- A curated content database.

## 12. Roadmap

- **v0 (done):** hackathon prototype and pitch deck.
- **v1:** a single pilot route with 20 hand-curated gems.
- **Later:** business accounts, then a city dashboard.
