# CODEX·OCVLVS — AI Glasses × Leonardo da Vinci

### ▶ Live: **https://codex-oculus.vercel.app**

A cinematic scrollytelling concept page that drops a pair of waveguide AI smart‑glasses into
Leonardo da Vinci's world — a fly‑through Renaissance gallery you scroll *down*, with the hero
product flying through it and opening into a spec teardown.

An unofficial concept study / portfolio piece. Built with the
[`hardware-art-crossover`](https://github.com/Aurora-zyy/hardware-art-crossover) skill.

## The five beats

1. **SEE** — the hero word over the Vitruvian Man; the glasses first enter.
2. **Not a screen. A way of seeing.** — the one‑line thesis over Leonardo's flight machine.
3. **The world, annotated.** — the quiet frame, the glasses alone in the grotto of the *Virgin of the Rocks*.
4. **An optic worth studying.** — the glasses explode into an annotated teardown over the foetus study.
5. **In the workshop.** — editorial card outro (self‑portrait + *Mona Lisa*).

## What's under the hood

- **Hero model** — waveguide AR glasses after the Even Realities G1 class: ultra‑thin monochrome
  gunmetal‑titanium frame, the signature flat rectangular temple module, clear waveguide lenses,
  a discreet flush micro‑sensor. Built procedurally in three.js (`renderer.html`) and rendered to
  a turntable + exploded image sequence (`assets/seq/`), played on a canvas and driven by scroll‑yaw.
- **Fly‑through corridor** — a CSS‑3D gallery (`#hall`/`#cam`): perspective floor grid, loggia
  arches you pass through, the da Vinci paintings hung on angled side walls. Scroll drives the
  camera forward; the pointer adds parallax sway; the teardown dissolves the hall to grounded parchment.
- **Two‑voice type** — Archivo × Cormorant. **Blueprint layer** — Leonardo's own circle‑and‑square.

## Run locally

```bash
python3 -m http.server 8137     # serve over HTTP — file:// blocks WebGL textures
# → http://localhost:8137
```

Verification / export modes: `?f=1..5` freezes a beat (still‑frame), `?p=<0..1>` scrubs the scroll.

## Credits

Artworks by **Leonardo da Vinci**, public domain, via Wikimedia Commons: Vitruvian Man; Design for
a Flying Machine; Virgin of the Rocks; Views of a Foetus in the Womb; presumed self‑portrait; Mona
Lisa. Not affiliated with any manufacturer — an unofficial concept study.
