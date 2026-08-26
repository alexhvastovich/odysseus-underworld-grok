# Character Consistency Bible

**This is the most important file in the production.** Stitching cannot fix a face that changes between shots. Lock characters here before generating video.

---

## Rule zero: one anchor, many angles

Do **not** regenerate Odysseus from text alone for each shot. That is how you get a different man in every clip.

**Workflow:**
1. Pick your **best approved Odysseus** (your Calypso-scene still or video frame — the bearded man in coarse tan linen).
2. Save it as **`odysseus-anchor.jpg`** — this is sacred; do not replace casually.
3. Generate every other Odysseus angle **from that anchor** using reference-to-image (attach anchor + angle prompt).
4. Generate every Odysseus **video** with the anchor + relevant angle stills attached (≤7 refs).
5. Repeat the same anchor chain for **Tiresias** once his portrait is approved.

---

## Locked Odysseus descriptor (copy into every Odysseus prompt)

Use this **verbatim** whenever Odysseus appears. Do not paraphrase the face.

```
SAME EXACT CHARACTER as reference images — do not alter face identity.
Odysseus of Ithaca: weathered man late 30s-40s, thick dark wavy hair with grey at temples,
 full salt-and-pepper beard (dark brown-black with distinct grey streaks, same density and line as reference),
 deep-set brown eyes, sun-darkened skin, straight nose, strong brow, wind-chapped lips.
 Costume IDENTICAL to reference: coarse undyed tan/beige hand-woven linen cloak over bare shoulders,
 same fabric texture and drape, same bronze fibula at shoulder, bronze belt, simple sandals,
 small bronze sword at hip. Same beard length and hair length as reference.
 Never look into camera lens.
```

### Your existing anchor (Calypso scene)

If you already have the approved look from your Calypso generations (screenshot canvas):
- Export the **top still** or best **1080p video frame** as `odysseus-anchor.jpg`
- That face/beard/costume **is** the master — do not re-roll a "better" Odysseus
- Underworld shots use **darker lighting** (torch, cavern) but the **same face and same linen**

> **Lighting ≠ identity.** Palette shifts to charcoal/amber for Hades; jawline, beard pattern, and costume stay locked.

---

## Locked Tiresias descriptor (copy into every Tiresias prompt)

Generate Tiresias **after** Odysseus anchor is locked. First portrait must feel like the same film, different person.

```
SAME EXACT CHARACTER as Tiresias reference images — do not alter face identity.
Tiresias: very old blind prophet, gaunt hollow cheeks, long thin grey hair,
 milky blind eyes or scarred lids, hooked nose, thin grey beard,
 dark charcoal wool robes (simple, no ornaments), bronze staff with worn grip.
 Ancient but frail — not a generic wizard. Same face in every Tiresias shot.
 Never look into camera lens; sightless eyes fixed slightly off-axis toward Odysseus.
```

---

## Reference-to-video: the 7-slot formula

Grok allows **up to 7 reference images** per generation. Spend them deliberately.

### Every Odysseus video shot (minimum refs)

| Slot | Attach | Why |
|------|--------|-----|
| 1 | `odysseus-anchor.jpg` | Identity lock — always |
| 2 | `odysseus-front.jpg` | Face front anchor |
| 3 | angle matching shot (3q-right / 3q-left / profile / fullbody / rear) | Pose + angle |
| 4–5 | environment ref(s) | Location/lighting |
| 6 | optional: previous approved video frame from nearest shot | Continuity bridge |
| 7 | optional: second Odysseus angle | Dialogue shots: add profile |

**Never skip slot 1.** If you only attach one image, make it the anchor.

### Every Tiresias video shot (minimum refs)

| Slot | Attach | Why |
|------|--------|-----|
| 1 | `tiresias-portrait.jpg` | Identity lock — always |
| 2 | `tiresias-3q-left.jpg` or `tiresias-profile.jpg` | Angle match |
| 3 | `odysseus-anchor.jpg` | Scale/skin-tone/film-stock match to Odysseus scenes |
| 4 | `env-cavern-dark.jpg` | Underworld lighting |
| 5–7 | shades / props / Odysseus angle for eyeline match | Per shot list |

### Two-shots and OTS (shots 14, 15, 25)

Attach **both** character anchors + both angle refs + environment:
```
odysseus-anchor, odysseus-3q-right, tiresias-portrait, tiresias-profile, env-cavern-dark
(+ env-shades-crowd or env-ritual-pit if room)
```

---

## Deriving angle stills from your anchor (image-to-still)

For each missing angle, attach **`odysseus-anchor.jpg`** and prompt:

```
Using the EXACT same man from the reference image — same face, same beard pattern,
 same costume, same age — generate a [front / 3q-left / profile / full body / rear] still.
 Change ONLY camera angle and pose. Do not change facial features or costume.
[GLOBAL STILL SUFFIX from 03-reference-pack.md]
 Underworld lighting variant: pre-dawn grey OR torch amber as specified.
```

**Reject and regenerate** if beard pattern, nose, or costume texture drifts.

---

## Pre-flight check (before every video generation)

Answer these. If any is **no**, fix refs before burning quota.

- [ ] `odysseus-anchor.jpg` attached?
- [ ] Angle still matches this shot's camera direction?
- [ ] Costume is tan/beige linen (not leather armor, not white toga)?
- [ ] Beard is salt-and-pepper (not solid black, not short stubble)?
- [ ] Eyeline specified (never at lens)?
- [ ] For Tiresias: blind eyes + dark robes match portrait ref?
- [ ] For dialogue: 180° rule preserved (Odysseus CR, Tiresias CL)?

---

## When a shot fails consistency

1. **Do not stitch it.** Mark as rejected.
2. Regenerate with **same prompt** + add:
   ```
   CRITICAL: Match reference face exactly. Previous attempt altered beard/face — unacceptable.
   ```
3. If two retries fail, attach **approved frame from previous successful shot** as extra ref (slot 6).
4. Never "fix" consistency in stitch — replace the shot.

---

## Consistency killers (avoid in prompts)

| Bad prompt habit | Result |
|------------------|--------|
| "A Greek hero" without refs | New face every time |
| "Odysseus" text only, no anchor attached | Drift |
| Changing costume ("armored", "royal robes") | Breaks continuity |
| "Younger Odysseus" / "older" | Face drift |
| Bright fantasy Underworld glow | Different film stock feel |
| Multiple characters described in one 10s shot | Identity mush |

---

## Shot-by-shot: mandatory character refs

| Shots | Odysseus refs required | Tiresias refs required |
|-------|------------------------|------------------------|
| 01 | — | — |
| 02–05 | anchor + fullbody or rear + profile | — |
| 06–09 | anchor + 3q-right + fullbody | — |
| 10–11 | anchor + 3q-right | — |
| 12 | anchor (background scale) | portrait + fullbody |
| 13 | anchor (OTS background) | portrait + 3q-left |
| 14 | anchor + 3q-right | portrait |
| 15 | anchor + profile | profile |
| 16–17 | anchor (optional BG) | portrait + 3q-left |
| 18, 22, 24 | anchor + front + 3q-right/left | — |
| 19–21 | — | portrait + profile/fullbody |
| 23 | — | portrait |
| 25 | anchor + rear | fullbody |
| 26 | anchor + fullbody (silhouette) | — |

---

## Bridge frames (advanced)

After approving shot 03, export its last frame as `odysseus-bridge-act1.jpg`.  
Attach it when generating shot 04. Repeat for each act boundary.

This keeps **costume drape, hair wind, and lighting transition** smoother than stills alone.

---

## Tiresias introduction rule

First Tiresias generation (shot 12) must establish him in the **same cavern** as Odysseus refs:
- Attach: `tiresias-fullbody`, `odysseus-anchor`, `env-cavern-dark`, `env-shades-crowd`
- Prompt must say: *"Same cinematic world and film stock as Odysseus reference."*

Every later Tiresias shot uses `tiresias-portrait` in slot 1 — no exceptions.
