# London round tables

A one-page catalogue of **47 round dining tables** that can be bought into a London flat,
with photographs, live prices and direct links.

**Live page: https://smnbss.github.io/london-tables-2026/**

Companion to [london-desk-2026](https://smnbss.github.io/london-desk-2026/).

## The organising idea

The desk page was grouped by *when a thing could arrive*, because a bank-holiday deadline
decided everything. Nothing is on a deadline here, so this page is grouped by **diameter** —
in a studio, how much floor the circle eats is the only question that settles anything.

| Band | Tables | What it means |
|---|---|---|
| Ø70–100 cm | 8 | Two to four seats. Base shape matters more than diameter. |
| Ø103–120 cm | 31 | The four-seater standard, where both Habitat picks sit. |
| Ø130 cm and up | 3 | Six seats, ~3.1 m of clear floor once chairs move. |
| Extendable | 5 | Round now, oval later. |

Filter by shop (IKEA, Sklum, Habitat) and by tone (oak, pale, dark, stone, metal).

## Coverage, and where it stops

| Retailer | Tables | Data quality |
|---|---|---|
| Sklum | 25 | Full — live price and stock state from product data |
| IKEA | 15 | Full — live price, size and delivery flags from the catalogue and stock API |
| Habitat | 7 | Partial — names, sizes and photographs, but only one confirmed price |

**Habitat and Argos block automated requests outright** — HTML, their internal APIs, a
headless browser and a server-side fetch all return 403. Only their image CDN is reachable,
which is why the Habitat cards carry photographs but mostly say *check price*. John Lewis,
Dunelm, Wayfair, La Redoute, Made, Heal's and Furniture Village were all tried and are
either blocked or render entirely client-side behind bot detection.

## Findings worth keeping

- **The two pendants are the constraint nobody mentions.** They hang in a line, spaced for a
  long table. A round table wants to be centred under one light.
- **Ø120 is the honest four-seater.** Ø100 seats four only on a single stem or pedestal;
  with four corner legs it is a two-seater.
- **Match the floor or contrast it, never near-miss it.** The laminate is a pale grey-toned
  oak; acacia, walnut and brown-stained oak read warmer and work as deliberate contrast.
- **IKEA VIHALS is £59** for a Ø107 round table — the cheapest of any size here by a wide margin.
- **Sklum ships from Spain** and several pieces are on back-order.

## How it was built

Read live on Saturday 29 August 2026 from the IKEA UK search and stock APIs and Sklum UK
JSON-LD product data. Habitat entries were assembled from search results plus the Argos
media CDN. Images are embedded as data URIs, so the page is a single self-contained file
with no external requests except Google Fonts.
