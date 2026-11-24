# New buzzkidz.org homepage: build plan

Source: `design/homepage.html` (from Hanneke, 23 Nov 2026). Being built in Webflow on the
draft page **Home (new design)** (`6b0598a69dc43490b887bb58`, `/home-new-design`), a copy
of the current Home page. The live Home page is not touched until the new one is approved.

## Section by section (new design vs current Home)
| # | Section | Change |
|---|---|---|
| 1 | Header | Red bar. Menu button left, logo + "Child Development through the Arts" centre, social icons (LinkedIn, Facebook, YouTube, Instagram, Podcast) + Log in + Buzz us right. Currently yellow with Menu right and no socials. |
| 2 | Hero | Same headline and copy, "Creativity" in red. One button "Why we buzz". New photo composition (two cut-out kids on teal/gold circles) with "Watch me Buzz!" badge. Drop "See how we help schools" and the dot link. |
| 3 | Traits ticker | Keep. Larger words on teal. |
| 4 | Accreditation badges | 5 small cards (Education Alliance Finland, HundrED Top 100, Mastercard Foundation EdTech Fellow, Nation Builder winner, Women in Leadership winner). Currently 3 large cards. |
| 5 | Our Offerings | Title "Our Offerings". Cards get a photo. Children: 4 outline buttons (During the School Day, Extramurals, Independent workshops, Buzz Parties), Original Content image, two round stickers (Our original content, The Buzz Curriculum), two CTAs. Adults: Buzz in a Box logo + "I want to upskill my teachers". |
| 6 | Video | Moves onto a yellow band, "Buzz in action!" + stats cards (300 000+ children, 200+ schools, 800+ teachers online, 100% original SA content). |
| 7 | Schools logo grid | New: "Buzzing in schools and networks like" (from Logos CMS, category School). |
| 8 | We deploy our programmes via | Two photo cards: franchisees (yellow button), Buzz Foundation (grey button, to thebuzzfoundation.org). Replaces the red "We deliver our services via" band. |
| 9 | Where we buzz | Teal band with map. |
| 10 | We partner with | Partner logo grid (Logos CMS, category Partner/Sponsor). |
| 11 | Photo strip | Row of 4+ photos. |
| 12 | The Buzz on us | Testimonials carousel (Testimonials CMS, Featured / Primary Page = Home). |
| 13 | Footer | Not final; leave as is. |

## Editable by the client (no developer needed)
- Copy and single images: Webflow Editor on the page.
- Lists that need add/remove/swap: CMS. Testimonials and Logos already exist. Add small
  collections for accreditation badges, stats, and the photo strip.

## Links (from Hanneke's brief)
Logo `/`, Log in `/buzz-in-a-box`, Buzz us = LeadConnector form
`https://api.leadconnectorhq.com/widget/form/VJbhdZYXvxtgwsQM7J8n`, LinkedIn
`https://www.linkedin.com/company/76597121/`, Why we buzz `/about-us`, During the School Day
`/buzz-in-schools`, Extramurals and Independent workshops `/where-we-buzz`, Buzz Parties
`/buzzparties`, Original content `/creative-content`, Curriculum `/what-happens-in-a-buzz-workshop`,
I want my child to buzz `/where-we-buzz`, I want Buzz at my school `/buzz-in-schools`, Buzz in a Box
logo and upskill teachers `/buzz-in-schools`, video `https://www.youtube.com/watch?v=lpFJlMIaQoQ`,
Franchise `/franchises`, Foundation `https://thebuzzfoundation.org`.

## Slugs to change to the old WordPress ones
| Page now | Now | Old slug |
|---|---|---|
| About (Why we buzz) | /about | /about-us |
| To Schools | /services/to-schools | /buzz-in-schools |
| Parties | /services/parties | /buzzparties |
| Creative Content | /services/creative-content | /creative-content |
| Brand Stages | /services/brand-stages | /buzz-brand-stages |
| How We Buzz (Curriculum) | /how-we-buzz | /what-happens-in-a-buzz-workshop |
| Team | (CMS /team) | /buzz-family (new static page) |
| Where We Buzz | /where-we-buzz | /where-we-buzz (same) |
| Franchises | /franchises | /franchises (same) |

## Progress (24 Nov 2026)
Built on the draft page **Home (new design)** (`/home-new-design`, draft, unpublished). The
live Home page and the shared header are untouched: all restyling uses new `h2-*` classes or
combo classes on top of the existing ones.

Done
- Header: new component **Site Header (new)** (copy of Site Header, the original is on 29 pages).
  Red bar, Menu button on the left (same mega menu and scroll effect), logo + tagline centred,
  social icons, Log in -> /buzz-in-a-box, Buzz us -> LeadConnector form (teal).
- Hero: "Creativity" in red, single "Why we *buzz*" button -> /about-us, eyebrow and secondary links hidden.
  Kids photo animation, rings and "Watch me buzz!" badge kept.
- Our Offerings: white card heads with red/teal top border, new copy, 4 option buttons with arrows,
  "Our original content" and "The Buzz Curriculum" stickers, CTAs "I want my child to *buzz*" and
  "I want Buzz at my school!", adults CTA "I want to upskill my teachers". All links per the brief.
- Video: yellow band, new subline, red "Watch on YouTube", 4 stat cards. Video embed kept.
- Order now: hero, ticker, badges, offerings, video, schools logos, deploy cards, Where we buzz
  (existing interactive map kept), partner logos, photo gallery (marquee kept), testimonials, footer.
- Deploy: white section, "Delivering the Buzz" / "We deploy our programmes via", eyebrows,
  "Learn more" (yellow) -> /franchises, "Read about our work" (grey) -> thebuzzfoundation.org.
- Testimonials: "Testimonials" / "The Buzz on us", white background, red top border on cards
  (still pulled from the Testimonials CMS).
- Hidden (not deleted): audience tiles, Education heading, trust cards, facilitators, Buzz-in-a-Box,
  Why we do what we do, research band, Original Content / Parties split. CTA banner removed from the draft only.

Waiting on image uploads (need the Webflow Designer open with the MCP app)
- 5 accreditation badge cards (replace the 3 current cards)
- Photos in both offering cards, Original Content image, Buzz in a Box logo
- Photos on the two deploy cards
- New school logos (13) and partner logos (4) from the design

Follow-ups
- Logos and gallery photos are static images: swappable in the Editor, but adding/removing needs
  the Designer. Option: move them to CMS lists (Logos collection already exists) so they can be
  added and removed in the Editor.
- Page slugs to old WordPress ones (table above), then point links at pages instead of URLs.
- Footer (waiting on final design), menu contents (waiting on final menu).

## 24 Nov, later: movement restored
Buttons, programme options and stickers had been moved onto new `h2-*` classes, which cut them off
from the site's hover effects on `bkh-btn-primary` and `bkh-bubble`. They are back on their original
classes, with the new look as combo classes on top. Hover colours are Buzz-only (red, blue, yellow,
grey, no black). A page-only embed adds a pulse on button hover, a gentle bob on the two stickers,
and lift-on-hover for stats, badges, deploy cards and testimonials (all off for reduced motion).
Kept throughout: word ticker, photo marquee, interactive map, hero kids animation, header shrink on scroll.
Decision: follow the 23 Nov design file where it differs from the client's earlier Webflow comments.

## 24 Nov, final pass against the design (screenshots in design/review/)
Checked section by section on staging (`/home-new-design`), desktop 1440px and iPhone 13.
- Hero: white background, kids animation runs (it needs Webflow's interactions script; it was never broken).
- Badges: 5 small cards (EAF, HundrED, Mastercard Foundation, Nation Builder, Edupulse), compact strip.
- Offerings: children card ~2x wider (as in design), photos in both cards, Original Content image,
  two stickers, both CTAs in one row, Buzz in a Box logo on the adults card. Stacks on tablet/phone.
- Video band: unchanged YouTube embed (renders blank only in headless screenshots).
- Schools: the design's 19 logos in its order. Partners: own section after the map, plus Val de Vie and
  Northern Cape Education logos.
- Deploy cards: photos flush to the card edges with yellow/grey bars.
- Header on phones: menu, logo, Log in, Buzz us on one row (no sideways scroll; the current live
  homepage scrolls sideways on phones).
Differences kept on purpose: the photo strip keeps the existing moving marquee and photos; testimonials
stay as the 3 CMS cards (design shows a scroll carousel); footer unchanged (not final).

## 24 Nov, evening: map, carousel, slugs
- Where we buzz: replaced the drawn SVG map with a Leaflet tile map (OpenStreetMap tiles; CARTO now
  needs an API key) beside the heading, as in the design. Pins come from the Venues CMS (hidden list on
  the page), nearby areas group at country zoom, popups link to /where-we-buzz?area=..., SA/USA toggle.
- Testimonials: autoplay every 6s (pauses on hover/touch, off for reduced motion), wraps both ways,
  ~2.7 cards visible so the next one peeks, equal-height cards, chevron arrows.
- Slugs now live: /about-us, /buzz-in-schools, /buzzparties, /creative-content, /buzz-brand-stages,
  /what-happens-in-a-buzz-workshop (service pages moved out of /services).
- Links fixed: Our Team / Buzz Family (both headers, both footers) -> /about-us#buzz-family;
  Creative Content buttons -> /what-happens-in-a-buzz-workshop#characters / #curriculum.
- Crawl of 18 pages: only broken internal link left is /buzz-in-a-box (header Log in, per brief) - no such page in Webflow.
- Still needed in Webflow settings (no API): Set "Home (new design)" as Home page; 301 redirects from
  old paths (/about, /how-we-buzz, /services/to-schools, /services/parties, /services/creative-content,
  /services/brand-stages, /buzz-family -> /about-us#buzz-family).

## 24 Nov, night: header and footer site-wide
- All 29 live pages (static pages + every CMS template) now use the new header and footer. Components
  renamed: "Site Header" / "Site Footer" are the new ones; the old ones are "(old, retired)" and only
  remain on the draft backup page.
- Header "Buzz us" hover pulse moved into the header component (was a homepage-only embed).
- Phone fixes (tiny breakpoint): bkh-btn-primary / bkh-btn-secondary may wrap; bkh-character-card min-width 0.
- Verified live: 21 URLs (incl. a blog post and a venue page) show exactly one new header + footer,
  no old ones, no sideways scroll at 390px. Only broken internal link: /buzz-in-a-box (header Log in).
- "/" still serves the old Home page content until "Home (new design)" is set as Home page in the Designer.
