# Grok Imagine — Official & Community Tips

Extracted from **@karaebel** (xAI/Grok team), **@SebJefferies**, and creator threads.  
Use alongside this repo's shot list and reference pack. Official @imagine scene language is in [`11-imagine-cinematic-guide.md`](11-imagine-cinematic-guide.md).

**Sources:** Kara replies on X · Aug 2026 · Grok Imagine / Agent Mode updates · community (Aug 25, 2026)

---

## 0. Stitch vs tagged storyboard sequences (IMPORTANT)

**Community tip (Aug 2026):**

> Don't stitch video **unless there is a clear cut point** marking the end of a story beat.  
> Instead, use a **sequence of tagged (@) images or a storyboard** in **one generation** for smoother, continuous motion.

### When to use each

| Method | Use when |
|--------|----------|
| **Tagged @ storyboard → one video** | Same beat, continuous motion — walk, pan, push-in, dialogue flow across angles that should feel like **one take** |
| **Stitch separate clips** | **Hard cut** between story beats — exterior → ritual → Tiresias arrives → prophecy → end |

### How to do tagged sequences

1. Upload storyboard stills to References (tag each: `@Odysseus`, `@env-cavern`, etc.)
2. In **one prompt**, describe a multi-shot sequence with inline tags:

```
Four shot sequence:

1. Wide — @env-shore-establishing — Odysseus small figure walks toward cavern at dusk.
2. Medium rear — @Odysseus rear ref — same walk continues, torch in hand.
3. Side track — @Odysseus profile — lateral follow, same continuous walk.
4. Low wide — @env-cavern-dark — he reaches cavern mouth. Beat ends. Hold.

Continuous motion throughout. 35mm grain. No music. 15s.
```

3. Generate **one clip** per beat — smoother than stitching 4 separate walk clips

### Map to this production

| Beat | Recommended approach |
|------|---------------------|
| **Descent walk** (03–05) | Try **@ storyboard sequence** in one 15s gen; stitch to Act I only if cuts needed |
| **Ritual** (06–08) | **Stitch OK** at end of 08 — clear beat change when shades stir (09) |
| **Shades + sword** (09–11) | **@ sequence** possible (OTS → medium → sword draw) OR separate gens + stitch at 11 |
| **Tiresias prophecy** (13–21) | **Stitch between CUs** — each line is a new camera; cut points are intentional |
| **Aftermath** (23–26) | **@ sequence** for 24–25 (reaction → rear abyss) if motion should flow |

**Contest export:** Still need **3–5 min** final — assemble beat-level clips (whether from @ sequences or individual shots) with **Stitch only at act breaks**.

See updated [`05-stitching-order.md`](05-stitching-order.md).

---

## 1. Character consistency (most important)

### Lock references with `@`
- Click **+** in the prompt bar → **References**
- Save approved characters to your library (e.g. `@Odysseus`, `@Tiresias`)
- In **Imagine** and **Agent Mode**: type **`@Odysseus`** in prompts to lock face/voice/costume
- Character `@` refs work in **Agent Mode** as of Aug 17, 2026 (use `@` in agent chat)

### Multi-picture → video
- Kara recommends **multi-picture to video** model for maintaining identity across clips
- Still add skin/texture language in the prompt even when using this model

### Our repo workflow
```
reference/odysseus-anchor.png  →  upload to References as @Odysseus
reference/tiresias-portrait.png →  upload as @Tiresias
Attach ≤7 refs per generation + @ handle in prompt text
```

---

## 2. Avoid plastic / soft skin

**Problem:** Video pass softens skin vs source still — looks plastic.

**Fixes (Kara):**
| Fix | Prompt / action |
|-----|-----------------|
| Start strong | Source still must already have natural skin texture |
| Film stock language | `"Kodak Portra 400 style"` or `"35mm film look, heavy grain"` |
| Skin explicitly | `"natural skin texture"`, `"visible sweat"`, `"light sheen under torchlight"` |
| Micro-movement | `"subtle realistic micro-movements in face and body"` |
| Model | Use **multi-picture to video** + above language together |

**Add to every Odysseus/Tiresias video prompt:**
```
Natural skin texture, wind-chapped, not plastic, not airbrushed.
35mm film look, shallow depth of field, heavy film grain.
```

---

## 3. Time-stamped direction (stop the model looping wrong)

**Problem:** Imagine agent ignores direction or loops wrong action.

**Fix:** Timestamp beats inside the prompt:

```
0:00–0:03 — Odysseus looks camera-right toward Tiresias, still, listening.
0:03–0:07 — slight drop of gaze; weight lands on his face. No smile.
0:07–0:10 — he speaks: "Is there no other path?" Low, grave voice.
Camera locked throughout. Never look at lens.
```

Use this format in **`prompts/shot-NN.md`** for dialogue shots (13–23).

---

## 4. Canvas / collage method (hard camera angles)

**Problem:** Changing angle moves characters to wrong positions in the set.

**Kara's fix when you MUST have a specific angle:**
1. Crop each character from an approved still (good face/lighting)
2. Crop the background plate separately
3. Composite on a canvas (Photoshop, Figma, Grok canvas) — place characters in **correct seats/positions**
4. Screenshot the composite
5. Upload screenshot → prompt: *"Place character A and character B in this scene — integrated into lighting, not as cutouts"*

**When to use in our production:**
- Profile two-shot (shot 15) if eyelines keep breaking
- OTS dialogue (shots 14, 18) if 180° rule fails after 2 retries
- Virtual set diagram: [`07-virtual-set.md`](07-virtual-set.md)

**Mindset tip:** Ask first — *"Do I really need this exact angle?"* Often a nearby camera from the virtual set works better.

---

## 5. Cinematic prompt template (proven format)

From successful Odyssey creators (Seb Jefferies / community):

```
[GLOBAL VISUAL — 35mm, grain, palette]

[CHARACTER @Odysseus — locked refs attached]

ACTION (with beats in parentheses):
"(Quiet pause. He lowers his gaze toward the ritual pit.)"
Dialogue: "Stay back… until the blood is tasted." — low, grave voice.

CAMERA: 85mm locked. Micro-handheld only. No unmotivated move.

PHYSICAL: Wind in hair and cloak. Natural skin texture. Micro-movements.

LOOK: 35mm film, shallow DOF, heavy grain. No text. No watermark.

AUDIO: Environmental only — wind, cavern drip, distant gibbering shades. No music.

Duration: 10 seconds. 1080p. 16:9.
```

---

## 6. Mode & quality workflow

| Step | Setting |
|------|---------|
| Explore / iterate | **Speed Mode** — fast, cheap iterations |
| Hero shots (CU dialogue) | **Quality Mode** or upscale Speed output |
| Final video | **1080p** · **6s / 10s / 15s** per shot (vary length — not all 15s) |
| Assembly | Select clips → **Stitch** in canvas |

Bradshannon/Kara tip: **Generate in Speed → upscale** for stills you lock as references.

---

## 7. Action / choreography (if you add combat later)

For suitor flash-forward or any action (Kara on fight scenes):
- **Shorter clips + frequent cuts** — pick the 2–3 seconds that work, discard the rest
- **Use Grok Bot to write movement beat-by-beat** before Imagine generation
- Do not ask for long fight in one 15s clip

*Book 11 note: no fight in the Underworld — sword standoff only. See [`02-scenario-and-dialogue.md`](02-scenario-and-dialogue.md).*

---

## 8. Audio rules (contest-winning pattern)

```
Audio: environmental sound only.
[wind | cavern drip | distant ocean | faint gibbering of many dead]
No music. No score.
```

Dialogue shots: specify **"low, grave voice"**, **"natural lip sync"**, delivery emotion in parentheses.

---

## 9. Full production workflow (Sebastien Jefferies)

```
1. Grok Bot    → paste shot list / 08-master-generation-order.md → plan beats
2. Grok Imagine → storyboard stills (our reference/ + images/ prompts)
3. Grok Imagine → one shot per generation, @ refs + dialogue
4. Stitch      → 3–5 min master
5. X           → quote-tweet @grok announcement with final video
```

Contest: **3–5 min · ≥1 min English dialogue · Grok Imagine video + voice**  
Rules: [`09-grok-odyssey-challenge-rules.md`](09-grok-odyssey-challenge-rules.md)

---

## 10. Quick checklist before each generation

- [ ] `@Odysseus` / `@Tiresias` locked in References
- [ ] Anchor PNG attached (slot 1)
- [ ] Skin texture language in prompt
- [ ] Time-stamped beats for dialogue shots
- [ ] Eyeline + 180° rule stated
- [ ] Environmental audio only, no music
- [ ] Duration 6–12s (not default 15s every time)
- [ ] Reject plastic skin → regenerate with Kodak Portra / grain language

---

## 11. Map tips → our shot list

| Tip | Apply to shots |
|-----|----------------|
| `@` character lock | All Odysseus 02–11, 14, 18, 22, 24–26; all Tiresias 12–23 |
| Time-stamped beats | 08, 13–23 (dialogue) |
| Multi-picture → video | 13–22 (prophecy block) |
| Canvas collage retry | 14, 15, 18 if OTS eyelines fail |
| Distant shade depth | 09, 10, 11, 26 + `env-shades-crowd.png` |
| Speed → upscale | Reference stills in `images/` phase |
| Stitch | Final — `05-stitching-order.md` |

---

## 12. What xAI is still improving

Kara noted (Aug 2026): team is **actively improving** natural skin texture preservation in video — until then, use prompt language + multi-picture model + strong source stills.

Character `@` refs in Agent Mode shipped Aug 17, 2026 — use for voice consistency across dialogue shots.
