# New's Handyman Service, LLC

Marketing site for New's Handyman Service, LLC — Michael New's craftsman shop
in Apopka, Florida. 4.9 stars across 34 Google reviews.

- **Address** 105 W Magnolia St, Apopka, FL 32703
- **Phone / text** (321) 356-0802
- **Hours** Open 24 hours
- **Plus code** MFHP+PC Apopka, Florida

## Pages

| File | Contents |
| --- | --- |
| `index.html` | Hero, key numbers, four headline trades, owner's statement, review highlights, contact |
| `services.html` | The nine-line schedule of work, photo set |
| `reviews.html` | Reviews verbatim with owner replies, topic counts, Google highlights |
| `about.html` | The owner's statement in full, how the work runs, FAQ |
| `contact.html` | Address, phone, hours, plus code, what to send, service area |

## Design

Identity: **the measured drawing** — a finish carpenter's own documents.
Walnut `#1A1512`, bone `#EFEAE1`, brass `#B08637`, with linen `#F1EDE6` panels
for contrast sections. Fraunces (variable, `opsz`/`SOFT`/`WONK` axes set per
role) for display over Karla for text. Dark-first, since the work is the bright
thing; a viewer on an explicit light setting gets a linen-grounded page.

Original drawn graphics, no clip art:

- **Hero figure** — a hand-authored SVG measured drawing of a through-dovetail
  tail board: 45° section hatching via `<pattern>`, extension and dimension
  lines with ticks, the overall dimension called out, and the 1:8 dovetail
  slope annotated the way a shop drawing would.
- **Brand mark** — two interlocking joint combs.
- **Section bands** — 45° drawing hatch rendered in CSS
  (`repeating-linear-gradient`), matching the hatch in the hero figure.
- **Icons** — hand-drawn SVG line art, `currentColor` stroked.

Photography passes through one grade — warmed, slightly desaturated, then a
brass-to-walnut diagonal wash (`.plate`, `.band-photo`) — so separately-shot
images read as one portfolio.

Static HTML, no build step, no JavaScript, no dependencies. Google Fonts is the
only external request.

## Reviews

Quoted verbatim from the Google Business profile. Where Google truncates a long
review, the cut is marked rather than hidden. Michael's replies are included in
full.

3 of 34 reviews are transcribed (Madison Donnell, Karen Barrios, Christine
Tyser), plus the three quotes Google surfaces in its summary and the four topic
counts it names. Google does not publish per-star counts, so no star
distribution is shown — inventing one would have been fiction.

To add more, copy an `<article class="review">` block in `reviews.html`.

## Service list provenance

Every one of the nine lines is evidenced, not guessed:

| Line | Evidence |
| --- | --- |
| Custom carpentry | Owner's statement; Madison's custom twin-sink vanity |
| Trim & finish | Owner's statement ("intricate trim work") |
| Water leak repair | Google topic count |
| Water heater repair | Google topic count |
| Bathroom & kitchen fixtures | Madison's sinks; Karen's bathroom details |
| Windows & doors | Google highlight quote (window repair) |
| Grab bars & accessibility | Christine's review |
| Punch lists & finish-out | Karen's review (contractor left details unfinished) |
| Mower & small engine repair | Google topic count |

## Before launch

- Photography is placeholder stock from Pexels in `assets/img/`. Michael has
  photos on his Google listing already — swap those in by replacing the files
  and keeping the filenames; grade and crop are handled by CSS. Suggested
  sizes: 1600px wide for `hero.jpg`, `bench.jpg` and `blueprint.jpg`, 1000px
  for the rest.
- No licensing or insurance claims appear anywhere by design. Add them only
  once verified.
- Confirm the service-area wording on `contact.html`.
- Rating and review counts are current as of September 2026.
