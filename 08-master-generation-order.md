# Master Generation Order — Images First, Then Video, Then Stitch

**Complete checklist.** Work top to bottom. Do not skip to video until every still in Phase 1–3 is approved.

**Repo:** https://github.com/alexhvastovich/odysseus-underworld-grok

---

## Phase 0 — Export your anchor (you already have this)

| Step | Output | Source |
|------|--------|--------|
| 0.1 | `odysseus-anchor.png` | **`reference/odysseus-anchor.png`** (pre-generated) OR your Calypso Grok frame |

> **Pre-generated pack:** The repo includes 16 ready-to-upload PNGs in [`reference/`](../reference/). Review them first — swap in your Calypso anchor if preferred.

---

## Phase 1 — Odysseus stills (attach anchor to each)

| Step | File | Prompt in |
|------|------|-----------|
| 1.1 | `odysseus-front.jpg` | `images/01-odysseus-front.md` |
| 1.2 | `odysseus-3q-left.jpg` | `images/02-odysseus-3q-left.md` |
| 1.3 | `odysseus-3q-right.jpg` | `images/03-odysseus-3q-right.md` |
| 1.4 | `odysseus-profile.jpg` | `images/04-odysseus-profile.md` |
| 1.5 | `odysseus-fullbody.jpg` | `images/05-odysseus-fullbody.md` |
| 1.6 | `odysseus-rear.jpg` | `images/06-odysseus-rear.md` |

**Gate:** Same face, same beard pattern, same tan linen in all six. If not → regenerate before continuing.

---

## Phase 2 — Environment stills (no characters, except optional scale)

| Step | File | Prompt in |
|------|------|-----------|
| 2.1 | `env-shore-establishing.jpg` | `images/07-env-shore.md` |
| 2.2 | `env-ritual-pit.jpg` | `images/08-env-ritual-pit.md` |
| 2.3 | `env-cavern-dark.jpg` | `images/09-env-cavern.md` |
| 2.4 | `env-shades-crowd.jpg` | `images/10-env-shades.md` |
| 2.5 | `prop-oar.jpg` | `images/11-prop-oar.md` |

**Gate:** One palette — charcoal, amber torch, cold blue-black. No glowing ghosts.

---

## Phase 3 — Tiresias stills (attach odysseus-anchor for film-stock match)

| Step | File | Prompt in |
|------|------|-----------|
| 3.1 | `tiresias-portrait.jpg` | `images/12-tiresias-portrait.md` |
| 3.2 | `tiresias-3q-left.jpg` | `images/13-tiresias-3q-left.md` |
| 3.3 | `tiresias-profile.jpg` | `images/14-tiresias-profile.md` |
| 3.4 | `tiresias-fullbody.jpg` | `images/15-tiresias-fullbody.md` |

**Gate:** Same blind face in all four. Dark robes, bronze staff. Attach `env-cavern-dark` for lighting match.

---

## Phase 4 — Stage frames (optional but recommended)

Composite approved stills in Grok canvas into six stage frames (see `07-virtual-set.md`).  
These become background refs for dialogue block shots 13–25.

| Step | Stage | Refs to combine |
|------|-------|-----------------|
| 4.1 | stage-exterior | env-shore |
| 4.2 | stage-ritual | env-ritual-pit |
| 4.3 | stage-cavern | env-cavern + env-shades |
| 4.4 | stage-axis-A | env-cavern + tiresias-portrait position |
| 4.5 | stage-axis-B | env-cavern + odysseus-3q-right position |
| 4.6 | stage-axis-D | env-cavern rear wide |

---

## Phase 5 — Video clips (strict order 01 → 26)

| Step | Shot | Duration | Camera | Prompt |
|------|------|----------|--------|--------|
| 5.1 | 01 Aerial establishing | 10s | Exterior | `prompts/shot-01.md` |
| 5.2 | 02 Ship & shore | 8s | Exterior | `prompts/shot-02.md` |
| 5.3 | 03 Rear walk | 9s | Exterior | `prompts/shot-03.md` |
| 5.4 | 04 Tracking side | 8s | Exterior | `prompts/shot-04.md` |
| 5.5 | 05 Cavern mouth | 7s | Exterior | `prompts/shot-05.md` |
| 5.6 | 06 Ritual master | 10s | Master | `prompts/shot-06.md` |
| 5.7 | 07 Libation insert | 7s | Insert | `prompts/shot-07.md` |
| 5.8 | 08 Odysseus over pit | 10s | Cam B / medium | `prompts/shot-08.md` |
| 5.9 | 09 OTS shades | 9s | OTS | `prompts/shot-09.md` |
| 5.10 | 10 Shade parting | 8s | Master | `prompts/shot-10.md` |
| 5.11 | 11 Odysseus sword | 9s | Medium | `prompts/shot-11.md` |
| 5.12 | 12 Tiresias emergence | 10s | Push-in | `prompts/shot-12.md` |
| 5.13 | 13 Tiresias opens | 10s | **Camera A** | `prompts/shot-13.md` |
| 5.14 | 14 OTS → Odysseus | 9s | **Camera B** | `prompts/shot-14.md` |
| 5.15 | 15 Profile two-shot | 10s | **Camera C** | `prompts/shot-15.md` |
| 5.16 | 16 Poseidon prophecy | 10s | **Camera A** | `prompts/shot-16.md` |
| 5.17 | 17 Cattle warning | 10s | Camera A med | `prompts/shot-17.md` |
| 5.18 | 18 Odysseus question | 8s | **Camera B** | `prompts/shot-18.md` |
| 5.19 | 19 Suitors prophecy | 10s | **Camera A** | `prompts/shot-19.md` |
| 5.20 | 20 Oar prophecy | 12s | Camera A med | `prompts/shot-20.md` |
| 5.21 | 21 Death prophecy | 10s | **Camera A** | `prompts/shot-21.md` |
| 5.22 | 22 Odysseus reaction | 8s | **Camera B** | `prompts/shot-22.md` |
| 5.23 | 23 Tiresias final | 9s | **Camera A** | `prompts/shot-23.md` |
| 5.24 | 24 Odysseus hold | 7s | **Camera B** | `prompts/shot-24.md` |
| 5.25 | 25 Rear abyss | 10s | **Camera D** | `prompts/shot-25.md` |
| 5.26 | 26 Shades closing | 8s | Master | `prompts/shot-26.md` |

**After each clip:** Pre-flight check in `06-character-consistency.md`. Reject drift. Export bridge frame if helpful.

**Total video runtime:** ~242 seconds (4:02)

---

## Phase 6 — Stitch

| Step | Action |
|------|--------|
| 6.1 | Select clips 01–26 in canvas in order |
| 6.2 | Click **Stitch** (or type "stitch these together") |
| 6.3 | Review eyelines on shots 13–24 |
| 6.4 | Replace any bad clips → re-stitch affected segment only |
| 6.5 | Download final sequence |

See `05-stitching-order.md` for partial stitch groups if needed.

---

## Quick reference: what attaches to each video

| Shot block | Minimum refs |
|------------|--------------|
| 01 | env-shore |
| 02–05 | odysseus-anchor + angle + env |
| 06–11 | odysseus-anchor + angle + env |
| 12 | tiresias-portrait + tiresias-fullbody + odysseus-anchor + env-cavern |
| 13–17, 19–21, 23 | tiresias-portrait + tiresias angle + env (+ odysseus-anchor) |
| 14, 18, 22, 24 | odysseus-anchor + odysseus-front/3q + tiresias-portrait |
| 15 | odysseus-anchor + odysseus-profile + tiresias-portrait + tiresias-profile |
| 25 | odysseus-anchor + odysseus-rear + tiresias-fullbody + env-cavern |
| 26 | odysseus-anchor + env-shades + env-cavern |

---

## Scene summary (what you're building)

**One scene:** Odysseus at the edge of Hades performs the blood ritual; shades gather; Tiresias alone speaks truth; prophecy of Poseidon, cattle, suitors, oar, and gentle death; Tiresias recedes; shades close in.

**One set:** Exterior shore → ritual pit → cavern conversation axis (virtual set in `07-virtual-set.md`).

**One sequence:** 26 clips stitched → ~4 minutes.
