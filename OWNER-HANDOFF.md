# Presenting This Website to the Owner — Notes & Fact Sheet

This document explains where every piece of content came from, what still needs
the owner's input, and what to say when presenting the site.

## Where the content came from

Everything on the site is based on **publicly available information** about
Dogwood Plumbing LLC of Front Royal, VA. Nothing was invented about the
business itself.

> **Note on sources (updated at the owner's request):** HomeAdvisor, Angi, and
> Thumbtack are no longer active for this company, so all references to them —
> the 5.0 ratings, the platform badges, the review links, and the two
> testimonials taken from those sites — have been **removed from the site**.
> Reviews should now come from the Google Business Profile, with Facebook as a
> secondary source. Several remaining facts below were *originally* sourced
> from those now-inactive listings; they are flagged so the owner can confirm
> they are still accurate.

| Fact on the site | Source |
|---|---|
| Family-operated, veteran-owned; "highest level of integrity and expertise"; 8+ years of plumbing experience; all phases of residential plumbing | Profile text originally from HomeAdvisor/Angi. Experience figure **confirmed by the owners, Nov 2026**: 8+ years of plumbing, 2+ years in business. Only the 8+ figure is shown on the site |
| Phone (540) 497-3174 · email dogwoodplumbingva@gmail.com | Public listings tied to the Facebook page |
| 100% recommended on Facebook | Facebook page (facebook.com/Dogwoodplumbingllc) |
| 4.9-star Google rating | Reported by the owner from the Google Business Profile in Aug 2026, and **re-confirmed by the maintainer on the relisted profile in Nov 2026.** No review *count* is shown anywhere by design: this is a static site, so a hard-coded count goes stale as soon as the next review arrives. If the star rating itself ever changes, it appears in five places — Reviews page stat, homepage hero chip, homepage stat card, homepage badge row, and About page credentials |
| "Hundreds of customers" | The company's existing site (dogwoodplumbva.com) claimed "trusted by more than 1,000 customers." The owner revised that figure down to hundreds, and the site now says hundreds. **The old site still says 1,000+ — update it to match.** |
| Emergency service, not 24/7 | **Owners confirmed Nov 2026 that they do NOT offer 24/7 service.** Every 24/7 and "around the clock" claim was removed. Emergencies are taken Mon–Fri and on Saturdays (emergencies only). The old site may still say 24/7 |
| Hours Mon–Fri 9–5, Saturday emergencies only, Sunday closed | **Confirmed by the owners, Nov 2026** |
| 10% military / veteran / first-responder discount | **Confirmed by the owners, Nov 2026** |
| Credit cards accepted | Originally from the HomeAdvisor profile — not yet confirmed |
| "Fast estimates" wording | Owner's preference |
| 10% military / veteran / first responder discount | Originally from the HomeAdvisor/Angi profiles — **confirm still offered** |
| Services: drain cleaning, toilet repair, residential plumbing | The company's existing site pages. (Copper repiping was listed there too, but the owner confirmed it is no longer offered, so it has been removed from the site.) |
| Services: water heaters, leak repair, sump/sewage/septic pumps | Company service descriptions in public listings |
| "Why Dogwood" — state flower angle | The flowering dogwood is Virginia's state flower & tree (marketing angle we added — confirm the owner likes it) |

## Ask Patrick & Lacie

Things to raise with the owners. Nothing here blocks the site from working —
these are accuracy checks and easy wins.

1. **Nudge customers to name their town in Google reviews.** When a job goes
   well, ask the customer to mention where they are — "came out to our place in
   Winchester," "fixed our water heater in Warrenton." This is the single
   cheapest thing the owners can do for search results. Google weighs a
   customer's own words more heavily than anything the business writes about
   itself, so a handful of reviews naming Winchester, Warrenton, or Manassas
   will do more for those searches than any page we could add. It also builds
   the material needed if dedicated town pages are ever revisited.
2. ~~**Confirm four facts carried over from the old HomeAdvisor listing.**~~
   **Answered Nov 2026** — see the fact table above. Two were right (hours,
   discount) and two were wrong (experience is 8+ years of plumbing, not 6+;
   there is no 24/7 service). The site has been corrected.
3. **Two photos still needed.**
   - `images/owner-family.jpg` — a friendly photo of Patrick and Lacie. This is
     the last placeholder on the site and the highest-trust image on a
     family-business page. Alt text and caption are already written.
   - A real truck photo to replace `images/PlumbingTruck.jpg` on the homepage,
     which is AI-generated and carries a visible watermark.
4. **Direct Google review link.** The "Review us on Google" button now points
   at the owners' profile share link (`https://share.google/n16piik2tAwDMfBIW`),
   which opens the business profile. Optional upgrade: the one-tap review link
   from the Google Business Profile → Ask for reviews → copy link, of the form
   `https://g.page/r/XXXXXXXX/review`. Belongs in `reviews.html`.
5. **The old Wix site.** Still advertises *free* estimates, *copper repiping*,
   and *1,000+ customers* — all three now inaccurate, and check it for 24/7 claims too. Needs correcting or
   taking down so the two sites don't contradict each other.
6. **Quote form delivery.** The form currently opens the visitor's own email
   app, pre-filled and addressed to the company Gmail — functional with zero
   setup, but it loses anyone without a configured mail client. A free
   Formspree account makes it submit silently in-page. **The account should be
   the owners' own**, since it receives their customer lead data
   (instructions in `js/main.js`).

7. ~~**Check the star rating on the Google profile.**~~ **Done, Nov 2026** —
   the relisted profile still shows 4.9, so the site's rating claim stands.

   Also worth doing on the profile itself: service area (the ten towns), hours
   (Mon–Fri 9–5, Saturday emergencies only), services, license number, phone,
   website URL once the domain is live, and the real job photos from the
   Services page.

### Settled — no action needed

- **License number.** Virginia License **#2705193552**, confirmed by the owners.
  Appears in the footer of all five pages, the About page credentials list, and
  the homepage structured data.
- **Owner names.** Patrick and Lacie Moore are named on the About page and as
  schema.org `founder` entries in the homepage structured data.
- **Service-area towns.** The owners' confirmed ten: Front Royal, Bentonville,
  Luray, Stephens City, Winchester, Warrenton, Haymarket, Gainesville,
  Nokesville, Manassas — all Virginia. Live across every page, footer, meta
  description, and the JSON-LD `areaServed`.
- **Reviews.** Six real reviews are in place — three Google, three Facebook —
  attributed as "Verified Google Customer" and "Facebook Verified Customer" at
  the maintainer's request, with no real names. The 4.9 Google rating is shown;
  the review *count* is deliberately omitted because it changes and the site
  would go stale.
- **Business address.** The LLC's registered address was deliberately left OFF
  the site — home-based service businesses generally shouldn't publish a home
  address. Service-area wording is used instead.
- **Town pages.** Considered and declined. Near-duplicate per-town pages risk
  being treated as doorway pages by Google. Revisit only with genuinely
  town-specific material (see item 1).

## Design decisions worth mentioning in the pitch

- **Phone-first design.** Most plumbing customers are on a phone with an
  urgent problem. The number is clickable in the header, hero, every section,
  and a sticky bottom bar on mobile.
- **Dogwood blossom branding.** Custom logo drawn for the company — the
  dogwood is Virginia's state flower, which ties the name to local pride.
  It's an SVG, so it stays crisp at any size and can go on business cards too.
- **Trust signals everywhere** — veteran-owned badge, 5.0 ratings, fast
  estimates, the military discount — because reviews and credibility are the
  #1 driver for choosing a local plumber.
- **Real reviews only.** Every quote on the site is from an actual public
  review. No fabricated testimonials.
- **SEO-ready.** Every page has proper titles/descriptions, the homepage has
  Plumber schema markup (helps Google show hours/phone/ratings), plus a
  sitemap and robots.txt. Phase 2: split each service into its own page and
  set up a Google Business Profile for map-pack rankings.
- **No monthly cost.** Pure static site — hosts free on Netlify/GitHub Pages;
  the only cost is the domain they already own.
