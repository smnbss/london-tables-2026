# London tables — 120 cm and up

A one-page catalogue of **129 dining tables**, none smaller than 120 cm along its longest
side, with photographs, live prices and direct links.

**Live page: https://smnbss.github.io/london-tables-2026/**

Companion to [london-desk-2026](https://smnbss.github.io/london-desk-2026/).

## What is on it

Sections split **round** from **oval** from **rectangular & square**, because that is the
decision underneath all the others. Filters for **size**, **shop** and **tone** compose.

| | Tables |
|---|---|
| Round | 34 |
| Oval | 10 |
| Rectangular & square | 85 |
| **Total** | **129** |

Size bands: 120–139 · 140–179 · 180+ · Extends. An extending table is filed under its
**open** size and marked *extends*.

| Retailer | Tables | Data quality |
|---|---|---|
| Sklum | 83 | Full — live price, stock state and dimensions from all 94 of its dining tables |
| IKEA | 38 | Full — live price, size and finish count from the search and stock APIs |
| Habitat | 8 | Partial — names, sizes and photographs, no prices |

## The findings

- **A 120 cm floor removes most of IKEA's round range.** Across a 315-product pool, IKEA
  sells exactly **five** round tables at 120 cm or over: NÄSINGE, SKOGSTA, MÖRBYLÅNGA and the
  two extendables. Round and big is where IKEA stops and Sklum starts.
- **Two pendants in a line is an argument for a rectangle.** A round table wants one light
  centred over it. The room has two, spaced for a long table.
- **At 120 cm a rectangle beats a circle on floor.** Ø120 and 120×80 seat the same four
  people, but the rectangle sits against a wall and leaves a walkway; the circle has to live
  in the middle of the room.
- **Only the pendants are black.** A table with a black frame or leg — SKOGSTA, TARSELE,
  MARIEDAMM, black-legged SKÅLSTA — is the one thing that answers them.
- **SKÅLSTA is £99 for 140×80** in 18 top-and-leg combinations; oak-effect top on black legs
  echoes both the floor and the pendants.

## Notes on sourcing

Read live on Saturday 29 August 2026. Sklum's own product data was used for dimensions where
the product title omitted them; Cloudflare rate-limited the crawl at 25 pages, so the
remaining 69 were re-fetched with pacing — an earlier version of this page was missing 10
Sklum round tables because of it.

Habitat and Argos block automated requests outright: HTML, their internal API, a headless
browser and a server-side fetch all return 403. Only their image CDN answers, which is why
Habitat cards carry photographs but no price. John Lewis, Dunelm, Wayfair, La Redoute, Made,
Heal's and Furniture Village were tried and are blocked or render fully client-side.
