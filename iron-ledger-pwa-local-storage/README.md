# Iron Ledger — PWA

This is the ready-to-host PWA version of Iron Ledger.

## Files

- `index.html` — the original Iron Ledger app
- `manifest.json` — PWA manifest
- `sw.js` — service worker for install/offline app-shell caching

## Hosting

Host this folder from an HTTPS website. GitHub Pages works well.

The site root should contain:

    index.html
    manifest.json
    sw.js

## Brave Android

1. Open the HTTPS site in Brave.
2. Open the Brave menu (⋮).
3. Choose **Add to Home screen** or **Install app**, depending on the Brave version.
4. Confirm the name and add it.

Do not open `index.html` as a local `file://` page if you want PWA installation/service-worker support.

Note: the app's existing workout functionality and styling are preserved.


## Data storage

Workout progress and profile data are stored locally in the browser using
standard `localStorage`. GitHub Pages only serves the app files; it does not
receive the workout data. Clearing the browser/site data can remove the saved
data, and data is not automatically synced between devices.
