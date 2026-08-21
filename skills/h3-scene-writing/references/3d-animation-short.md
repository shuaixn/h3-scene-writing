# Story-first stylized 3D animation short

Use for a multi-shot narrative animation where story causality, character performance, spatial continuity, and audio need production-level planning. Do not force the original Skill's Pixar-like default when the user supplies another style.

## Story and design locks

Record the premise, emotional promise, audience feeling, total duration, ratio, dialogue mode/language, and visual style. Build an active protagonist with a want, need, and flaw; define the world rule and an eight-beat causal spine. The protagonist's flaw should intensify the crisis, coincidence must not solve it, and the payoff should reuse an earlier emotional anchor.

Create identity notes for each character: name, role, silhouette, proportions, face/hair, costume colors, signature props, expression range, and do-not-change traits. Create environment-only scene anchors with named landmarks, key/fill/rim direction, emotional subspaces, and prop positions. Do not contaminate scene references with characters.

## Six-column shot table

Use exactly these planning columns when the user needs a full production package:

1. Shot ID and duration.
2. Continuity handoff from the prior state and into the next state.
3. Spatial and identity anchors.
4. Hook type.
5. Shot description with per-second directives.
6. Audio and dialogue track.

Spatial anchors name fixed landmarks with screen-relative positions; every character's screen position, facing, depth, pose, and prop state; recently exited characters; inherited lighting; exact character/scene reference IDs.

Every per-second directive includes five elements: action/pose/expression, camera, spatial position, audio cue or intentional silence, and the state handed to the next second/shot. Use sub-second beats only for critical actions. Track anticipation, squash/stretch, overshoot, overlap, follow-through, eye-line, and mouth-open/mouth-closed state where performance requires them.

## Continuity and hook audit

- No H3 clip exceeds 15 seconds.
- No shot carries more than three important acting/speaking characters unless explicitly justified.
- Each shot has a hook such as setup, visual joke, reversal, reveal, callback, suspense, tender beat, chase, expression beat, or climax.
- Across repeated locations, landmarks and lighting either remain consistent or their movement/change is explicitly caused by the camera or story.
- Per-second directives cover the full duration without gaps.
- Eyeline, character position, prop state, costume, and lighting changes are inherited or explicitly marked as a cut/time jump.

## Text storyboard

For each shot, record title/duration, hook, scene/characters, spatial anchor card, continuity from/to adjacent shots, and one beat block per second. Each beat block specifies pose/expression, camera, audio, anchor, and handoff. A simple ASCII layout may help human review but is never model-facing content.

For final generation prompts, strip planning labels, table syntax, arrows, panel borders, storyboard notes, and reference-debug markers. Convert the approved beat blocks into the official H3 shot schema and keep one continuous master audio plan across assembled clips.

Source adaptation: MiniMax official `3d-animation-short-generator` Skill and its shot-table/storyboard references.
