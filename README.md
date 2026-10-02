# Bartefy — landing page

The page for **bartefy.ge** and **bartefy.com.ge**: what Bartefy is, a way to
the app at **bartefy.com**, apps coming soon, and how to install the web app
meanwhile. A product of ORZOMI.

- One static page: `index.html` (styles and icons inline).
- **All the words are in `i18n/en.json` (English) and `i18n/ka.json`
  (Georgian; `ka` is Georgian's language code).** Edit the values, never the
  keys. Words in `{braces}` are placeholders for a small button or icon --
  keep them; their labels are entries in the same section. Both files must
  keep the same keys. The English inside `index.html` is only a fallback.
- Georgian and English. It opens in Georgian on a `.ge` domain or a Georgian
  browser, otherwise English; the ქარ / EN switch is remembered.
- Screenshots in `assets/shots/` are the real app with demo content (demo
  people and finds, nothing from real users), made by
  `client/scripts/_demo-shots.mjs` in the app repo.
- Store badges are Apple's and Google's official artwork, shown greyed out
  with "Soon" until the apps are live.

## Run locally

    python3 -m http.server 5288   # then open http://localhost:5288

## Hosting

GitHub Pages from `main`. Pages serves one custom domain per repository: set
it to the main one (e.g. `bartefy.ge`) and point the other domain at it with a
redirect at the registrar.
