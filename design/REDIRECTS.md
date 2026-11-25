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
| /bubbas | /buzz-brand-stages |
| /buzzeez | /buzz-brand-stages |
| /buzz | /buzz-brand-stages |
| /buzz-academy | /buzz-brand-stages |
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

# thebuzzfoundation.org
At the domain registrar (once bought): URL forwarding, permanent (301),
thebuzzfoundation.org and www.thebuzzfoundation.org -> https://buzzkidz.org/foundation
(Adding it to Webflow as an extra domain would send visitors to the Buzz Kidz homepage instead.)
