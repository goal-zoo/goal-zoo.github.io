# Goal Zoo — website

Public pages for the Goal Zoo iOS (and later Android) game, served by GitHub Pages
from the `goal-zoo` organisation, so no personal name is in the address. Two pages
for each of the game's 15 languages:

| | Privacy policy | Help & support |
| --- | --- | --- |
| English | https://goal-zoo.github.io/ | https://goal-zoo.github.io/support/ |
| Türkçe | https://goal-zoo.github.io/gizlilik-politikasi/ | https://goal-zoo.github.io/destek/ |
| every other language | `https://goal-zoo.github.io/<lang>/` | `https://goal-zoo.github.io/<lang>/support/` |

`<lang>` is `es`, `pt`, `de`, `fr`, `it`, `id`, `ru`, `ar`, `hi`, `ja`, `ko`, `zh-hans`
or `zh-hant`. Every page links to the same page in every other language.

The privacy policy is the App Store / Google Play privacy URL and the link in the
game's parents area, behind the parental gate; the support pages are the store's
support URL.

**The pages are not edited here.** They are written by the game's repository
(`node scripts/site.mjs` there, from its `site/` folder: one set of texts per
language, one frame, one stylesheet). Change the texts there and run the script;
this repository only receives the finished files:

- `index.html`, `support/`, `gizlilik-politikasi/`, `destek/`, `<lang>/`, `<lang>/support/` — the pages
- `site.css` — one stylesheet for every page
- `logo.png` — the game's logo, shown at the top of every page
- `favicon.png`, `apple-touch-icon.png` — the same logo on the game's sky blue (the app icon)
- `.nojekyll` — serve files as they are

Static HTML and one stylesheet: no scripts, no web fonts, no trackers. This
repository is public: the support address on the pages is the only contact detail; no other personal details and no other apps here.
Publishing: see `DEPLOY.md`.
