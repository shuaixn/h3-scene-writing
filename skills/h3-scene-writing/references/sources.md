# Source provenance and portability audit

This companion was derived from the official MiniMax H3 repository at:

- Repository: `https://github.com/MiniMax-AI/MiniMax-H3`
- Audited revision: `d21241f0a4b3acbb34c97dae47fa417b7065e438`
- Audit date: 2026-08-21

Upstream source mapping:

| Portable reference | Official source Skill |
|---|---|
| `music-video.md` | `music-video-subtitle-generator` |
| `minimalist-product-ad.md` | `minimalist-product-ad-generator` |
| `brand-promo.md` | `brand-promo-video-generator` |
| `3d-animation-short.md` | `3d-animation-short-generator` plus shot-table/storyboard references |
| `papercraft-explainer.md` | `papercraft-stop-motion-explainer` |
| `paper-collage-explainer.md` | `paper-collage-explainer-generator` |
| `co-op-game-intro.md` | `co-op-game-intro-generator` plus H3 video template |
| `handdrawn-live-fusion.md` | `handdrawn-live-video-generator` |

Audit findings:

- The eight official specialized directories contained Markdown and YAML only; no executable scripts or package dependencies were required by the files.
- They contained no credential readers or telemetry code.
- Their main portability risk was procedural: the original Skills assume MiniMax Hub canvas, media-generation, audio, editing, choice-card, routing, and source-fetch tools. Those operations can create network, privacy, publication-rights, and generation-cost effects.
- This companion removes all Hub execution promises and retains only scene planning, prompt writing, reference-role design, continuity, audio, typography, and quality-control methods.
- The official `h3-prompt-writing` Skill remains the authority for model-facing H3 field structure and reference syntax. This companion does not replace or modify it.

Maintenance rule: compare a future upstream revision by meaning, not by copying whole files. Import only changes that improve portable writing decisions. Do not reintroduce Hub tool calls, automatic generation, external writes, or cost-bearing actions.
