# STATIONS — Hybrid Training Timer

**A precision training timer for athletes who program their own sessions.**

🔗 [Live App](https://clarenceos.github.io/STATION-HybridTimer/) &nbsp;·&nbsp; ☕ [Ko-fi](https://ko-fi.com/clarenceos)

---

## What it is

STATIONS is a free, open-source PWA built for hybrid athletes — Hyrox, CrossFit, and anyone who programs their own training. No subscriptions. No ads. No account required. Everything lives on your device.

My ADHD brain makes it difficult to run workouts completely from memory. I built this so I — and athletes like me — could focus on training, not tracking.

---

## Features

### WOD Builder
- Build workouts station by station with 135+ seeded exercises
- Station types: Exercise, Cardio, Complex (movement chains), Interval, AMRAP
- Unit types: Reps, Meters, Seconds, Steps, AMRAP
- Equipment categories: Kettlebell, Dumbbell, Barbell, Medicine Ball, Sandbag, Bodyweight, TRX, Cardio, Interval
- Build and save complexes (e.g. 10× KB Swing → 5× KB Press)
- WOD tags + searchable library
- Export and import WODs as JSON (cross-device)

### Timer
- Dual display: Station Time + Total Time (wall-clock)
- Interval stations with auto-lap countdown
- AMRAP stations with auto-lap + voice countdown (halfway, last 10s, 5-4-3-2-1)
- Pause/resume with freeze and wall-clock tracking
- Undo last lap
- Landscape split view (iPad)
- Wake lock — timer survives app switching

### Voice Coaching
- Announces each station at the top of every LAP
- Full Readout mode: reads weight, reps, distance, and notes
- Speakified: "KB" → "kettlebell", "kg" → "kilograms"
- Pause / Resume / Undo / Workout Complete announcements
- AMRAP countdown: halfway, last 10 seconds, 5-4-3-2-1

### Session History & Journal
- Full lap breakdown per session
- Basic / Advanced summary toggle
- 6-metric post-session journal (RPE, energy, breathing, hydration, soreness, satisfaction)
- Copy as Markdown or export as CSV
- Session data stays on your device

---

## Stack

Single-file PWA — all HTML, CSS, and JavaScript inline in one file.

| Layer | Tech |
|-------|------|
| Storage | IndexedDB via [idb](https://www.npmjs.com/package/idb) |
| Audio | Web Audio API |
| Voice | SpeechSynthesis API |
| Wake Lock | Screen Wake Lock API |
| Deployment | GitHub Pages |

No build step. No framework. No backend. No dependencies beyond the idb CDN.

---

## Getting Started

Open [clarenceos.github.io/STATION-HybridTimer](https://clarenceos.github.io/STATION-HybridTimer/) in Safari on iPhone or iPad.

For the best experience, install to your Home Screen:
1. Tap the **Share** icon in Safari
2. Tap **Add to Home Screen**
3. Open from your Home Screen like a native app

All features — including clipboard copy — work best when installed.

---

## Roadmap

| Version | Feature | Status |
|---------|---------|--------|
| v3.4 | TRX category, voice timing fixes, AMRAP weight, notes button | ✅ Shipped |
| v3.5 | EMOM mode | 🔨 Building |
| v3.6 | Tabata + HIIT Intervals | Planned |
| v3.7 | WOD-level AMRAP | Planned |
| v3.8 | For Time format | Planned |

---

## Local Development

No build tools required.

```bash
git clone https://github.com/clarenceos/STATION-HybridTimer.git
cd STATION-HybridTimer
npx serve .
```

Open the local URL in your browser. For full feature testing (clipboard, wake lock), deploy to GitHub Pages and test on a real device.

---

## Contributing

This is a personal project built for my own training, open-sourced so others can use and learn from it. Issues and PRs are welcome — especially for bug reports from real workouts.

---

## Support

STATIONS is free and will stay free. If it's made one workout better, consider buying me a coffee.

☕ [ko-fi.com/clarenceos](https://ko-fi.com/clarenceos)

---

## License

MIT
