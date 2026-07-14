# Happy Birthday, Sia

A standalone, cinematic interactive birthday site for Sia's 17th birthday on July 20, 2026. Open `index.html` in a modern browser; there is no build step.

## Personalize it

- Replace the two commented audio file paths in `index.html` with licensed MP3s at `assets/music/soft-piano.mp3` and `assets/music/celebration.mp3`.
- Your three personal gallery images are now stored in `assets/images/`. To change them later, update both `src` and `data-full` for the relevant gallery entry in `index.html`.
- The date is set in `js/countdown.js`; update it if the celebration date changes.
- The full experience is locked until July 20, 2026 in the visitor's local time. Update the matching `new Date(2026,6,20)` value in `js/main.js` if the celebration date changes.
- Once the birthday date arrives, the site asks for the gift password before revealing the experience. The current password is configured in `js/main.js`.
- The birthday message is in `js/typing.js`.

## Features

The site includes a canvas night sky and fireworks, adaptive countdown, SVG cake with 17 extinguishable candles, optional microphone-based blow detection with a touch-friendly fallback, confetti, lightbox gallery, smooth scrolling, lazy images, keyboard-compatible buttons, and reduced-motion support.

## Notes

Microphone access needs HTTPS or `localhost` in most browsers. If it is unavailable or denied, clicking the candle button again automatically starts the celebration. Empty asset folders are intentional placeholders for private images, music, sounds, fonts, and icons.

## Put it on a phone with GitHub Pages

The site must be hosted before it can be opened on a phone. This is the simplest GitHub Pages option:

1. Create a new public GitHub repository, for example `happy-birthday-sia`.
2. Upload every file and folder from this project to that repository. `index.html` must be at the top level, not inside another folder.
3. In the GitHub repository, open **Settings → Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
4. Select the `main` branch and the `/(root)` folder, then click **Save**.
5. Wait for GitHub to show the live HTTPS page address, then open that address on the phone.

HTTPS is important: it allows the optional microphone candle interaction to work on supported mobile browsers.
