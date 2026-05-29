# hirotaka-nifuji-skill

A Codex skill for roleplaying Hirotaka Nifuji from *Wotakoi: Love Is Hard for Otaku* with a calm, deadpan, low-drama conversational style.

This repository packages the skill as a standalone folder suitable for publishing, versioning, and installing into a local Codex skills directory.

## What This Skill Does

- roleplays Hirotaka Nifuji in Chinese or English
- keeps his tone restrained, practical, and quietly affectionate
- uses series context from *Wotakoi* to keep relationship dynamics coherent
- uses public quote anchors as flavor guidance without relying on full scripts or subtitle dumps
- includes playtest notes and drift-control guidance for longer chats

## Files

- `SKILL.md`: main skill instructions and invocation rules
- `agents/openai.yaml`: UI metadata for the skill
- `references/persona.md`: stable character core
- `references/voice.md`: base dialogue guidance
- `references/chinese-voice.md`: Chinese tone adaptation
- `references/series-context.md`: plot and relationship context
- `references/quote-bank.md`: compact canon-flavored anchors
- `references/quotes.md`: broader public quote library and paraphrase seeds
- `references/drift-control.md`: anti-drift guardrails
- `references/chat-samples.md`: multi-turn conversation examples
- `references/playtest.md`: current playtest report

## Install

Copy this folder into your local Codex skills directory:

```powershell
Copy-Item -Recurse -Force .\hirotaka-nifuji-skill "$HOME\\.codex\\skills\\hirotaka-nifuji"
```

Or clone directly into the skills directory:

```powershell
git clone https://github.com/kanemaverick/hirotaka-nifuji-skill.git "$HOME\\.codex\\skills\\hirotaka-nifuji"
```

## Example Prompts

- `Use $hirotaka-nifuji to roleplay a calm late-night chat.`
- `用二藤宏嵩的语气陪我聊天。`
- `帮我写一段宏嵩和成海约会后的对话。`
- `分析一下宏嵩为什么看起来冷淡但其实很可靠。`

## Design Notes

This skill is built from:

- official public-facing character descriptions
- public quote roundup pages
- public story summaries and commentary
- original paraphrase and dialogue-structure rules

It is not a full script archive or subtitle mirror.

## Limitations

- It does not contain a complete official transcript.
- Some quote anchors come from public roundup pages rather than primary scripts.
- The intended result is a convincing conversational persona, not strict scene-by-scene canon reproduction.

## License

This repository is licensed under the MIT License for the skill structure and original prompt/reference material in this repo.

Character and series rights remain with their original copyright holders.
