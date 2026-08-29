# A table by Monday

**201 dining tables from 100 cm up, across six UK retailers, grouped by one question: can it
be in a London flat on Monday morning?** Monday 31 August 2026 is the UK Summer Bank Holiday.

**Live page: https://smnbss.github.io/london-tables-2026/**

Companion to [london-desk-2026](https://smnbss.github.io/london-desk-2026/).

## The answer

| Tier | Tables | Why |
|---|---|---|
| **In a London IKEA right now** | 37 | Physically on the shelf tonight, branch and count read live from IKEA's stock API |
| **IKEA, not on a London shelf** | 11 | Deliverable 7 days a week, but you'd be betting on a Monday slot |
| **The wider field** | 153 | None of it arrives Monday |

Only IKEA can do it, and only by walking into a store. Stores open **Sunday 11:00–17:00** and
on the bank holiday: **Wembley 10:00–22:00**, Croydon / Greenwich / Oxford Street 10:00–21:00,
Hammersmith 10:00–20:00.

Filters for size (100–119 / 120–139 / 140–179 / 180+ / extends), shape, shop and tone.

## Two corrections to the desk page

The desk page states two things that are wrong as applied to a dining table:

1. **"Wembley opens its collection point at 07:00."** That 07:00–11:00 window is IKEA's
   **parcel lockers**. A locker cannot dispense a dining table. Furniture collection follows
   store hours, so 10:00 on the bank holiday.
2. **"Argos Fast Track excludes bank holidays."** Fast Track *does* run on bank holidays — it
   runs 364 days a year. The real reason Habitat can't make Monday is different: **Fast Track
   does not carry large furniture.** Habitat dining tables ship on Argos standard delivery at
   5–7 working days.

Both of the user's Habitat picks therefore cannot arrive by Monday.

## Sourcing

Store-level stock, prices and opening hours read live from IKEA's UK stock and store APIs on
Saturday 29 August 2026 at 20:30. A stock count is evidence a branch had one that evening, not
a reservation.

Sklum from its own product data across all 94 of its dining tables. Heal's, Danetti, dusk.,
Rose & Grey and Atkin & Thyme from their public Shopify catalogues — **only products whose
listing states a size are shown**, so those shops are under-represented. Habitat carries no
price because habitat.co.uk and argos.co.uk block automated requests outright; only their image
CDN answers.

Crawls were paced at 1.8–3 s per request after Cloudflare rate-limited an earlier unpaced run.
