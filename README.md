# 🍼 Sonia Storm — Baby Spawn LVL 999

A birthday browser game for Sonia. Her Maternal Magic spawns a new baby every few
seconds; the babies wander off leaving 💩 poops and 🔥 fires. Walk Sonia over the
messes to clean them. Let too many pile up and the **CHAOS** meter fills — survive
as long as you can for a high score!

## ▶️ How to play / run it

**Easiest:** double-click `index.html` — it opens in your browser and just works.

If your browser is fussy about loading local images, run a tiny local server from
this folder instead:

```bash
python -m http.server 8000
# then open http://localhost:8000
```

**Controls**
- Move Sonia: **WASD** or **arrow keys**
- Or **drag / tap** anywhere (great on phones/tablets)
- Clean a mess by walking over it
- **P** or the ⏸ button to pause, 🔊 to mute

High score is saved automatically in the browser.

## 🌐 Putting it online (like the example sites)

It's a fully static site (one HTML file + the `assets/` folder), so any static host works:

- **Netlify / Vercel:** drag-and-drop this whole folder, done.
- **GitHub Pages:** push the folder to a repo, enable Pages.
- **Custom domain** (e.g. `soniastorm.com`): point it at whichever host above.

## 📁 Files

- `index.html` — the entire game (HTML + CSS + JS, no dependencies)
- `assets/sonia-player.png` — player sprite (background removed)
- `assets/gameover.png` — game-over art (background removed)
- `assets/babies/baby1–10.png` — baby sprites cropped from the concept art
- `assets/sonia-*` (originals) — kept for reference / re-cropping

## 🔧 Tuning (in `index.html`)

Look near the top of the `<script>` for easy knobs:
- `SAFE` — how many messes you can have before chaos rises (default 5)
- `MAX_BABIES` — baby cap (default 15)
- spawn ramp / chaos rate live in `update()` if you want it easier or harder.

Made with 💕 for Sonia.
