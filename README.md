# BuzzKidz marketing website

Working copy of the BuzzKidz marketing site. The live source of truth is Webflow;
this repo holds a snapshot of it plus the design files for upcoming changes, so
updates can be planned, reviewed and tracked from here.

| | |
|---|---|
| Webflow site | **Buzzkidz** (`buzzkidz-marketing`), site ID `6a6cb6333d9e36d497fa85aa` |
| Staging URL | https://buzzkidz-marketing.webflow.io |
| Planned domains | buzzkidz.org (this site), thebuzzfoundation.org (Foundation "door") |
| Member portal (separate site) | Buzz in a Box, `6a8da16032390f336dc7e054`, repo `launchllama/buzzkidz` |
| Snapshot taken | 2026-11-24 |

## What's in here
- `site/`: full static mirror of the published staging site (all pages, CMS item pages, CSS, JS, images).
  Open `site/buzzkidz-marketing.webflow.io/index.html` in a browser.
- `cms/`: every CMS collection's items as JSON (`cms/_schema/` has the field definitions).
- `pages.json`: Webflow page list with IDs, slugs and SEO settings.
- `design/`: new designs to build. `homepage.html` is the new buzzkidz.org homepage
  (open in a browser), `rendered.html` is its unpacked markup, plus desktop and mobile screenshots.

## Pages
| Page | Path | Page ID |
|---|---|---|
| Home | `/` | `6a6cb6353d9e36d497fa85e8` |
| About | `/about` | `6a8ed0c8d94df1cc943e473f` |
| Buzz Blog | `/buzz-blog` | `6a8ed0c8328055c0ff9c5bf8` |
| Buzz for Grown-Ups | `/buzz-for-grown-ups` | `6a8ed0c8fd9787a0a4326c89` |
| Contact | `/contact` | `6aa2dce6f4e514a32f725ead` |
| Foundation | `/foundation` | `6a8ed0c7c17b711a7fbc600d` |
| Franchises | `/franchises` | `6a8ed0c78b97cd04210b65f6` |
| How We Buzz | `/how-we-buzz` | `6a8ed0c11b998ed5835923c6` |
| Partner With Us | `/partner-with-us` | `6a8ed0c68b97cd04210b65a4` |
| Services | `/services` | `6a8edb05e965519a1c8c00ca` |
| Brand Stages | `/services/brand-stages` | `6aa2dce70a18e2400b8967e0` |
| Creative Content | `/services/creative-content` | `6a8edb05e965519a1c8c00f1` |
| Parties | `/services/parties` | `6a8ed0bdc26dd5c53ac5ad6a` |
| To Schools | `/services/to-schools` | `6a8ed0bdda8eabb79f17341b` |
| Terms & Insurance | `/terms-and-insurance` | `6aa2dce7bd804e298d6a7d00` |
| Thank You | `/thank-you` | `6a8ed0c9fd9787a0a4326d2f` |
| Where We Buzz | `/where-we-buzz` | `6a8ed0c6da8eabb79f173b57` |
| Why Buzz | `/why-buzz` | `6a8ed0bcecd28aa19762d7ce` |

## CMS collections
| Collection | Items | Collection ID | Template path |
|---|---|---|---|
| Party Themes | 14 | `6aa2ddb33568af1488b75886` | `/party-themes/…` |
| Podcast Episodes | 104 | `6aa2dcda25ceac00ddd6d56c` | `/podcast-episodes/…` |
| Blog Posts | 29 | `6a8ed9c29d5438669dc9014d` | `/blog/…` |
| Territories | 10 | `6a8ed9c17932c3cb0225cfe5` | `/territories/…` |
| Logos | 21 | `6a8ed0cfb088d160c155dc9f` | `/logos/…` |
| Testimonials | 85 | `6a8ed0cee8ee8d0f9d8c86f3` | `/testimonials/…` |
| Adventure Themes | 8 | `6a8ed0ce46a3110da4fdfb48` | `/adventure-themes/…` |
| Team | 39 | `6a8ed0cda1df71c59d0234d5` | `/team/…` |
| Franchisees | 11 | `6a8ed0cc7c0b44bdc16dd99d` | `/franchisees/…` |
| Venues | 146 | `6a8ed0cafd9787a0a4326e57` | `/venues/…` |

## Refreshing the snapshot
```
wget -e robots=off --mirror --page-requisites --convert-links --adjust-extension --no-parent -H \
  -D buzzkidz-marketing.webflow.io,cdn.prod.website-files.com https://buzzkidz-marketing.webflow.io/ -P site
```
CMS JSON is pulled with the Webflow MCP connector (`data_cms_tool` > `list_collection_items`).
