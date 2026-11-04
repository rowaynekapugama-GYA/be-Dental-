# Be Dental landing pages

Four static Google Ads landing pages for bedental.com.au. Plain HTML and CSS, no build step.

```
index.html                    New patients (home page)
same-day-crowns/index.html
dental-implants/index.html
invisalign/index.html
assets/be-dental-logo.svg
```

Upload the whole folder to any static host (Vercel, Netlify, SiteGround, a subdomain such as offers.bedental.com.au). The new patient page is the home page at `/`; the others live at their folder paths, e.g. `/dental-implants/`. A row of links in each page's footer switches between the four pages.

## Before going live

- **Forms:** the enquiry forms are design placeholders. Replace each `<form>` with the SmileOX form embed, or point it at the SmileOX endpoint.
- **Tracking:** add the Google Tag Manager container (GTM-W682F8X2) to each page's `<head>` and `<body>`, then set up call click, form submit and online booking conversions.
- **Booking link:** pages use `https://apac.dentalhub.online/soe/new/?pid=AUSTC01` (stray `%20` removed from the site's version). Test it.
- **Placeholders to fill:** `[$NEW PATIENT PRICE]`, `[Offer terms to be confirmed by the practice.]`, `[Implant dentist name, qualifications]`, and the photo placeholder blocks.
- **Offers to approve:** gap-free check-up for Medibank, HCF and Smile.com.au members; free implant consult with CBCT (normally $119).
- **Indexing:** pages carry `noindex` so ad pages don't compete with the main site in Google. Remove it if you want them indexed.
- **Compliance:** keep the AHPRA surgical risk statement on the implant and crown pages. Don't add patient testimonials about clinical care.
