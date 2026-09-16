# TravelMexico — September 2026 content

21 self-contained, paste-ready HTML blocks. AI cover images are embedded (base64); client photos link to the live site. Preview at the GitHub Pages URL; source in /raw/.


## Revision 2 (September 14, 2026)

Client round-one feedback applied to all 21 pieces: CTA target is now https://travelmexico.travel/ (was the booking partner); every page has a byline, publish date, last-updated date and an official-sources list (plus a dated WebPage/Article JSON-LD node); AI vocabulary and tropes removed ("genuinely", "actually", "the honest answer is", negative parallelism, significance inflation); answer box and intro paragraphs no longer repeat each other; structure varies by page (at-a-glance table dropped on nine pages, duplicate comparison sections dropped on two, headings and CTA anchor text vary). Source of truth for the edit: `TravelMexico_PSEO/_revise.py`.


## Revision 3 (September 15, 2026)

CTA buttons link to https://www.moretravel4less.com/ again (target=_blank, rel=noopener), each followed by the disclaimer "Searches and bookings are done through MoreTravel4Less. Opens in a new tab." The byline names the partner. Same 21 pieces pushed to the StoreBox CMS (tenant 1093c4f1) as drafts via `TravelMexico_PSEO/publish.py`.


## Revision 4 (September 16, 2026)

The hero-band title is an `h1` in all 21 blocks (was `h2`). Verified against a live StoreBox `custom_page`: the theme renders the title field only in listings, not as a page heading, so the pages had no H1 and the document's only H1 was the theme's footer contact block. Blogs already get an H1 from the theme (their hero is stripped at publish); the change gives the standalone blocks one too. CSS updated so the H1 renders exactly as before. Script: `TravelMexico_PSEO/_h1_fix.py`.
