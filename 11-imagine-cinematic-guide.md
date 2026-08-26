# Odyssey Challenge Cinematic Guide

Official @imagine scene help. Source: https://x.com/imagine/status/2092675531057885288  
Article: https://x.com/i/article/2092302666345164800  
Posted 2026-08-26. Deadline reminder: August 31.

Use this on every Odysseus generate. Do not treat "cinematic" as a prompt word.

---

## 1. Aim before you create

**What should the scene do for the viewer?**

Answer this first. The experience you want drives shot selection.

Example (Cyclops, not our Book 11 scene):
- A scene about the Cyclops could emphasize how cunning Odysseus is.
- It could just as well focus on what it means for a leader like Odysseus to see his men being eaten alive, and how he decides to take back his power in a desperate situation.

**Our Book 11 aim (lock):** Odysseus at the edge of Hades performs the blood ritual; shades gather; Tiresias alone speaks truth; prophecy of Poseidon, cattle, suitors, oar, and gentle death. The viewer should feel scale, hunger of the dead, and the weight of a path with no other road.

---

## 2. Glossary of helpful prompting words

Do not prompt "cinematic." Use specific film language.

**Shot size:** extreme wide shot, wide, medium, close-up, extreme close-up, over-the-shoulder, POV.

On Grok Imagine canvas you can generate several of these stills in one go, then pick.

**Angle:** eye level, low angle, high angle, bird's-eye, dutch angle

**Move:** camera static, pan, tilt, dolly in, dolly out, push-in, pull-out, handheld

**Lens:** 24mm wide-angle, 35mm, 50mm normal, 85mm portrait, shallow depth of field

This pack already maps those to shots 01–26 in `01-cinematography.md` and `prompts/shot-NN.md`.

---

## 3. Film-style realistic aesthetic

### Speed Mode for base images
Use **Speed Mode** to explore characters, scenes, aesthetics. It has a cinematic vibe. Then upscale with **Quality Mode**.

Quality Mode is optimized for precision, accurate text, and professional stills (infographics, ads, photography). For this film, Speed for exploration, Quality to lock a still.

### Upscale in Quality Mode
Generate a Speed still (often 720p). Prompt to upscale to 1080p in Quality Mode. Aesthetic holds. If a tint (example: yellow-tint) must stay, put that word in the upscale prompt.

### Animate with omni-reference to video
The omni-reference video model takes **multiple images** as refs. Smartest current model. Locks aesthetics, characters, locations, props.

You can use an uploaded image as a **first frame** or as a **guide**.

Example from the official guide: Penelope had 3 refs, Odysseus had 1, then they animated the two-character scene.

**Our attach rule stays:** one Odysseus anchor on every Odysseus shot, plus the matching angle, plus env. ≤7 refs.

---

## 4. Prompt like a director

Short prompts sometimes win. Long prompts need more context of what the model should do.

Director checklist (from the official Penelope/Odysseus example):

- **What is the shot like?** Wide shot from the cliffside, camera static.
- **What are they doing?** They are silent standing side-by-side looking out at the ocean together but feeling distant. Not looking into the camera.
- **How is the speech?** A beat before she speaks. Long pause. Emphasis. Speed-up when angry. Eyes darting.
- **What else should the model remember?** Preserve natural skin, natural pores, fine lines. Nature sounds and ocean sounds. No music.

Put all of those in the prompt when the shot needs it.

Our dialogue shots (08, 13–23) should spell beat / pause / emphasis the same way. Env shots stay environmental audio only.

---

## Generate-day order (this pack)

1. Aim is locked (Book 11 prophecy, not Cyclops).
2. Still lock: use `reference/` pack. Speed+Quality only if Alex rejects a face.
3. Video: omni-reference, one shot at a time, attach listed refs, paste `prompts/shot-NN.md`.
4. First unlocked generate: shot 01 only, attach `env-shore-establishing`, `READY-shot-01.txt`.
5. Stitch in Imagine canvas after Alex locks the clips.

Good luck line from @imagine: they read feedback weekly.
