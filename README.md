# Kartik Reddy | Official VIP Club

A single-page, mobile-first landing page for joining the Kartik Reddy VIP Telegram channel. It shows a profile card and a prominent "Join VIP Channel" button, then redirects to the channel automatically after a 10-second countdown.

## Tech

- Plain HTML, no build step
- Tailwind CSS (Play CDN) and Google Fonts (Cinzel, Plus Jakarta Sans)
- Meta Pixel for `PageView` and `Lead` events
- Hosted on Netlify as a static site

## Run locally

Open `index.html` in a browser, or run `netlify dev` to serve it.

## Editing

- Channel link: `TARGET_URL` in the script, plus the `href` on `#cta-join`
- Countdown length: `TOTAL_SECONDS`
- Pixel ID: the `fbq('init', ...)` call and the `<noscript>` image
