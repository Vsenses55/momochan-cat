# Sliced Cat

An interactive Three.js sculpture: a sitting cat cut into 44 parallel plates. Orbit it, and run the cursor across the plates to play them like an instrument.

## Features

- Plates are generated in the browser from a signed-distance model of the cat, using marching squares, so the plate count can change live (24–96)
- Each plate plays a pentatonic note with a synthesized struck-metal tone, panned by position, through a short reverb (Web Audio, no samples)
- Hovering wakes a translucent teal / plum / coral glass color that fades out after the cursor leaves
- Resting finish: polished steel or clear glass
- Hover motion: Tilt, Ripple or Slide; Explode spreads the plates apart

## Run locally

It is a single static file. Open `index.html` in a browser, or serve the folder with any static server:

```
npx serve .
```

## Publish with GitHub Pages

1. In GitHub Desktop, choose File → Add Local Repository (or New Repository) and point it at this folder.
2. Commit and click Publish repository. Untick "Keep this code private" if you are on a free plan, because Pages needs a public repository there.
3. On github.com, open the repository's Settings → Pages, set Source to "Deploy from a branch", pick `main` and `/ (root)`, and save.
4. The site goes live at `https://<your-username>.github.io/<repo-name>/` within a minute or two.

## Credits

The sliced-plate form is inspired by Julian Voss-Andreae's stainless steel figure sculptures. The cat model, sound and interaction are original. Three.js r128 is loaded from cdnjs and jsDelivr.
