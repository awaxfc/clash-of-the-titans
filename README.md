# Clash of the Titans (1981): The Quest of Perseus

An interactive story game based on the 1981 film. Zeus narrates it, with Thetis, Athena, Hera and Aphrodite speaking their own lines.
Follow Perseus from the Arena of Life to the Kraken. There are choices, timing challenges, Bubo's hints and two endings.

**Play:** https://awaxfc.github.io/clash-of-the-titans/

- Tap or click to play. Keyboard: Space/Enter to continue, 1–4 for choices, H for a hint, M to mute.
- The game is a single `index.html`. It needs no build step and no dependencies.
- All 111 voice lines live in `audio/`. They were made with ElevenLabs `eleven_v4`, and Zeus is voiced by Alistair.

The voice files are stored in this repo as base64 text (`audio/*.mp3.b64`).
The Pages workflow decodes them back to `.mp3` before it deploys.
To run locally, decode them with `for f in audio/*.b64; do base64 -d "$f" > "${f%.b64}"; done`, then open `index.html`.
