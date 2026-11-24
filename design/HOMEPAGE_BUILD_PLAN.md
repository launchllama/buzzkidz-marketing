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
