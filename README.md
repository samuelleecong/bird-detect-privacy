# Bird Detect — Privacy Policy

Static GitHub Pages site hosting the privacy policy for the Bird Detect macOS app.

## Live URL

```
https://samuelleecong.github.io/bird-detect-privacy/
```

This is the URL referenced from inside the app (Settings → About → Privacy Policy) and submitted to App Store Connect as the app's privacy policy URL.

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

1. Edit `index.html` (update the "Last Updated" date and any relevant sections).
2. Commit and push.
3. GitHub Pages redeploys automatically; the in-app link picks up the new content immediately.

App-side changes that may require a privacy policy update:

- Adding any analytics, telemetry, or crash reporting
- Adding network access (e.g., a future cloud-sync feature)
- Adding new permissions (camera, microphone, location, contacts)
- Adding new in-app purchases or subscriptions
- Adding any third-party SDK
