# Virtual Set — Ritual Pit & Conversation Axis

Design the **entire set once**. Every dialogue shot uses one of four locked camera positions. Grok repeatedly "shoots" from these positions — that is what makes stitched clips feel like one location.

---

## Top-down set diagram

```
                    [ DEAD / ABYSS ]
                    smoke, darkness,
                    shades at edge of light
                           ↑
                           │
         torch brazier     │     ritual pit
              🔥           │        (blood/fire)
                           │
    TIRESIAS ●─────────────┼─────────────● ODYSSEUS
    (blind prophet)   conversation axis   (kneeling/standing)
         │                                   │
         │         Camera C (TWO SHOT)       │
         │         profile, 50mm, side       │
         │                                   │
    Camera A                          Camera B
    (Tiresias CU)                     (Odysseus CU)
    behind Odysseus shoulder          behind Tiresias shoulder
    85mm OTS → Tiresias               85mm OTS → Odysseus
         │                                   │
         └─────────── Camera D ──────────────┘
                   (REAR WIDE)
              behind both, facing abyss
                    40mm wide
```

---

## Set geography (lock for Acts II–V)

| Zone | Description | Lighting |
|------|-------------|----------|
| **North (upstage)** | Abyss / dead realm. Pure darkness with faint human shapes in smoke. No glow. | Cold blue-black fill |
| **Center** | Conversation axis. Packed black sand, wet stone. | Torch amber key + underfill from pit |
| **South (downstage)** | Ritual pit — blood, clay vessels, bronze bowl, small fire | Fire underlight + amber |
| **East/West edges** | Shade crowd — dozens of faint figures at torchlight perimeter | 1–2 stops under key |

**Odysseus position:** Camera-right of frame in dialogue (looks CR toward Tiresias).  
**Tiresias position:** Camera-left of frame in dialogue (looks CL toward Odysseus).

---

## Camera positions → shots

| Camera | Lens | Movement | Used in shots |
|--------|------|----------|---------------|
| **A — Tiresias CU** | 85–100mm | Locked, micro-handheld | 13, 16, 19, 21, 23 |
| **B — Odysseus CU** | 85mm | Locked or subtle push | 18, 22, 24 |
| **C — Profile two-shot** | 50mm | Locked | 15 |
| **D — Rear wide** | 40mm | Locked | 25 |
| **OTS A→B** | 85mm over Tiresias | Locked | 14 |
| **Master wide** | 35–40mm | Locked or slow push | 06, 10, 12, 26 |
| **Odysseus medium** | 50–65mm | Locked | 08, 11 |
| **Insert** | 100mm+ | Locked | 07 |
| **Exterior / descent** | 24–50mm | Drift / track | 01–05 |

---

## Shot grammar (this sequence)

For the full 4-minute piece, coverage follows classical film grammar:

```
Aerial → Master → Medium → OTS → CU-A → CU-B → Profile two-shot → Rear → Reaction → Establishing
```

**Act I (Descent):** Aerial → Master → Rear walk → Track → Establishing cavern  
**Act II (Ritual):** Master → Insert → Medium → OTS shades  
**Act III (Meeting):** Master → Medium → Push-in → CU-A → OTS → Two-shot  
**Act IV (Prophecy):** CU-A × 4 → CU-B → CU-A × 3 (alternate who speaks)  
**Act V (Close):** CU-A final → CU-B reaction → Rear wide → Master shades  

---

## Eyeline map (180° rule)

```
         ABYSS
           ↑
  Tiresias ← • → Odysseus
   looks CL    looks CR
           ↓
         RITUAL PIT
```

| Character | Screen position | Eyeline | Never |
|-----------|-----------------|---------|-------|
| Tiresias | Frame left | Camera-left (toward Odysseus) | At lens |
| Odysseus | Frame right | Camera-right (toward Tiresias) | At lens |

**Camera A** sits on Odysseus's side → sees Tiresias CL.  
**Camera B** sits on Tiresias's side → sees Odysseus CR.  
Do not cross the conversation axis between shots 13–24.

---

## Stage frames before animating (Grok canvas)

Create **empty stage frames** in canvas for each camera position using environment stills:

| Stage frame | Build from refs | Purpose |
|-------------|-----------------|---------|
| `stage-exterior` | env-shore-establishing | Shots 01–05 |
| `stage-ritual` | env-ritual-pit + pit fire | Shots 06–09 |
| `stage-cavern` | env-cavern-dark + env-shades-crowd | Shots 10–12, 26 |
| `stage-axis-A` | env-cavern-dark, torch left, abyss up | Tiresias CU shots |
| `stage-axis-B` | same set, reversed eyeline | Odysseus CU shots |
| `stage-axis-C` | both characters in profile | Shot 15 |
| `stage-axis-D` | rear view toward abyss | Shot 25 |

Animate **from the stage frame** + character refs for that camera position.

---

## Visual rules (apply to every generation on this set)

```
35mm anamorphic • 2.39:1 inside 16:9 • 1080p
Ancient Mediterranean realism • Nolan-adjacent practical cinematography
Muted earth/charcoal palette • volumetric smoke • natural skin
Realistic linen/wool • subtle grain • no fantasy glowing ghosts
Environmental audio: wind, cavern drip, fire, distant surf (exterior only)
```
