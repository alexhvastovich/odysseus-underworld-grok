# Odysseus in the Underworld — Grok Imagine Production Pack

A **shot-by-shot production bible** for building a ~4-minute cinematic sequence in **xAI Grok Imagine 1.5** — *Odyssey* Book 11 (Odysseus meets Tiresias in Hades).

**Grok Odyssey Challenge:** See [`09-grok-odyssey-challenge-rules.md`](09-grok-odyssey-challenge-rules.md) — $175K prizes, deadline **Aug 31, 2026**.

Designed for the **film-crew workflow**: generate individual 6–12s clips with reference-to-video, then **Stitch** in Grok canvas. Do **not** ask Grok for a four-minute movie in one prompt.

---

## Quick start (when your Grok limit resets)

### 1. Reference stills — **pre-generated in `reference/`**
Download the [`reference/`](reference/) folder (16 PNGs) and upload to Grok canvas.

**Or** replace `odysseus-anchor.png` with your approved Calypso frame, then regenerate angles using [`images/`](images/) prompts.

Skip to Phase 5 video when stills pass your review. See [`08-master-generation-order.md`](08-master-generation-order.md).

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
| [`06-character-consistency.md`](06-character-consistency.md) | **Anchor workflow + 7-ref formula — read before generating** |
| [`07-virtual-set.md`](07-virtual-set.md) | Virtual set diagram + Camera A/B/C/D positions |
| [`08-master-generation-order.md`](08-master-generation-order.md) | **Full checklist: all images → all video → stitch** |
| [`09-grok-odyssey-challenge-rules.md`](09-grok-odyssey-challenge-rules.md) | **Official @grok contest rules + submission checklist** |
| [`10-grok-imagine-tips.md`](10-grok-imagine-tips.md) | **Kara/@grok tips: @refs, skin texture, timestamps, canvas method** |
| [`11-imagine-cinematic-guide.md`](11-imagine-cinematic-guide.md) | **Official @imagine Odyssey cinematic guide — aim, film language, Speed/Quality, omni-ref, director prompts** |
| [`images/`](images/) | Copy-paste prompts for every still (15 images) |
| [`reference/`](reference/) | **Pre-generated PNG reference pack (16 files)** |
| [`prompts/`](prompts/) | Copy-paste Grok prompts for shots 01–26 |
| [`PRODUCTION-GUIDE.md`](PRODUCTION-GUIDE.md) | Extended workflow notes |
| [`skills/`](skills/) | Cursor agent skills: cinematic sequence + Imagine cinematic scenes |

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

- **One anchor face** — export your approved Odysseus still; attach it to every Odysseus shot
- **One shot = one generation** (6–12s typical; 15s max)
- **1080p, 16:9** — compose for 2.39:1 anamorphic inside the frame
- **180° rule:** Odysseus eyeline camera-right; Tiresias camera-left
- **No glowing fantasy ghosts** — shades are dim, human, smoke-obscured
- **Alternate dialogue** with reactions and atmospheric inserts
- **Stitch does not fix faces** — reject and regenerate inconsistent shots

---

## Quota saver

If generations are limited, see the **16 must-have shots** list in [`04-shot-list.md`](04-shot-list.md) for a ~2:30 cut with the full prophecy intact.

---

## License

MIT — use freely for personal and commercial Grok productions. Homer belongs to the ages.
