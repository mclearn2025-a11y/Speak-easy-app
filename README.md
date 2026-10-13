# Speak-easy-app
SpeakEasy — An advanced, ethical Augmentative and Alternative Communication (AAC) platform featuring a fixed-core, dynamic-fringe architecture and AI-driven contextual prediction. Built to give a voice to nonverbal individuals with uncompromising accessibility.

McLearn Media LLC · Brandon, MS · v1.0.0

## What's in here
- `index.html` — the app
- `manifest.webmanifest` — app name, colors and icons (lets phones and computers install it)
- `sw.js` — offline worker (stores the app so it keeps talking with no internet)
- `icons/` — home-screen icons

No build step. It's a plain website, ready to publish as is.

## Publish it with Cloudflare Pages
1. In Cloudflare, go to **Workers & Pages → Create → Pages → Connect to Git**.
2. Pick this repository (`Speak-easy-app`).
3. Build settings: **Framework preset: None**, **Build command: leave empty**, **Output directory: `/`**.
4. Click **Save and Deploy**. You get a web address like `speak-easy-app.pages.dev`.

After that, every change saved to the `main` branch goes live on its own in about a minute.

## Install it on a device
- **iPhone / iPad:** open the web address in Safari → Share → Add to Home Screen.
- **Android / Chromebook:** open it in Chrome → menu → Install app.
- **Windows / Mac:** open it in Chrome or Edge → install icon in the address bar.

Open it once while online. After that it works offline.

## Updating
When you change the app, also change the `VERSION` line at the top of `sw.js`
(for example `speakeasy-v1.0.1`). Devices pick up the new version the next time they open it online.

## Good to know
- Everyone's words, photos and settings stay on their own device. Nothing is sent to McLearn Media.
- Use Settings → backup file to move a person's words to a new device.
- Real bird photos come from Wikimedia Commons and need internet the first time each one is shown;
  after that they're stored for offline use. Drawings always work.
