# Woof! Roar! Vroom! 🐶🦖🛻

A tap-and-play browser game for toddlers. No reading, no losing, no timers — every tap makes a sound and something fun happen.

**Play it:** https://woof-roar-vroom.vercel.app

Install it like an app: open the link in Chrome on a phone → menu → **Add to Home screen**. Works offline after the first visit.

## Worlds

| World | What happens |
|---|---|
| 🐶 Pups | Rescue puppies, fire truck, kitty-in-a-tree rescue |
| 🦖 Dinos | Roaring T-Rex, erupting volcano, hatching egg |
| 🛻 Trucks | Monster trucks doing wheelies + a jump ramp |
| 🚜 Diggers | Knock-down block tower, crane, dump truck |
| 🚂 Trains | Steam train, crossing signal, tunnel |
| ✈️ Planes | Runway takeoff, helicopter, control tower |
| 🔍 Find It! | Where's-Waldo seek-and-find with levels (saved on device) |
| 🐮 Farm | Animal sounds, barn, tractor |
| 🐳 Ocean | Whale, shark, poppable bubbles |
| 🎈 Pop! | Endless balloon popping |
| 🥁 Music | 8 instruments + pentatonic xylophone |
| 🎆 Boom! | Tap-anywhere fireworks |

## Tech

- One self-contained `index.html` — no build step, no dependencies, no external assets.
- All sounds synthesized with the Web Audio API.
- PWA: `manifest.webmanifest` + `sw.js` service worker for offline play.

## Deploying

```
vercel deploy --prod --yes
```

When shipping changes, bump the `CACHE` version string in `sw.js` so installed clients pick up the update.

Auto-deploys from `main` via the Vercel GitHub integration.
