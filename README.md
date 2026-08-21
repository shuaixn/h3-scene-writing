# MiniMax H3 Scene Writing Skill

English | [简体中文](#简体中文)

An unofficial, portable companion Skill for writing MiniMax H3 prompts in eight scene-specific video formats. It adapts the prompt-writing and pre-production methods from MiniMax's official Hub-oriented Skills for use in Codex, Hermes Agent, and other agents that support `SKILL.md`.

This repository is prompt-only. It contains no model weights, API keys, generation scripts, telemetry, or automatic calls to MiniMax Hub.

## Supported formats

1. Music videos and lyric typography
2. Minimalist premium product ads
3. Brand, product, app, and website promos
4. Story-first stylized 3D animated shorts
5. Papercraft stop-motion explainers
6. Editorial paper-collage explainers
7. Two-player co-op game intros
8. Glowing hand-drawn/live-action fusion clips

POV is not a separate format in this Skill. Use the official general `h3-prompt-writing` Skill for POV and other general H3 camera language.

## How it works

`h3-scene-writing` selects the scene-specific construction method: story spine, beat structure, reference roles, continuity, camera, typography, audio, and quality checks.

The official `h3-prompt-writing` Skill remains responsible for the final H3 model-facing schema, including Base and Ref2VA reference syntax. For best results, install and use both Skills.

## Install

### Codex and agents supported by `npx skills`

```bash
npx skills add https://github.com/shuaixn/h3-scene-writing --skill h3-scene-writing
npx skills add https://github.com/MiniMax-AI/MiniMax-H3 --skill h3-prompt-writing
```

### Hermes Agent

```bash
hermes skills install shuaixn/h3-scene-writing/skills/h3-scene-writing --category creative --yes
hermes skills install MiniMax-AI/MiniMax-H3/skills/h3-prompt-writing --category creative --yes
```

Installed Skills normally take effect in a new agent session.

### Manual installation

Copy the complete [`skills/h3-scene-writing`](skills/h3-scene-writing) directory into your agent's Skill directory. Keep `SKILL.md`, `agents/`, and `references/` together.

## Usage examples

```text
Use $h3-scene-writing and $h3-prompt-writing to write a 15-second performance MV prompt. Lock the supplied lyrics and place cuts on breaths and snare hits.
```

```text
Use $h3-scene-writing and $h3-prompt-writing to turn this product photo into a 10-second minimalist launch film with one hero action and a stable copy closing.
```

```text
Use $h3-scene-writing to build a multi-shot 3D animation plan, then package each clip with $h3-prompt-writing.
```

## Repository layout

```text
skills/h3-scene-writing/
├── SKILL.md
├── agents/openai.yaml
└── references/
    ├── music-video.md
    ├── minimalist-product-ad.md
    ├── brand-promo.md
    ├── 3d-animation-short.md
    ├── papercraft-explainer.md
    ├── paper-collage-explainer.md
    ├── co-op-game-intro.md
    ├── handdrawn-live-fusion.md
    └── sources.md
```

## Portability and safety

The official specialized Skills were designed for MiniMax Hub and assumed Hub canvas, generation, audio, editing, routing, and choice-card tools. This adaptation removes those execution instructions and retains only portable writing and pre-production guidance. It does not generate video or contact external services by itself.

## Attribution and license

This is an unofficial community adaptation and is not endorsed by MiniMax. The source methods come from the official [MiniMax H3 repository](https://github.com/MiniMax-AI/MiniMax-H3). See [`sources.md`](skills/h3-scene-writing/references/sources.md) for the audited revision and source mapping.

The adapted files are distributed subject to the [MiniMax H3 Community License Agreement](LICENSE) and the required [`NOTICE`](NOTICE). Review the upstream agreement, including its territorial and acceptable-use restrictions, before using or redistributing this repository. This summary is not legal advice.

---

## 简体中文

这是一个非官方、可移植的 MiniMax H3 场景写作 Skill。它把 MiniMax 官方面向 Hub 的八种专项视频工作流中的提示词写法与前期设计方法，整理成可供 Codex、Hermes Agent 及其他支持 `SKILL.md` 的 Agent 使用的版本。

本仓库只提供提示词与前期方案，不包含模型权重、API Key、生成脚本、遥测，也不会自动调用 MiniMax Hub。

### 支持的八种类型

1. MV 与歌词文字包装
2. 极简高质感产品广告
3. 品牌、产品、应用和网站宣传片
4. 故事驱动的风格化 3D 动画短片
5. 纸艺定格科普
6. 编辑感纸张拼贴解说
7. 双人合作游戏开场
8. 手绘发光动画与实拍融合

POV 不属于这八种专项类型。普通 POV、运镜以及 H3 最终字段结构仍由官方 `h3-prompt-writing` Skill 处理。

### 工作方式

`h3-scene-writing` 负责场景类型的创作方法：故事结构、节拍、素材职责、镜头连续性、运镜、文字、声音和质量检查。

官方 `h3-prompt-writing` 负责最终提交给 H3 的标准格式，包括 Base 与 Ref2VA 的引用语法。建议两个 Skill 一起安装和调用。

### 安装

Codex 或支持 `npx skills` 的 Agent：

```bash
npx skills add https://github.com/shuaixn/h3-scene-writing --skill h3-scene-writing
npx skills add https://github.com/MiniMax-AI/MiniMax-H3 --skill h3-prompt-writing
```

Hermes Agent：

```bash
hermes skills install shuaixn/h3-scene-writing/skills/h3-scene-writing --category creative --yes
hermes skills install MiniMax-AI/MiniMax-H3/skills/h3-prompt-writing --category creative --yes
```

安装后通常需要新开 Agent 会话才能生效。

### 使用示例

```text
使用 $h3-scene-writing 和 $h3-prompt-writing 写一个15秒表演型MV提示词，锁定现有歌词，在换气和军鼓点切镜。
```

```text
使用 $h3-scene-writing 和 $h3-prompt-writing，把这张产品图设计成10秒极简新品发布片，只有一个主动作，并以稳定的产品加文案画面收尾。
```

### 来源与许可

这是社区维护的非官方适配版，与 MiniMax 没有隶属或背书关系。方法来源于 [MiniMax H3 官方仓库](https://github.com/MiniMax-AI/MiniMax-H3)，具体来源映射与审计版本见 [`sources.md`](skills/h3-scene-writing/references/sources.md)。

本仓库中的适配文件受 [MiniMax H3 Community License Agreement](LICENSE) 和 [`NOTICE`](NOTICE) 约束。使用或再分发前，请阅读完整协议，尤其是地域限制与可接受使用政策。本说明不构成法律建议。
