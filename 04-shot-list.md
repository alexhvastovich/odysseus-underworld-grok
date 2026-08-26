# Shot List — Master Table (26 shots)

**Total runtime:** 242 seconds (~4:02)  
**Eyeline key:** CL = camera-left, CR = camera-right, H = horizon/darkness, D = down (pit)

Copy full prompts from `prompts/shot-NN.md`.

---

## Act I — Descent (0:00–0:42)

| # | Title | Dur | Camera | Dialogue | Eyeline | References |
|---|-------|-----|--------|----------|---------|------------|
| 01 | Aerial establishing | 10s | High wide, slow drift | — | — | env-shore-establishing |
| 02 | Ship & shore wide | 8s | 32mm locked wide | — | — | env-shore, odysseus-fullbody |
| 03 | Odysseus rear walk | 9s | 40mm rear follow | — | toward cavern | odysseus-rear, env-shore |
| 04 | Tracking side | 8s | 50mm lateral track | — | forward | odysseus-profile, odysseus-fullbody |
| 05 | Cavern mouth wide | 7s | 35mm low angle | — | — | env-cavern-dark, odysseus-rear |

**Act I subtotal:** 42s

---

## Act II — Ritual (0:42–1:06)

| # | Title | Dur | Camera | Dialogue | Eyeline | References |
|---|-------|-----|--------|----------|---------|------------|
| 06 | Ritual pit master | 10s | 40mm wide | — | — | env-ritual-pit, odysseus-fullbody |
| 07 | Hands pour libation | 7s | 100mm insert | — | — | env-ritual-pit |
| 08 | Odysseus over pit | 10s | 65mm medium | "Stay back… until the blood is tasted." | down to pit | odysseus-3q-right, env-ritual-pit |
| 09 | OTS — shades stir | 9s | 85mm OTS Odysseus | — | shades in H | odysseus-3q-right, env-shades-crowd |

**Act II subtotal:** 36s → cumulative 1:18

*Note: cumulative exceeds nominal act time — trim in stitch or shorten 01/06 by 1s each if you need exactly 4:00.*

---

## Act III — Tiresias arrives (1:06–1:48)

| # | Title | Dur | Camera | Dialogue | Eyeline | References |
|---|-------|-----|--------|----------|---------|------------|
| 10 | Wide — shade parting | 8s | 35mm wide | — | — | env-shades-crowd, env-cavern-dark |
| 11 | Odysseus medium — sword | 9s | 50mm | — | CR toward approaching shade | odysseus-3q-right, odysseus-fullbody |
| 12 | Tiresias emergence | 10s | 65mm slow push | — | CL toward Odysseus | tiresias-fullbody, env-cavern-dark |
| 13 | Tiresias CU — opens | 10s | 85mm locked | "Son of Laertes… you seek a way home." | CL to Odysseus | tiresias-portrait, tiresias-3q-left |
| 14 | OTS Tiresias → Odysseus | 9s | 85mm OTS | "Tell me what the gods have hidden from me." | CR to Tiresias | odysseus-3q-right, tiresias-portrait |
| 15 | Two-shot profile | 10s | 50mm side | "First you must hear what awaits you…" | CL / CR | tiresias-profile, odysseus-profile |

**Act III subtotal:** 56s → cumulative 2:14

---

## Act IV — Prophecy (1:48–3:12)

| # | Title | Dur | Camera | Dialogue | Eyeline | References |
|---|-------|-----|--------|----------|---------|------------|
| 16 | Tiresias CU — Poseidon | 10s | 85mm | "Poseidon still hunts you…" | CL | tiresias-portrait, env-cavern-dark |
| 17 | Tiresias medium — cattle | 10s | 65mm | "On Thrinacia's isle…" | CL | tiresias-3q-left, env-shades-crowd |
| 18 | Odysseus reverse CU | 8s | 85mm | "And if I keep my hands from them?" | CR | odysseus-front, odysseus-3q-right |
| 19 | Tiresias CU — suitors | 10s | 85mm | "You will reach Ithaca…" | CL | tiresias-portrait, tiresias-profile |
| 20 | Tiresias medium — oar | 12s | 65mm slow push | "You must break them. Then take an oar…" | CL | tiresias-fullbody, prop-oar |
| 21 | Tiresias CU — death | 10s | 100mm | "Plant it in the earth… gentle death from the sea." | CL | tiresias-portrait, env-cavern-dark |
| 22 | Odysseus CU — reaction | 8s | 85mm | "Is there no other path?" | CR then down | odysseus-front, odysseus-3q-left |

**Act IV subtotal:** 68s → cumulative 3:22

---

## Act V — Aftermath (3:12–4:00)

| # | Title | Dur | Camera | Dialogue | Eyeline | References |
|---|-------|-----|--------|----------|---------|------------|
| 23 | Tiresias final | 9s | 85mm | "There is only the path you make." | CL then into darkness | tiresias-portrait, env-cavern-dark |
| 24 | Odysseus reaction hold | 7s | 85mm | — | CR into dark | odysseus-front |
| 25 | Behind both — abyss | 10s | 40mm rear | — | — | odysseus-rear, tiresias-fullbody, env-cavern-dark |
| 26 | Wide shades closing | 8s | 35mm | — | — | env-shades-crowd, env-cavern-dark |

**Act V subtotal:** 34s → **Total 242s**

---

## 180° rule cheat sheet (dialogue block)

```
OTS Tiresias → Odysseus (shot 14): camera on Tiresias's side; Odysseus eyeline CR
Tiresias CU (13, 16, 17, 19, 21, 23): Tiresias eyeline CL
Odysseus CU (18, 22, 24): Odysseus eyeline CR
Profile two-shot (15): Tiresias CL, Odysseus CR — maintain in all reverse cuts
```

If a generated clip breaks eyeline, **regenerate that shot only** — do not stitch and hope.

---

## Generation order

Strictly **01 → 26**. Do not skip ahead to dialogue until ritual shots (06–09) match environment refs.

---

## Regeneration priority (if quota is tight)

**Must-have (16 shots):** 01, 03, 06, 08, 09, 12, 13, 16, 17, 19, 20, 21, 22, 23, 25, 26  
**Nice-to-have (10 shots):** 02, 04, 05, 07, 10, 11, 14, 15, 18, 24

Minimum viable stitch ≈ 2:30 with prophecy intact.
