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
| Family-operated, veteran-owned; "highest level of integrity and expertise"; 6+ years experience; all phases of residential plumbing | Originally from the HomeAdvisor/Angi profile text — **confirm still accurate** |
| Phone (540) 497-3174 · email dogwoodplumbingva@gmail.com | Public listings tied to the Facebook page |
| 100% recommended on Facebook | Facebook page (facebook.com/Dogwoodplumbingllc) |
| 4.9-star Google rating | Reported by the owner from the Google Business Profile. Google blocks automated access, so this was not independently verified — **re-check before launch.** No review *count* is shown anywhere by design: this is a static site, so a hard-coded count goes stale as soon as the next review arrives. If the star rating itself ever changes, it appears in five places — Reviews page stat, homepage hero chip, homepage stat card, homepage badge row, and About page credentials |
| "Hundreds of customers" · 24/7 availability | 24/7 availability is from the company's existing site (dogwoodplumbva.com), which also claimed "trusted by more than 1,000 customers." The owner revised that figure down to hundreds, and the site now says hundreds. **The old site still says 1,000+ — update it to match.** |
| Hours Mon–Fri 9–5 · credit cards accepted | Originally from the HomeAdvisor profile — **confirm still accurate** |
| "Fast estimates" wording | Owner's preference |
| 10% military / veteran / first responder discount | Originally from the HomeAdvisor/Angi profiles — **confirm still offered** |
| Services: drain cleaning, toilet repair, residential plumbing | The company's existing site pages. (Copper repiping was listed there too, but the owner confirmed it is no longer offered, so it has been removed from the site.) |
| Services: water heaters, leak repair, sump/sewage/septic pumps | Company service descriptions in public listings |
| "Why Dogwood" — state flower angle | The flowering dogwood is Virginia's state flower & tree (marketing angle we added — confirm the owner likes it) |

## Ask Patrick & Lacie

Things to raise with the owners. Nothing here blocks the site from working —
these are accuracy checks and easy wins.

1. **Claim the Google Business Profile — highest-priority item on this project.**
   As of Oct 2026 the listing does not appear to come up in a Google Maps
   search, but the profile demonstrably exists: three Google reviews and a 4.9
   rating were pulled from it in Aug 2026 and are quoted on the Reviews page.
   So it is either unverified, thinly filled in, or has been suspended.

   **Claim the existing listing — do not create a new one.** Reviews do not
   transfer between listings. Creating a duplicate strands the 4.9 rating and
   every existing review on an orphaned profile, and duplicate listings are
   difficult to get merged afterwards.

   Start at **https://business.google.com** and search for the business; Google
   will offer to let the owner claim it rather than create it if it finds the
   existing record. Verification is usually by postcard, phone, or video.

   Worth being blunt with the owners about why this outranks the website: for a
   local plumber, the Google Business Profile drives more phone calls than the
   website does. It is what populates the map pack — the three businesses shown
   above the normal search results. A plumber with a complete, verified profile
   and a website will beat a plumber with a website alone, every time. Nothing
   else on this list comes close in value.

   Once claimed, fill in: service area (the ten towns), hours, services,
   license number, phone, website URL, and photos — the same real job photos
   used on the Services page.
2. **Nudge customers to name their town in Google reviews.** When a job goes
   well, ask the customer to mention where they are — "came out to our place in
   Winchester," "fixed our water heater in Warrenton." This is the single
   cheapest thing the owners can do for search results. Google weighs a
   customer's own words more heavily than anything the business writes about
   itself, so a handful of reviews naming Winchester, Warrenton, or Manassas
   will do more for those searches than any page we could add. It also builds
   the material needed if dedicated town pages are ever revisited.
3. **Confirm four facts carried over from the old HomeAdvisor listing.** All
   four are live on the site right now and none has been verified by the
   owners. If any are wrong it's a quick find-and-replace:
   - "6+ years experience" (homepage, Reviews page)
   - "Mon–Fri, 9:00 AM – 5:00 PM" (all five pages)
   - "10% off for military, veterans & first responders" (all five pages)
   - "24/7 emergency availability" (all five pages)
4. **Two photos still needed.**
   - `images/owner-family.jpg` — a friendly photo of Patrick and Lacie. This is
     the last placeholder on the site and the highest-trust image on a
     family-business page. Alt text and caption are already written.
   - A real truck photo to replace `images/PlumbingTruck.jpg` on the homepage,
     which is AI-generated and carries a visible watermark.
5. **Direct Google review link.** *Blocked on item 1 — the profile has to be
   claimed first.* The "Review us on Google" button currently falls back to a
   Google search. The direct link (from the Google Business
   Profile → Ask for reviews → copy link, of the form
   `https://g.page/r/XXXXXXXX/review`) opens the review box in one tap. Belongs
   in `reviews.html`.
6. **The old Wix site.** Still advertises *free* estimates, *copper repiping*,
   and *1,000+ customers* — all three now inaccurate. Needs correcting or
   taking down so the two sites don't contradict each other.
7. **Quote form delivery.** The form currently opens the visitor's own email
   app, pre-filled and addressed to the company Gmail — functional with zero
   setup, but it loses anyone without a configured mail client. A free
   Formspree account makes it submit silently in-page. **The account should be
   the owners' own**, since it receives their customer lead data
   (instructions in `js/main.js`).

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
