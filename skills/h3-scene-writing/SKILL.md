---
name: h3-scene-writing
license: MiniMax H3 Community License Agreement
description: >-
  Write, adapt, or audit MiniMax H3 prompts and pre-production plans for eight
  official specialized video formats: music videos with lyric typography,
  minimalist product ads, brand promos, stylized 3D animated shorts,
  papercraft explainers, editorial paper-collage explainers, co-op game intros,
  and hand-drawn/live-action fusion clips. Use when the user names one of these
  formats or asks for its scene-specific method. Do not use for a generic H3
  prompt with no specialized format, ordinary subtitle cleanup, or automatic
  video generation.
---

# MiniMax H3 Scene Writing

This is a portable, prompt-only companion to the official `h3-prompt-writing` Skill. It extracts the writing and pre-production methods from MiniMax's eight Hub-specific Skills without carrying over Hub canvas, generation, editing, routing, or API calls.

## Route the request

Read only the reference that matches the requested format:

| Request | Required reference |
|---|---|
| MV, music video, lyric typography, 卡点MV, 贴字MV | [references/music-video.md](references/music-video.md) |
| Apple-like, premium, minimalist physical-product ad | [references/minimalist-product-ad.md](references/minimalist-product-ad.md) |
| Brand/product/app/website launch promo | [references/brand-promo.md](references/brand-promo.md) |
| Story-first stylized 3D animated short | [references/3d-animation-short.md](references/3d-animation-short.md) |
| Papercraft, pop-up-book, layered diorama explainer | [references/papercraft-explainer.md](references/papercraft-explainer.md) |
| Editorial halftone paper-collage explainer or B-roll | [references/paper-collage-explainer.md](references/paper-collage-explainer.md) |
| Two-player co-op game menu/opening | [references/co-op-game-intro.md](references/co-op-game-intro.md) |
| Glowing hand-drawn animation fused with live action | [references/handdrawn-live-fusion.md](references/handdrawn-live-fusion.md) |

POV is camera/viewpoint language in the general H3 guide, not one of these eight specialized formats. For a POV request without one of the formats above, use `h3-prompt-writing` directly.

## Shared workflow

1. Preserve the user's supplied references, identities, lyrics, copy, product facts, duration, aspect ratio, language, and delivery scope. Ask only for missing information that changes the structure.
2. Apply the selected format reference to decide the story spine, beat structure, reference roles, continuity locks, camera logic, typography/audio rules, and quality checks.
3. When the user wants a model-facing H3 prompt, also apply `h3-prompt-writing` and its relevant Base or Ref2VA guide. The format reference decides creative construction; `h3-prompt-writing` decides the final H3 schema and reference syntax.
4. H3 generates 4–15 seconds per clip. If the intended work exceeds 15 seconds, write a master timeline plus multiple 4–15 second shot prompts and explicit assembly/continuity notes. Never describe a longer work as one native H3 generation.
5. Keep exact visible copy, usernames, dialogue, and lyrics verbatim. Do not invent missing brand claims, metrics, logos, lyrics, or identity-bearing assets unless the user explicitly asks for concept material.
6. Default deliverable is the requested prompt or pre-production package. Do not call generation, canvas, audio, editing, browser, or external services merely because an upstream Hub Skill did so.

## H3 integration rules

- Choose Base T2VA/I2VA/FL2VA/L2VA when the task is controlled by text and optional first/last frames. Choose Ref2VA when images, videos, or audio have distinct reusable roles.
- Give each reference one narrow job: identity, environment, typography, product appearance, camera/edit rhythm, or audio. State both what transfers and what must not transfer.
- Within every shot, describe composition, subject state, environment, ordered action, camera motion, and synchronized sound. Use timestamped cuts only when the scene, viewpoint, subject state, or time materially changes.
- Put physical and ambient sound in `overall_soundscape`. Put audience-only score in `non_diegetic_music`. Keep dialogue, singing, diegetic music, and lyric timing inside the shot description according to the official guide.
- For long-form packages, make the master audio, global aesthetic lock, reference IDs, and continuity chain authoritative across all clip prompts.

## Portability and maintenance

The source Skills were designed for MiniMax Hub and are not directly portable. This companion never assumes Hub tools exist. For provenance, upstream names, and the audited revision, see [references/sources.md](references/sources.md); read it only when maintaining or verifying this Skill.
