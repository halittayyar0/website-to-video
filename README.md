# Website to Video

Turn a website address into a scene designed for that particular business: two consistent START/END frames (or copyable image prompts), a complete video prompt, and a web-use handoff.

**Give it a URL. The agent does the creative work.** It researches the site, understands the offering and visual identity, then chooses a suitable scene, action, style, camera, pacing and composition. You can specify any of those choices, but a creative brief is optional. There is no universal product rotation, hand interaction, garment shot, duration or aspect preset.

```text
$website-to-video kutarel.com
```

Addresses work with or without `https://`. Product/detail URLs stay the focus. The agent may ask once whether you want generated images or prompts only; an existing choice is preserved. That delivery preference is separate from creative direction.

## What it delivers

- A source-grounded explanation of the chosen scene and its place on the website.
- Exactly two endpoint images or complete English image prompts for a feasible, resolved shot.
- A complete English video prompt directly in the final chat response as one copyable text code block, including action, intermediate phases, camera, timing and continuity constraints. A download link does not replace it.
- Crop, poster, accessibility and playback recommendations, with unverified items identified.

The source is researched before the scene is chosen. For an ordinary motion request, merely zooming or cropping a static product photograph is insufficient. Proposed editorial staging is labeled and does not invent product features or claim to be real footage. Explicit camera-only, ambient and loop briefs remain valid. START is reviewed against source before END is generated with that actual START as reference. Failed outputs are rejected and repairs are bounded.

A video file is **not** automatically rendered. Two stills do not prove intermediate motion, mobile playback or a seamless loop. This skill does not buy services, deploy a website, publish content or contact anyone as part of ordinary use. No additional API key or paid fallback is required; available host tools and limits apply.

## Install

The shared skill is in `skills/website-to-video/`.

- **Codex:** copy that folder into your user skills directory (commonly `~/.codex/skills/website-to-video`), then invoke `$website-to-video example.com` in a session that discovers it.
- **ChatGPT/Codex plugin packaging:** [OpenAI plugin ZIP](https://github.com/halittayyar0/website-to-video/raw/refs/heads/main/packages/website-to-video-openai-plugin.zip). This is a skills-only package; native installation depends on the host/account. Uploading `SKILL.md` as a normal chat attachment is not native installation.
- **Claude:** [skill ZIP](https://github.com/halittayyar0/website-to-video/raw/refs/heads/main/packages/website-to-video-claude.zip). This workflow uses prompts-only there. Actual execution of this package in Claude has not been verified.

A skill is the workflow instruction. A plugin is a distribution package containing that skill. The core is shared; host installation methods differ.

## Version and evidence

Current version: **0.2.6**. Creative ownership is explicit: an unspecified brief delegates creative decisions to the agent after research. Prior motion and source-fidelity checks remain acceptance criteria, not an aesthetic template.

[TEST-REPORT.md](TEST-REPORT.md) separates current bounded behavioral checks, historical live source/image work, failed attempts, and unverified platforms/video execution. Existing examples are test artifacts, not mandatory shot recipes. Third-party brands are independent examples without endorsement; source links are not blanket media licenses.

Public source availability does not imply approval for unrelated account, spending, publishing or messaging actions. The existing hosted plugin has its own account-scoped distribution and is separate from GitHub repository visibility.
