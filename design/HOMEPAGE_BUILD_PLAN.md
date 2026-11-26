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

## 25 Nov: homepage live + full-site QA
- "Home (new design)" is now the Home page (client set it). Old home drafted (/old-home 404). Home SEO title/description added.
- Testimonials: whole cards only (3 desktop / 2 tablet / 1 phone), slides one card at a time; nothing cut off.
- Menu "Philanthropy" -> https://thebuzzfoundation.org (new tab). Footer logo was linked to the old home page -> now Home.
- Full-site visual review (2 reviewers, 20 pages x desktop/phone). Fixed:
  - Squashed team/character cards on phones (Franchises, Workshop) - my earlier min-width change; cards now full width on phones.
  - Parties: baked-in balloon images (wrong Ninja Turtles text, cut-off words, missing Princess Sofia) replaced by drawn balloons (page head code).
  - Workshop: missing Dinosaurs cover shows a branded teal tile (page head code) until artwork is supplied.
  - Buzz in Schools statistic was unstyled (divs inside a <p>): now large white headline.
  - Site default font was Arial (Webflow default) -> brand font via site head code.
  - 53 "Read more" buttons linked to "#" (About team 39, Franchises 11, Why Buzz 3): now link to item pages via data-cms-slug + site footer script.
  - Blog: 21 posts updated - links to old slugs (/how-we-buzz, /about, /services/...) fixed, orphan <li> wrapped in <ul>, excerpts without captions, typos.
  - Testimonial typos (Gail Fry, Lizette Uys). Podcast artwork fragment hidden. Button spacing/alignment, rich-text link colour.
- Verified: crawl of 18 pages + item pages, only broken link /buzz-in-a-box (header Log in, waiting on client).
- Open for client: Dinosaurs cover art, Princess Sofia (now covered), Terms & Insurance page is placeholder text,
  "Ravi" vs "Zadie" in podcast episodes, footer grey (#838484) white-text contrast ~3.6:1, school count 200+ vs 317.

## 25 Nov: site structure to the website plan (design/website-plan.html)
- New page Buzz Fam /buzz-family (team list moved from About; About's team section hidden).
- Header menu rebuilt to the plan's 8 groups, headings not clickable: Why we buzz (Why we do what we do, Buzz Blog);
  Drama, Dance & Singing (How we buzz, Who we buzz with); Our Original Content; Our services (To Children, To Schools);
  Our Philanthropy (The Buzz Foundation -> /foundation until the domain forwards); Our Franchising (Franchisees,
  Become a Franchisee); Our Parties; Our Team (Meet the Buzz Fam, Work for Buzz -> current job form).
- Footer: About Buzz Kidz (Meet the Buzz Fam, Work for Buzz), Legal (2 PDFs), Buzz us (phones, email, Buzz us form), socials.
  Explore column hidden. Merch Store link waiting on its address.
- Renamed: About -> Why we buzz; How we buzz -> The Buzz Curriculum; Brand Stages -> Who we buzz with;
  Franchises -> Our Franchises (hero button "Become a Franchisee"); Partner -> Become a Franchisee. SEO titles updated.
- Redirects and foundation domain: see design/REDIRECTS.md.

## 2026-11-25: plan re-check and Why we buzz rebuild
- Website plan updated (design/website-plan.html). Changes: Why we buzz has a 7-section layout; Buzz Fam opens with Hanneke's full bio.
- Why we buzz (/about-us) rebuilt natively from design/why-we-buzz-design.html (classes `wwb-*`): banner, What motivates us, quote strip, two programme streams, research cards + six study links (new tab), compliance pie (HTML embed), Buzz Blog taster (CMS list, newest 3, Read More via data-cms-slug fallback). Old About sections hidden, not deleted. Banner photo: home2-strip-1 (design file had no hero photo).
- Buzz Fam: founder section (`fam-founder`) with Hanneke's full bio above the team.
- Buzz in Schools: added "Learn about Buzz" links (Curriculum, Why we buzz, Content, Who we buzz with, Parties).
- Where we buzz: "Why we do what we do" now -> /about-us (was dead /why-buzz).
- Homepage: hero kids bob + sticker wobble re-created in site CSS (old IX3 timeline targeted elements on the drafted old homepage); tighter section gaps.
- Homepage ticker: "Critical Thinking" added after Collaboration in every ticker set.
- Menu: verb "buzz" italic in Why we buzz / How we buzz / Who we buzz with (site footer script wraps it in <em>; brand names untouched).
- Full re-check 2026-11-25: all 13 plan pages 200 with new header/footer, no mobile overflow, one H1 each, no broken images; only broken link is header "Log in" -> /buzz-in-a-box (awaiting destination).

## 2026-11-26: Buzz Blog page
- Plan "v2" upload is identical to the previous plan (only the file name differs).
- Blog Posts collection: new Option field `category` (Franchising / Our story / Parenting / Teaching); all 29 posts assigned.
- /buzz-blog rebuilt to design/buzz-blog-design.html (classes `blg-*`): banner, search (filters all posts), CMS card grid (photo, coloured category dot, date "29 April 2022", title, excerpt, Read more; whole card links to /blog/<slug>), Load more blogs (6 at a time). Old hero/list sections hidden.
- Footer: Buzz us column left-aligned, Buzz us as teal button (matches designs).
- REDIRECTS.md: one rule per old top-level post address -> /blog/<slug>.
- Review pass vs designs: added the design's gold burst (by the banner label) and gold swoosh to the Blog and Why we buzz banners (assets shape-burst-gold.png / shape-swoosh-gold.png); "The Buzz Blog" heading upright as in the design; design hover states added (blog cards lift, Load more fades, Why we buzz buttons/links).
- Why we buzz full review vs design/why-we-buzz-design.html: text word-for-word match; 9 study links now open in a new tab (builder had dropped target); base type matched (line-height 1.55, body 13px, tighter headings, 68ch paragraph cap, balanced headings); section widths now measured like the design (content-box); research photos at natural height; research bottom padding 16px; quote 22px with teal quote marks; therapy box titles teal/red; button sizes. Sections now within ~1% of the design pixel-for-pixel (blog differs only because the design has photo placeholders).
