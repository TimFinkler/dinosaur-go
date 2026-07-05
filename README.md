# 🦖 Dinosaur Go

A Pokémon GO–style **augmented-reality dinosaur hunter** for your phone. Point your
camera at the world, track prehistoric giants on a live radar, capture them in AR,
and fill out a **Dinodex** packed with real paleontology — including where each
species was actually discovered.

It's a single self-contained `index.html` — no build step, no dependencies.

## Play it now

**On your phone (full experience):** open `index.html` over **HTTPS** so the
browser will grant camera, GPS, and compass access. The easiest way is GitHub Pages:

1. In the repo, go to **Settings → Pages**.
2. Set **Source** to **Deploy from a branch**, pick this branch and `/ (root)`, save.
3. Open the published URL on your phone and tap **Begin the hunt**.

A GitHub Actions workflow (`.github/workflows/pages.yml`) is included to auto-deploy
on every push once Pages is enabled.

> Camera and location need HTTPS. Opened from `file://` or without permission, the
> app falls back to a rendered prehistoric scene and a simulated field so it stays
> fully playable anywhere.

## How to play

- **Radar** — a sweeping scope shows nearby specimens by bearing and distance,
  colour-coded by rarity. Tap **Rescan** to sweep again.
- **Hunt / AR** — tap a specimen to enter the camera view. Walk toward it (or tap
  **Approach**) until you're within range, then **Capture**.
- **Dinodex** — every catch unlocks a full field-notes page: period, size, diet,
  fun facts, and a world map pinned to the real discovery site.

## What's real here

All 12 species use genuine paleontology — geologic period and age, body size,
diet, discovery formation, and coordinates (e.g. *T. rex* from the Hell Creek
Formation, Montana; *Velociraptor* from the Gobi Desert, Mongolia; *Spinosaurus*
from the Kem Kem Beds, Morocco).

## Tech

Vanilla HTML/CSS/JS. Uses `getUserMedia` (rear camera), the Geolocation API,
and `DeviceOrientation` (compass) with graceful fallbacks. Progress is saved in
`localStorage`. Type: Fraunces / Archivo / JetBrains Mono.
