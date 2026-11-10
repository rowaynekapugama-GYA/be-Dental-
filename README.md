# Be Dental landing pages

Three static Google Ads landing pages for bedental.com.au. Plain HTML and CSS, no build step.

```
index.html                    New patients (home page)
same-day-crowns/index.html
invisalign/index.html
assets/                       Photos, team headshots, health fund logos, Be Dental logo
```

Upload the whole folder to any static host (Vercel, Netlify, SiteGround, or a subdomain such as offers.bedental.com.au). The new patient page loads at `/`, and the others live at their folder paths, e.g. `/invisalign/`. The footer on each page links to all three.

## What's on each page

- Reception photo banner, with the offer panel overlapping it
- Preferred provider logos (Medibank, HCF, Smile.com.au), plus HICAPS, Medicare and a DVA Veteran Card line, under the banner
- Dental Hub online booking embedded right after the health funds (all "Book online" buttons scroll to it)
- Clinic photos, team headshots, FAQs
- Google map, opening hours with a live "Open now / Closed" badge (Brisbane time), contact details and directions

The new patient page also has the services grid, facilities gallery, payment plans and the full team.

## Before going live

- **Online booking embed:** check the Dental Hub calendar loads inside the page on the live https domain. Some Centaur booking pages redirect to http inside an iframe and get blocked. If that happens, the "Open online booking in a new tab" link under the calendar still works, and we can swap the embed for a button.
- **Tracking:** add the Google Tag Manager container (GTM-W682F8X2) to each page, then set up call click and booking conversions.
- **Offer to confirm:** gap-free check-up for Medibank and HCF members (not Smile.com.au).
- **DVA:** shown as text only. DVA does not let health providers use its logo, and ads must not say services are "free", "fully funded" or "DVA pays".
- **Images:** photos are AVIF, which every current browser supports.
- **Indexing:** pages carry `noindex` so ad pages don't compete with the main site in Google. Remove it if you want them indexed.
- **Compliance:** keep the AHPRA risk statement on the crown page. Don't add patient testimonials about clinical care.
