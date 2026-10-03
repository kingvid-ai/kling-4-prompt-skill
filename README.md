# Kling 4.0 Prompt Skill

An agent skill for writing and improving Kling video prompts: text-to-video, image-to-video, camera movement, references, dialogue, and multi-shot plans.

[Read the full prompt guide](https://kingvid.app/posts/kling-4-0-prompt-guide) · [Browse the visual examples](https://kingvid.app/kling-4-prompt) · [Awesome Kling prompts](https://github.com/kingvid-ai/awesome-kling-4-prompts)

## Install

With the Skills CLI:

```bash
npx skills add kingvid-ai/kling-4-prompt-skill --skill kling-4-prompt
```

Or install directly for Codex:

```bash
git clone https://github.com/kingvid-ai/kling-4-prompt-skill.git ~/.codex/skills/kling-4-prompt
```

For Claude Code, clone into `~/.claude/skills/kling-4-prompt` instead. If that folder already exists, update the existing installation rather than overwriting it. Restart your agent session if the new skill is not discovered.

## Use

```text
Use $kling-4-prompt to write a 10-second perfume ad with a slow camera push-in.
```

```text
Use $kling-4-prompt to animate this portrait with a subtle turn and a fixed camera.
```

```text
Use $kling-4-prompt to fix this prompt: the mug keeps changing shape and the camera moves too much.
```

The skill returns a copyable prompt and any important assumptions or suggested settings. It does not execute generation, require an API key, or require a KingVid account. Refer to the chosen model's interface for available duration, audio, reference, and keyframe controls.

## Files

- [SKILL.md](SKILL.md): workflow, output guidance, source links, and version boundaries.
- [references/examples.md](references/examples.md): original teaching prompts and troubleshooting suggestions.
- [agents/openai.yaml](agents/openai.yaml): Codex display metadata.

Maintained by [KingVid](https://kingvid.app). Independent of Kling AI; examples are teaching prompts, not verified model outputs. Source material reviewed October 3, 2026. MIT licensed.
