# AGENTS.md

## Architecture
Static single-file site. `index.html` holds all markup, styles (Tailwind Play CDN plus a small `<style>` block) and inline JavaScript. `netlify.toml` publishes the repo root. There is no package.json and no build step. Keep it that way unless the owner asks for a framework.

## Behavior
- A 10-second countdown animates the SVG ring and then sets `window.location.href` to `TARGET_URL`.
- Meta Pixel fires `PageView` on load and `Lead` on a CTA click (`status: clicked`) or on auto-redirect (`status: redirected`).
- The "just joined" pill cycles through a hardcoded list of names every 2.8s.

## Conventions
- The Telegram URL appears twice (the CTA `href` and `TARGET_URL`). Keep both in sync.
- The owner supplied this page. Keep their markup and copy as-is unless they ask for changes.
