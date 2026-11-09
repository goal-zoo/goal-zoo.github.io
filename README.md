# Goal Zoo — website

Public pages for the Goal Zoo iOS (and later Android) game, served by GitHub Pages
from the `goal-zoo` organisation, so no personal name is in the address:

- https://goal-zoo.github.io/ — Privacy Policy (EN)
- https://goal-zoo.github.io/gizlilik-politikasi/ — Gizlilik Politikası (TR)
- https://goal-zoo.github.io/support/ — Help & Support (EN)
- https://goal-zoo.github.io/destek/ — Yardım ve Destek (TR)

The privacy policy is the App Store / Google Play privacy URL and the link in the
game's parents area, behind the parental gate (`goal-zoo/src/platform/links.ts`);
the support pages are the store's support URL.

- `site.css` — one stylesheet for every page
- `favicon.png`, `apple-touch-icon.png` — from the game's icon
  (`node scripts/brand.mjs --site=../goal-zoo.github.io` in the game repo)
- `.nojekyll` — serve files as they are

Static HTML and one stylesheet: no build step, no scripts, no web fonts, no
trackers. Keep both languages in step, and bump the effective date when the
policy changes. Publishing: see `DEPLOY.md`.
