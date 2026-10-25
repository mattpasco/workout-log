# Workout Log

Single-file static workout tracker (`index.html`). Type one password (10+ characters) on each device; it syncs automatically after every change and each time the page opens. Sync uses the MattTrips Cloudflare Worker (`matttrips-sync`), with its own key (`workoutlog-sync:` + password hashed), so it never mixes with trip data. Data is also cached in `localStorage`, so it works offline.

## Workflow

Edit `index.html`, then `git push` to `main`. GitHub Pages serves `main` at the repo root, so a push is a deploy.
