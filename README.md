# FaceBooth

A browser-based AR photobooth app. Draw on your live camera feed, apply filters, and capture photo strips — all running directly in the browser with no installs needed.

**Live demo:** https://kasviii.github.io/ar-tryon

---

## What it does

- **Air drawing** — click and drag on the camera feed to draw with any color and brush size
- **Filters** — Normal, B&W, Vintage, Neon, and Stars (animated floating stars over the feed)
- **Single shot** — capture one photo at a time into the strip
- **Photobooth strip** — show ✊ fist gesture to trigger a 3..2..1 countdown then 3 consecutive shots
- **Download strip** — saves all 3 shots as a single PNG strip with header and date

---

## Gestures

| Gesture | Action |
|---|---|
| ✊ Fist (hold 1s) | Start photobooth — 3..2..1 then 3 shots |
| 👍 Thumbs up (hold) | Single snap |
| 🖐 Open palm (hold) | Clear drawing |
| 🖱 Click & drag | Draw on camera |

---

## Known issues

- The fist gesture occasionally captures the hand in frame before the countdown completes — work in progress
- Gesture detection sensitivity varies with lighting conditions
- Hand tracking uses CPU fallback on some devices which may cause slight lag
- its honestly a very laggy version but if you just press click 3 pics it works perfectly, the gesture reading is the issue and also not a main component so its fine


---

## Stack

- Pure HTML / CSS / JavaScript — single file
- MediaPipe Tasks Vision (hand + face landmark detection)
- Canvas API for drawing, filters, and compositing
- Hosted on GitHub Pages

---

## Run locally

No setup needed — just open in Chrome via Live Server (VS Code extension) or push to GitHub Pages. Opening as a local `file://` will block camera access.

```bash
git clone https://github.com/kasviii/ar-tryon.git
cd ar-tryon
# open with VS Code Live Server
```

---

*Part of a series of CV and ML portfolio projects.*
