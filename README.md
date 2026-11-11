# NTPC Simhadri Plant Guide

Map of NTPC Simhadri plant and township locations with search, road routes,
distances, turn-by-turn directions and live guidance from your current location.

Version 1.5 · Data revision 2026-11-10 · 95 locations

## Files

| File | Purpose |
|---|---|
| `index.html` | The app (map library built in) |
| `data/locations.json` | All locations. The only file to replace when locations change |
| `manifest.webmanifest`, `icons/`, `favicon.ico` | "Add to Home screen" on phones |
| `.nojekyll` | Tells GitHub Pages to publish the files as they are |
| `404.html` | Sends wrong addresses back to the app |

## Publish on GitHub Pages

1. Create a repository on github.com (for example `simhadri-plant-guide`).
2. **Add file → Upload files**, drag in everything from this folder
   (keep the `data` and `icons` folders), then **Commit changes**.
   Note: `.nojekyll` is a hidden file; if your computer hides it, the site still works.
3. **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*,
   Branch = `main`, folder = `/ (root)` → **Save**.
4. After a minute or two the site is live at
   `https://<your-github-username>.github.io/simhadri-plant-guide/`

## Updating locations

1. Open the site → **Admin login** → add / edit / move locations.
2. Press **Download data file** → saves `locations.json`.
3. On GitHub open the `data` folder → **Add file → Upload files** → upload the new
   `locations.json` (it replaces the old one) → **Commit changes**.
4. Everyone sees the new data within a few minutes (refresh the page).

## Notes

- Uses internet services in the browser: Esri satellite imagery, OpenStreetMap
  street map, Google Maps (route view and Navigate button), Google Fonts.
- "Start from my current location" needs the phone's Location switched on and
  permission given in the browser.
- The admin login only stops casual editing. Anyone can read the page source on
  a public site, so it is not strong security.
