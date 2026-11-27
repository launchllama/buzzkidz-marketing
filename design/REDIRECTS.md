# 301 redirects to add (Webflow: Site settings > Publishing > 301 redirects)

| Old path | Redirect to |
|---|---|
| /about | /about-us |
| /why-buzz | /about-us |
| /how-we-buzz | /what-happens-in-a-buzz-workshop |
| /buzz-curricula | /what-happens-in-a-buzz-workshop |
| /services/to-schools | /buzz-in-schools |
| /services/to-children | /where-we-buzz |
| /services/parties | /buzzparties |
| /services/creative-content | /creative-content |
| /services/brand-stages | /buzz-brand-stages |
| /buzz-in-real-life | /where-we-buzz |
| /bubbas | /buzz-brand-stages#bubbas |
| /buzzeez | /buzz-brand-stages#buzzeez |
| /buzz | /buzz-brand-stages#buzz |
| /buzz-academy | /buzz-brand-stages#buzz-academy |
| /buzz-kidz-music | /creative-content |
| /buzz-kidz-podcast | /creative-content |
| /buzz-edutainment-tv-show | /creative-content |
| /thandi | /creative-content |
| /ben | /creative-content |
| /zadie | /creative-content |
| /the-buzz-foundation-2 | /foundation |
| /buzz-blog/(.+) | /blog/%1 |
| /workshops/venues/(.+) | /venues/%1 |

Old blog posts and venue pages keep working through the last two wildcard rules
(Webflow cannot put the posts under /buzz-blog/ because the Buzz Blog page uses that address).

# Old blog post addresses (top level on the old site)
On the old site each post lived at buzzkidz.org/<post-slug>/ (the Buzz Blog design links them that way).
Add one rule per post:

| Old path | Redirect to |
|---|---|
| /introducing-buzz-franchise-opportunity | /blog/introducing-buzz-franchise-opportunity |
| /struggling-artist-to-franchisor | /blog/struggling-artist-to-franchisor |
| /metamorphosis-into-franchising | /blog/metamorphosis-into-franchising |
| /pack-a-punch-with-a-bit-of-faith | /blog/pack-a-punch-with-a-bit-of-faith |
| /balance-between-screen-world-real-world-crucial-for-kids | /blog/balance-between-screen-world-real-world-crucial-for-kids |
| /5-kids-personality-types-which-one-fits-your-child | /blog/5-kids-personality-types-which-one-fits-your-child |
| /everyone-is-an-expert-what-are-you-an-expert-at | /blog/everyone-is-an-expert-what-are-you-an-expert-at |
| /a-visual-diary-memoirs-of-creating-stories-songs-and-dances-for-children | /blog/a-visual-diary-memoirs-of-creating-stories-songs-and-dances-for-children |
| /creative-thinking-and-why-fostering-it-in-your-child-is-their-ticket-to-success | /blog/creative-thinking-and-why-fostering-it-in-your-child-is-their-ticket-to-success |
| /5-tips-to-help-with-discipline-at-home-or-at-school | /blog/5-tips-to-help-with-discipline-at-home-or-at-school |
| /teacher-training | /blog/teacher-training |
| /ask-for-support-and-give-yours-freely | /blog/ask-for-support-and-give-yours-freely |
| /5-tips-for-building-a-new-small-business | /blog/5-tips-for-building-a-new-small-business |
| /my-story-of-creative-content-creation-for-children | /blog/my-story-of-creative-content-creation-for-children |
| /4-simple-tips-to-give-your-child-a-most-memorable-but-cost-effective-party | /blog/4-simple-tips-to-give-your-child-a-most-memorable-but-cost-effective-party |
| /5-reasons-why-i-live-in-johannesburg-and-how-kidz-can-benefit-from-it | /blog/5-reasons-why-i-live-in-johannesburg-and-how-kidz-can-benefit-from-it |
| /why-i-believe-the-word-shy-has-become-stigmatized | /blog/why-i-believe-the-word-shy-has-become-stigmatized |
| /3-worth-the-2-5-minutes-endearingly-funny-videos-of-kidz | /blog/3-worth-the-2-5-minutes-endearingly-funny-videos-of-kidz |
| /3-things-that-cost-money-but-make-you-and-your-kidz-richer | /blog/3-things-that-cost-money-but-make-you-and-your-kidz-richer |
| /5-reasons-why-superheroes-are-good-for-kidz | /blog/5-reasons-why-superheroes-are-good-for-kidz |
| /5-reasons-why-podcasts-could-help-you-and-your-child | /blog/5-reasons-why-podcasts-could-help-you-and-your-child |
| /what-does-the-world-look-like-when-your-child-is-an-adult | /blog/what-does-the-world-look-like-when-your-child-is-an-adult |
| /music-choices-to-suit-parent-child | /blog/music-choices-to-suit-parent-child |
| /a-throwback-to-traditional-values-at-buzz-birthday-parties | /blog/a-throwback-to-traditional-values-at-buzz-birthday-parties |
| /experienced-teachers-at-buzz | /blog/experienced-teachers-at-buzz |
| /a-buzz-kidz-agency-to-represent-or-not-to-represent | /blog/a-buzz-kidz-agency-to-represent-or-not-to-represent |
| /the-best-for-your-child-an-expert | /blog/the-best-for-your-child-an-expert |
| /every-child-is-special-especially-mine | /blog/every-child-is-special-especially-mine |
| /the-world-is-changing-what-will-your-child-need-to-succeed | /blog/the-world-is-changing-what-will-your-child-need-to-succeed |

# thebuzzfoundation.org
At the domain registrar (once bought): URL forwarding, permanent (301),
thebuzzfoundation.org and www.thebuzzfoundation.org -> https://buzzkidz.org/foundation
(Adding it to Webflow as an extra domain would send visitors to the Buzz Kidz homepage instead.)
