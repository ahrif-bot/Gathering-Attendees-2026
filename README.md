# The Gathering 2026 — Meet the Attendees

A static attendee directory for The Gathering 2026. Single-page app in `index.html`
with attendee data and photos served from `/_blob/`.

- **`index.html`** — the page (self-contained bundle; loads React + fonts from CDNs).
- **`_blob/dd65b6ceb3db578495bae279548541b6`** — attendee data (JSON).
- **`_blob/<hash>`** — attendee headshots (JPEG, 600×600).
- **`vercel.json`** — sets content types for the extensionless `/_blob/` files.

## Local preview

```bash
python3 -m http.server 4178
```

Then open http://localhost:4178

## Deploy

Static site — deploys on Vercel with zero build step (framework preset: **Other**).
Every push to `main` triggers a new deployment.
