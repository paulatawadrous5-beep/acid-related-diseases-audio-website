# Acid Related Diseases — Arabic Audio Website

Arabic audio explanation of the 65-slide "Acid related diseases — basic module" PowerPoint, with English medical terms kept as in the slides.

- 6 lessons, 32 narrated scenes (about 17 minutes of Arabic narration)
- Images are the original PowerPoint images, plus site-drawn animated diagrams
- While narration plays, the scene image stays visible and a caption overlay (the scene's opening spoken sentence) fades in over the image in a bottom gradient band, in the same teal/dark stage style — the captions and points below the player are unchanged
- Player: play/pause, next/previous scene, playback speed, scene list with durations, gallery of all PowerPoint images linked to their slides, and the full Gastric vs Duodenal Ulcer comparison table

## Run locally

Serve this folder with any static server (opening `index.html` directly works for the page, but audio/image paths resolve most reliably over HTTP), for example:

```sh
python3 -m http.server 8000
```

then open http://localhost:8000/

## Structure

- `index.html` — the full site (same design as the delivered audio website, plus the on-image overlay caption)
- `assets/img/` — PowerPoint images (`.jpg` files are the ones the page references; `.png` copies are the original PNG sources where applicable)
- `assets/audio/` — 32 Arabic narration MP3s, one per scene (`l{lesson}s{scene}.mp3`)
