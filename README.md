# Quran Cube ﷺ — Ayah Visualizer

Peace and blessings upon Muhammad. Each ayah of the Qur'an rendered as a 3D cube:

- **Ayah Cube** — 14×14 horizontal grid × 28 vertical (sun letters +1..+14 above the gold plane, moon letters −1..−14 below), letter triples of the ayah placed as coloured cells in the surah's colour (from a 3×3×3 surah cube mapped onto red/yellow/blue axes). Vertical scale: base = 0–100, top = 901–1000. Hover any filled cell to read its letters. Recitation audio with 0.5× default speed.
- **Surah Cube** — the 3×3×3 cube itself, each cell a node labelled with its surah numbers (famous surahs marked ★). Click a cell to jump to that surah.
- **Reverse Draw** — place points in the empty grid and the app finds the matching ayahs.
- Letter-feelings sentences (alif = palm shoot, ba = boat, ta = coconut …) drawn from the world of the Prophet ﷺ, Hijaz and hadith imagery.

Single self-contained `index.html` (Three.js inlined, 114 first ayahs embedded). Works offline; uses the alquran.cloud API and the islamic.network audio CDN when online.

## Publish on GitHub Pages

1. Create a new repository on GitHub (e.g. `quran-cube`), public.
2. Upload the files from this folder — at minimum `index.html` (drag & drop via **Add file → Upload files** on the repo web page).
3. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, folder `/ (root)`, Save.
4. Your live app will be at `https://<your-username>.github.io/quran-cube/` within a minute or two.

No build step is needed — GitHub Pages serves the static HTML directly. Audio and full-surah text require internet; the cubes render fully offline.
