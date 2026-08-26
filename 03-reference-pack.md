# Reference Pack — Still Images (generate BEFORE video)

Generate these as **still images** in Grok Imagine first. Approve each angle before using as reference-to-video attachments. Max **7 refs per video** — shot list specifies which to attach.

**Naming convention:** Save approved stills with the filenames below so you can find them quickly in canvas.

---

## Global still prompt suffix (append to every reference still)

```
Cinematic still frame. 16:9 1080p. 2.39:1 anamorphic composition.
35mm film look, subtle grain, natural skin, ancient Mediterranean realism.
Muted earth and charcoal palette. No text. No watermark. Photorealistic.
```

---

## ODYSSEUS MASTER

### `odysseus-front.jpg`
```
Front-facing portrait of Odysseus, king of Ithaca. Weathered man late 30s-40s,
 thick dark beard with grey streaks, deep-set tired eyes, sun-darkened skin,
 wind-chapped. Coarse undyed linen cloak over bare muscular shoulders, bronze fibula.
 Neutral grey coastal background, overcast pre-dawn light. Symmetrical portrait, eyes level.
[GLOBAL STILL SUFFIX]
```

### `odysseus-3q-left.jpg`
```
Three-quarter portrait from camera-left of Odysseus. Same face, beard, costume as front master.
 Head turned slightly toward camera. Overcast coastal light, muted palette.
[GLOBAL STILL SUFFIX]
```

### `odysseus-3q-right.jpg`
```
Three-quarter portrait from camera-right of Odysseus. Same face, beard, costume as front master.
 Head turned slightly away from camera. Overcast coastal light, muted palette.
[GLOBAL STILL SUFFIX]
```

### `odysseus-profile.jpg`
```
Strict profile portrait of Odysseus facing camera-left. Same beard, nose, brow, costume.
 Grey sky background. Documentary portrait clarity.
[GLOBAL STILL SUFFIX]
```

### `odysseus-fullbody.jpg`
```
Full body of Odysseus standing on rocky shore. Coarse linen cloak, bronze belt,
 simple sandals, travel-worn. Rear-quarter light, wind in cloak. Small bronze sword at hip.
 Desolate Mediterranean coast, dark cavern mouth distant in background.
[GLOBAL STILL SUFFIX]
```

### `odysseus-rear.jpg`
```
Rear view of Odysseus walking toward dark cavern entrance on desolate shore.
 Same cloak and silhouette as full body master. Torch in hand, smoke from cavern.
[GLOBAL STILL SUFFIX]
```

---

## TIRESIAS MASTER

### `tiresias-portrait.jpg`
```
Portrait of Tiresias the blind prophet. Very old man, gaunt face, long grey hair,
 milky blind eyes or scarred closed lids, deep lines. Dark simple wool robes, bronze staff
 held vertical. Cold cavern darkness behind, faint amber torch rim light on one cheek.
[GLOBAL STILL SUFFIX]
```

### `tiresias-3q-left.jpg`
```
Three-quarter portrait of Tiresias from camera-left. Same blind face, robes, staff.
[GLOBAL STILL SUFFIX]
```

### `tiresias-profile.jpg`
```
Profile of Tiresias facing camera-right. Blind eyes, hooked nose, long beard.
 Staff visible. Low-key torch lighting, smoke in background.
[GLOBAL STILL SUFFIX]
```

### `tiresias-fullbody.jpg`
```
Full body of Tiresias standing in cavern mist. Dark robes, bronze staff, bare feet on wet stone.
 Faint human shades out of focus behind him — dim, not glowing.
[GLOBAL STILL SUFFIX]
```

---

## UNDERWORLD MASTER

### `env-shore-establishing.jpg`
```
Aerial-style establishing still: desolate rocky shore at edge of the world, pre-dawn grey sky,
 black volcanic sand, dark cavern mouth in cliff face, thin mist, small ancient ship beached distant.
 No people. Epic scale, muted palette.
[GLOBAL STILL SUFFIX]
```

### `env-ritual-pit.jpg`
```
Ground-level still: shallow ritual pit dug in black sand, bronze bowl, clay vessels,
 sheep blood dark in sand, small fire, smoke rising. Torch stuck in sand. Cavern mouth behind.
[GLOBAL STILL SUFFIX]
```

### `env-cavern-dark.jpg`
```
Interior cavern mouth still: wet stone, volumetric smoke, cold blue-black darkness beyond,
 amber firelight from foreground brazier. No figures. Oppressive depth.
[GLOBAL STILL SUFFIX]
```

### `env-shades-crowd.jpg`
```
Wide still: dozens of faint human shades standing in smoke at edge of torchlight in cavern.
 Semi-transparent, mournful, not monstrous, not glowing. Charcoal and amber palette.
[GLOBAL STILL SUFFIX]
```

---

## Optional prop insert (generate if needed)

### `prop-oar.jpg`
```
Close still of weathered wooden oar, salt-stained, lying on rocky ground. Torch light. Symbolic.
[GLOBAL STILL SUFFIX]
```

---

## Reference attachment matrix (quick lookup)

| Shots | Primary refs (pick ≤7) |
|-------|------------------------|
| 01 | env-shore-establishing |
| 02–05 | odysseus-fullbody, odysseus-rear, env-shore-establishing, env-cavern-dark |
| 06–09 | odysseus-3q-right, odysseus-fullbody, env-ritual-pit, env-shades-crowd |
| 10–12 | env-cavern-dark, env-shades-crowd, odysseus-3q-right |
| 13–15 | tiresias-portrait, tiresias-3q-left, odysseus-3q-right, env-cavern-dark |
| 16–18 | tiresias-portrait, tiresias-profile, odysseus-3q-right, env-shades-crowd |
| 19–22 | tiresias-portrait, odysseus-3q-left, odysseus-front, env-cavern-dark |
| 23–26 | tiresias-fullbody, odysseus-front, env-shades-crowd, env-cavern-dark, prop-oar |

---

## Approval checklist

Before animating shot 01:

- [ ] All Odysseus angles match same face/beard/costume
- [ ] Tiresias matches across portrait, 3q, profile, full body
- [ ] Environment palette consistent (charcoal + amber + cold blue)
- [ ] Shades in env-shades-crowd are dim human forms, not fantasy glow
- [ ] Saved with filenames above in Grok canvas or local folder
