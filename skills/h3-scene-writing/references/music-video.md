# Music video and lyric typography

Use this method for narrative, performance, beat-cut, or typography-led MVs. Typography is a designed spatial subject, not automatically a subtitle bar.

## Lock before writing

- Confirm aspect ratio, target duration, platform, music window, lyric source, performance mode, visual preset, and whether the user needs one H3 clip or a stitched work.
- Treat an uploaded song as the master audio unless the user requests replacement. If it is longer than the target, lock exact start/end timestamps first.
- User-supplied lyrics are immutable unless the user asks for rewriting. Visible words, sung words, and timestamp mapping must match exactly.
- For a finished MV without supplied lyrics, do not silently invent them. Ask for lyrics or explicit permission to create original lyrics.

## Creative contract

State the music genre, instrumentation, tempo/BPM feel, vocal mode, emotional temperature, visual language, camera density, transition logic, and exclusions. Then assign narrow reference roles:

- Character card: identity, hair, wardrobe, proportions, presence.
- Scene card: space, depth, lighting, texture, palette.
- Typography card: font texture, graphic composition, scale, placement, and motion only; it must not transfer people or scenery.
- Audio reference: song, vocal delivery, beat, or timbre.
- Video reference: camera path, cut rhythm, performance, or temporal structure.

## Timeline construction

- 10-second test: usually 1–2 shots.
- 15-second hook: usually 2–4 shots.
- More than 15 seconds: lock one continuous master audio timeline, then split into multiple H3 clips of 4–15 seconds. Inside each clip, use shorter beats when the edit needs them. Map every clip to exact master-audio timestamps.
- Put cuts on breaths, lyric gaps, snares, drops, or intentional visual accents. Avoid cutting through a sustained vowel unless mouth shape and performance continue convincingly.
- Continue the same scene with a prior tail frame as the next head frame when possible. For a hard scene change, preserve character/wardrobe/grade and use a match cut, same-direction motion, occlusion, flash, or beat impact.

## Per-shot module

For each shot record:

```text
Shot N (start–end)
Vocal or lyric line: exact text
Typography: exact visible text, placement, depth layer, entry/exit behavior
Visual and performance: space, pose, lip/jaw/breath/gesture accents
Camera and motion: shot size, move, speed, direction
Audio event: master-audio timestamp and beat/lyric cue
Transition out: visual and rhythmic handoff
```

Typography may occupy foreground, midground, or background and may pass behind a hand or shoulder, but must not cover the eyes or critical mouth shapes. Prefer one primary typography event per shot. If accurate text is fragile, reduce text frequency rather than adding more blocks.

## Preset-specific grammar

Hard cuts, scan glitches, photocopy texture, frame skips, halftone, and bass-reactive distortion belong to Dark-pop/Cyber-grunge/Trap directions; do not impose them on every MV. A soft ballad, performance film, dance MV, or narrative MV needs its own transition and camera language.

## Delivery and audit

Deliver a global aesthetic/identity lock, master timeline, per-shot H3 prompts, exact lyric/copy map, and stitching notes. Verify audio continuity, lip/lyric continuity, beat alignment, reference isolation, typography legibility, color/lighting consistency, and a clear ending state.

Source adaptation: MiniMax official `music-video-subtitle-generator` Skill.
