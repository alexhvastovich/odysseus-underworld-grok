---
name: Grok Imagine Agent
description: >-
  Use when driving Grok Imagine Agent Mode on grok.com/imagine (project +
  infinite canvas) for a multi-shot film. Log every still/video ID from the
  first generate. Last frame of N is first of N+1. Ask Agent to trim and stitch
  joins. Spoken video goes through Agent chat with the still attached. Not
  Studio. Not x.com SuperGrok chat.
---
# Grok Imagine Agent

Drive **Imagine Agent Mode** at `https://grok.com/imagine`. URLs look like `/imagine/agent/<id>` — do not publish private IDs. Three panes: **sidebar** (projects / history), **agent chat** (Type to imagine), **infinite canvas** (dot grid + tools). Different from Studio (`/imagine/studio`) and SuperGrok chat on `x.com/i/grok`.

This is the **web** app in Chrome on this computer. Not a desktop app. Not the user's laptop.

Official Odyssey craft: [Odyssey Challenge Cinematic Guide](https://x.com/imagine/status/2092675531057885288) (2026-08-26). Contest deadline August 31. Do not contest-submit without a human yes.

## ID ledger (from the first generate)

Every still and every video gets a canvas **id** the moment it exists. If you skip this, later edits guess thumbnails and joins break.

1. The instant a still or video node appears, write a row: shot number, still UUID, video UUID, take letter, KEEP/CHANGE/DELETE.
2. The ledger lives with the film (`CANVAS-MAP.md` or equivalent). Update it **before** the next generate.
3. Click by **id**, never by a guessed thumbnail.
4. A new take gets a new video id. Do not overwrite the old row — add `take-b` and keep take-a.
5. Do not invent ids. Truncated ids stay marked INCOMPLETE. Missing ids stay NEED ID.
6. Never publish `/imagine/agent/<id>` or conversation query strings. Node UUIDs for shots are the working ids.

No generate without a ledger row.

## Map the canvas, then edit cut by cut

1. **Zoom out** until every shot node is visible (25–50%).
2. **Map** node id → boarded shot. Write the map before you edit.
3. Edit **only CHANGE** shots. Leave KEEP nodes alone.
4. **One cut at a time.** Click that still id. Then left Agent chat with that still selected/attached.
5. Still first (Speed → Quality upscale, pores/lines). Spoken video only after the still PASSes, via Agent chat + still. Node one-click Make Video skips the line.
6. Download the new node. Write its new video id. Never overwrite `*_LOCK` or keeper clips.

## Last frame is first frame (do not skip)

Same camera / same location: the **last frame of shot N is the first frame of shot N+1**.

- Extract last frame (or use Agent "Extract Frame" at the end).
- That image **is** the start of the next still/video. Prompt: start on this exact frame, then play the new beat.
- New lock still only when camera angle or location actually changes.
- If start/end do not match, the join will slam. That is a skill miss, not a stitch trick.

## Ask Agent to trim and stitch

Imagine Agent **can trim and stitch**. Ask it. Do not hard-concat locally as the first answer.

Name the join, the two **video ids**, and the transition:

- Same location: last-frame match, or a short dissolve. "Start shot N+1 on the last frame of video `<id>`."
- Location change: a real cut or a named fade (e.g. 0.6s cave-mouth → ritual).
- Line ends → shades: trim the tail of the spoken take, then **emerge from shadow** into the next still — not a slam to OTS.
- Never close→wide on the same face. Hold size or cut away.
- Composer submits on every newline: stitch asks are **one line**.

Example one-liner: `Stitch video <id-A> then video <id-B> start B on the last frame of A trim the tail of A so the join is continuous same cave no slam`

ffmpeg pairwise xfade is a **fallback** after Agent stitch is refused or Picture FAILs the Agent join. It is not the default.

## Official still → video

Do not write “cinematic” and stop. Name **shot size, angle, move, lens**.

1. Aim.
2. Speed Mode still.
3. Quality Mode upscale (pores, fine lines).
4. Animate with omni-reference.
5. Prompt like a director: shot / doing / speech / remember. **No music.**

## Two video paths (do not mix)

### Spoken — Agent chat
Attach the selected canvas still. 1080p, 6/10/15s, Audio ON. Exact line. No extra words. Never into lens. NO MUSIC.

### Silent — canvas tap on that node is fine
Audio OFF. One job.

## While it runs

- Stay on the live agent tab. One Chrome. One job.
- Download when the node is done. Size >1MB. Log the new id.

## Do not

- Use Studio if Agent + canvas is live.
- Hard-concat or local xfade before asking Agent to trim/stitch.
- Skip last-frame handoff on a same-location join.
- Generate without writing the still/video id.
- Fire a second generate while one is Generating.
- Publish private `/imagine/agent/<id>` or conversation IDs.
- Invent scenes. Human pass locks keepers.
- Contest-submit without a human yes.
