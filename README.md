# tellry-site

Public landing + legal pages for **TaleBird** (the iOS app, internal name Tellry).

Mirrors the `solofamily-site` setup: static HTML, deployed on Vercel, lives at the (future) `talebird.app` root.

## Pages

- `/` — landing placeholder
- `/legal/privacy` — Privacy Policy
- `/legal/terms` — Terms of Service

## Deploy

Imported as a Vercel project. Auto-deploys on push to `main`. `vercel.json` enables `cleanUrls` so `/legal/privacy` resolves to `legal/privacy.html` without the extension in the URL.

Once `talebird.app` is registered, point the root at this project. URLs in the iOS app's About → Legal section update to the custom domain.

## Editing

Pages are hand-written HTML — no build step, no framework. Edit, push, Vercel deploys.

Match the visual tone of the app: dark plum background, gold accents, serif headers, generous whitespace.
