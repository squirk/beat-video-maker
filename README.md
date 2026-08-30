# Beat Video Maker

A browser-based, webcam music-video maker inspired by the (now-discontinued) LEGO VIDIYO app. Point your camera at yourself, drop on some stickers, pick a filter, and record a short music video — all client-side, no install, no server.

**⚠️ Not affiliated with LEGO.** This is a fan-made, unofficial project and is not affiliated with, endorsed by, sponsored by, or connected in any way to the LEGO Group. LEGO® and VIDIYO™ are trademarks of the LEGO Group, which has no involvement with this project. No LEGO artwork, character designs, or proprietary assets are used here — all visuals (stickers, effects, UI) are original.

## What it does

- **Webcam stage** — your camera feed becomes the canvas, mirrored like a selfie cam.
- **Stickers** — tap to drop emoji props onto the scene; drag to reposition, double-tap to remove.
- **Filters** — Natural, Neon Glow, Retro VHS, Black & White, Comic Pop, Sunset Warm, Ice Cool, Purple Haze.
- **Beats** — five original, synthesized backing tracks (Web Audio API, no external audio files) with a Pause/Resume control that keeps the beat's place instead of restarting it.
- **Chip Scanner** — hold up a solid-colored object (red, orange, yellow, green, teal, blue, purple, pink, black, or white — a colorful brick works great) to the marked zone, and the app recognizes the color and reacts with its own filter, beat, sticker burst, and screen effect (lightning, bursts, sparkles, confetti, bubbles, rainbows, hearts).
- **Recording** — captures a 15-second clip (video + beat baked in) you can preview and download as a `.webm` file.

## Usage

1. Open `beat-video-maker.html` in a modern browser (Chrome, Firefox, Safari, Edge).
2. Click **Enable Camera** and grant permission.
3. Play with stickers, filters, beats, and the chip scanner.
4. Hit **Record** to capture a clip, then download it.

No build step, no dependencies, no installation — it's a single self-contained HTML file.

## Notes & limitations

- Camera access requires a real browser tab (not an embedded/sandboxed preview) and a secure context (`https://` or a local file opened directly).
- The Chip Scanner reacts to plain color, not printed artwork — it doesn't recognize any specific physical product's designs.
- Recording uses the `MediaRecorder` API, so exact browser support and output format may vary slightly.

## Tech

Vanilla JavaScript, HTML5 Canvas, the Web Audio API, and `MediaRecorder` — no frameworks, no build tools, no external services.
