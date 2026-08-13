# REBUILT FMS · GitHub Pages Package

This folder is ready to publish as a single GitHub Pages site.

## Site routes

- `/` — Station Launcher
- `/hub/` — HUB Console
- `/fms/` — FMS Backstage
- `/audience/` — Audience Display
- `/ref/` — Referee Console

The launcher passes the selected Room ID through the URL (`?room=HUB1`) so each tool opens on the same match room.

## Important

GitHub does **not** unzip a ZIP file into a repository for GitHub Pages. Extract the ZIP first, then upload the **contents** of the extracted folder so `index.html`, `.nojekyll`, `hub/`, `fms/`, `audience/`, and `ref/` are at the repository root.

## GitHub Pages settings

Use:

- **Source:** Deploy from a branch
- **Branch:** `main`
- **Folder:** `/(root)`

No build step, framework, npm install, or GitHub Action is required for this package.

## Operational note

All match devices must use the same Room ID. The existing MQTT broker and Arduino/Web Serial flow remain unchanged; this package only reorganizes the UIs into one Pages site and adds the launcher/query-room handoff.
