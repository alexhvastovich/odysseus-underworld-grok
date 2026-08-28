# Stitching Order

**This cut:** shots **05–26**. 01–04 are out (triple cave entrance). Open on the last cavern-mouth take.

## Do this, in this order

1. **ID ledger.** From the first still, write shot / still UUID / video UUID / take in [`records/guide-review/CANVAS-MAP.md`](records/guide-review/CANVAS-MAP.md). Click by id. Do not invent ids.
2. **Last frame is first frame.** Same camera / same cave: extract the last frame of video N. That picture **is** the first frame of N+1. Prompt: start on this exact frame, then play the new beat. New lock still only when camera or location changes. Start/end mismatch is a miss, not a stitch trick.
3. **Ask Imagine Agent to trim and stitch.** Name the two video ids. Trim the tail of a spoken take after the line. Agent can stitch. Do not hard-concat locally first. ffmpeg xfade is fallback only.
4. **Named joins:** 05→06 fade mouth→kneeling. 08→09 trim 08, emerge from shadow (not a slam to OTS). 09→10 same cavern as 09 after 10 is remade from 09's last frame. 16→17 last-frame. 19→20 hold CU size (no close→wide same face). 24→25 after look-left. 25→26 he stays.

Paste-ready one-liners: [`records/guide-review/AGENT-FIX-PROMPT.txt`](records/guide-review/AGENT-FIX-PROMPT.txt).

---

**Rule:** Stitch only at **clear story-beat cut points**. For continuous motion within a beat, prefer **one generation from a tagged (@) storyboard sequence** — smoother than stitching micro-clips. See [`10-grok-imagine-tips.md`](10-grok-imagine-tips.md) §0.

---

## Two assembly strategies

### Strategy A — Individual shots (default in this repo)
Generate each `prompts/shot-NN.md` separately → stitch at **act breaks** below.

### Strategy B — Tagged storyboard sequences (smoother motion)
For continuous beats, one prompt with multiple `@` tagged stills → one video per beat → stitch fewer, longer segments.

| Beat | Shots | Try Strategy B? |
|------|-------|-----------------|
| Descent walk | 03–05 | ✓ one 15s @ sequence |
| Ritual | 06–08 | optional |
| Shades pressure | 09–11 | ✓ one @ sequence |
| Prophecy dialogue | 13–21 | ✗ keep separate CUs (hard cuts) |
| Close | 24–25 | ✓ one @ sequence |

---

## Full sequence (Strategy A — 26 clips)

Assemble in this order. Select clips → **Stitch** only where act breaks mark end of a beat.

```
01 → 02 → 03 → 04 → 05 → 06 → 07 → 08 → 09 → 10 → 11 → 12 → 13 → 14 → 15 → 16 → 17 → 18 → 19 → 20 → 21 → 22 → 23 → 24 → 25 → 26
```

**Expected duration:** ~242 seconds (4:02)

---

## Preferred stitch points (clear cut points only)

Stitch **between** these beats — not mid-motion:

| Stitch after | ~Time | Why (beat ended) |
|--------------|-------|------------------|
| 02 or 05 | 0:18–0:42 | Exterior descent → ritual begins |
| 08 | 1:06 | Libation done → shades stir |
| 11 | 1:33 | Sword standoff → Tiresias path opens |
| 15 | 2:14 | Setup dialogue done → prophecy block |
| 22 | 3:22 | Prophecy done → aftermath |
| 26 | 4:02 | Final |

**Do NOT stitch** mid-walk (03→04), mid-push-in (12), or mid-reaction flow (24→25) if @ storyboard sequence produced one smooth clip instead.

---

## Act breaks (optional chapter markers for review)

| After shot | Timestamp ~ | Beat |
|------------|---------------|------|
| 05 | 0:42 | Descent complete — cavern reached |
| 09 | 1:18 | Ritual done — shades released |
| 15 | 2:14 | Conversation axis locked |
| 22 | 3:22 | Prophecy complete |
| 26 | 4:02 | End |

---

## Partial stitch groups (if stitching all at once fails)

Stitch in four segments, then stitch segments:

### Segment A — Descent (shots 01–05)
`01-02-03-04-05` → ~42s

### Segment B — Ritual (shots 06–09)
`06-07-08-09` → ~36s

### Segment C — Arrival & setup (shots 10–15)
`10-11-12-13-14-15` → ~56s

### Segment D — Prophecy & end (shots 16–26)
`16-17-18-19-20-21-22-23-24-25-26` → ~108s

Then: **Stitch A + B + C + D**

---

## Trim notes

If final runtime must be **exactly 4:00**, trim 2 seconds from:
- Shot 01 (aerial) −1s, and
- Shot 20 (oar prophecy) −1s

Or trim in Grok/player if hard cuts are available post-stitch.

---

## Audio continuity

Stitch does not mix dialogue levels. Expect:
- Wind/env bed may jump between clips — normalize in post if needed
- Dialogue shots 08, 13–23 should be checked for overlap when stitched; if two lines bleed, shorten the **earlier** shot's tail and re-stitch that pair

---

## Re-stitch triggers

Re-generate and replace **individual shots** (do not re-stitch entire 4:00) when:

| Problem | Fix shot |
|---------|----------|
| Eyeline break in dialogue | Offending CU or OTS only |
| Odysseus beard/costume drift | That character's shots only |
| Tiresias face drift | 13, 16, 17, 19, 21, 23 |
| Shade glow fantasy look | 09, 10, 26 |
| Wrong line delivery | That dialogue shot only |

---

## Export checklist

- [ ] All 26 clips present in canvas
- [ ] Clips named or ordered 01–26
- [ ] Eyeline check on 13–15, 16–22 block
- [ ] Full stitch plays 4:00 ±5s
- [ ] Optional: segment stitches merged
- [ ] Download final stitch from canvas toolbar
