# tellry-site

Public landing + legal pages for **TaleBird** (the iOS app, internal name Tellry).

Static HTML, served via **GitHub Pages** directly from `main`. No build, no framework, no separate hosting account — the repo IS the deployment.

## Pages

- `/` — landing placeholder
- `/legal/privacy/` — Privacy Policy
- `/legal/terms/` — Terms of Service

Each page lives at `<path>/index.html` so the URL renders clean without any `.html` extension or rewrite config.

## Deploy

Pages is enabled on this repo with source `main` / `/` (root). Pushing to `main` triggers a deploy automatically; takes ~30s to land. Current host: `https://zbencz3.github.io/tellry-site/`.

When `talebird.app` is registered, drop the apex `CNAME` to `zbencz3.github.io` and add a `CNAME` file at the repo root containing `talebird.app`. URLs in the iOS app's Legal section then read `.app` instead of `.github.io`.

## Editing

Pages are hand-written HTML. Edit, push, wait ~30s, refresh. Match the visual tone of the app: dark plum background, gold accents, serif headers, generous whitespace.
