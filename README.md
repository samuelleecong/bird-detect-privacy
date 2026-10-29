# BirdFrame — Privacy Policy

Static GitHub Pages site hosting the privacy policy for the BirdFrame macOS app.

## Live URL

The policy moved to **https://getbirdframe.com/privacy/** on 29 Oct 2026. Its source is `BirdFrame/site/privacy/index.html`, published with the rest of the site.

This repo's `index.html` now only redirects the old address (`https://samuelleecong.github.io/bird-detect-privacy/`) there. Keep the redirect: App Store Connect and builds up to 1.3 still use the old address. Apple only lets the Privacy Policy URL change with a new app version.

App Review sample files are hosted at:

```
https://samuelleecong.github.io/bird-detect-privacy/reviewer-samples/
```

## Deployment

This folder is meant to be the contents of a dedicated public repository named `bird-detect-privacy` on GitHub, with GitHub Pages enabled from the `main` branch root.

Steps:

1. Create a new public repo on GitHub: `bird-detect-privacy`.
2. Copy `index.html` and this `README.md` into the repo root.
3. Commit and push.
4. In repo settings → Pages → set source to `main` / `/ (root)` and save.
5. Wait ~1 minute for the Pages build, then visit the live URL above.

## Local Preview

```bash
cd bird-detect-privacy
python3 -m http.server 8000
# Visit http://localhost:8000
```

## Updating the Policy

Whenever app behavior changes in a way that affects the privacy policy:

1. Edit `BirdFrame/site/privacy/index.html` (update the "Last Updated" date and any relevant sections).
2. Publish the site (`marketing/seo-2026-10-27/publish.sh`).

App-side changes that may require a privacy policy update:

- Adding any analytics, telemetry, or crash reporting
- Adding network access (e.g., a future cloud-sync feature)
- Adding new permissions (camera, microphone, location, contacts)
- Adding new in-app purchases or subscriptions
- Adding any third-party SDK
