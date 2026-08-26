# Odysseus in the Underworld — Grok Imagine Production Pack

A **shot-by-shot production bible** for building a ~4-minute cinematic sequence in **xAI Grok Imagine 1.5** — *Odyssey* Book 11 (Odysseus meets Tiresias in Hades).

Designed for the **film-crew workflow**: generate individual 6–12s clips with reference-to-video, then **Stitch** in Grok canvas. Do **not** ask Grok for a four-minute movie in one prompt.

---

## Quick start (when your Grok limit resets)

### 1. Lock reference stills first
Open [`03-reference-pack.md`](03-reference-pack.md) and generate **still images only**:
- Odysseus (6 angles)
- Tiresias (4 angles)
- Underworld environments (4 plates)

Approve faces, costume, and palette before animating anything.

### 2. Generate shots in order
Open [`04-shot-list.md`](04-shot-list.md). For each shot **01 → 26**:
1. Open [`prompts/shot-NN.md`](prompts/)
2. Attach the listed reference images (≤7 per generation)
3. Copy the prompt block into Grok Imagine
4. Generate → review eyelines → next shot

### 3. Stitch
Follow [`05-stitching-order.md`](05-stitching-order.md). Select all clips in canvas → **Stitch** (or type *"stitch these together"*).

---

## What's in this repo

| File | Purpose |
|------|---------|
| [`01-cinematography.md`](01-cinematography.md) | Global visual rules — paste into every prompt |
| [`02-scenario-and-dialogue.md`](02-scenario-and-dialogue.md) | Book 11 story + all spoken lines |
| [`03-reference-pack.md`](03-reference-pack.md) | Still-image prompts for character/environment masters |
| [`04-shot-list.md`](04-shot-list.md) | 26-shot master table (duration, camera, refs, eyelines) |
| [`05-stitching-order.md`](05-stitching-order.md) | Assembly order + partial stitch groups |
| [`prompts/`](prompts/) | Copy-paste Grok prompts for shots 01–26 |
| [`PRODUCTION-GUIDE.md`](PRODUCTION-GUIDE.md) | Extended workflow notes |
| [`skills/`](skills/) | Cursor agent skill for this workflow |

**Runtime:** ~242 seconds (26 shots) · **Source:** Homer, *Odyssey* Book 11

---

## Feeding this to Grok

You can paste individual prompt files directly into Grok Imagine chat, or share the repo URL and ask Grok to walk the shot list with you.

**Recommended order:**
1. Paste the **Global Prompt Block** from `01-cinematography.md` once so Grok learns the look
2. Work reference pack (`03-reference-pack.md`) shot by shot
3. Work `prompts/shot-01.md` through `shot-26.md` in sequence
4. Stitch using `05-stitching-order.md`

---

## Key rules

- **One shot = one generation** (6–12s typical; 15s max)
- **1080p, 16:9** — compose for 2.39:1 anamorphic inside the frame
- **180° rule:** Odysseus eyeline camera-right; Tiresias camera-left
- **No glowing fantasy ghosts** — shades are dim, human, smoke-obscured
- **Alternate dialogue** with reactions and atmospheric inserts

---

## Quota saver

If generations are limited, see the **16 must-have shots** list in [`04-shot-list.md`](04-shot-list.md) for a ~2:30 cut with the full prophecy intact.

---

## License

MIT — use freely for personal and commercial Grok productions. Homer belongs to the ages.
