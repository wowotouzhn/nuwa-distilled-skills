# Codex repository guidance

This repository contains task-specific Codex Skills in `.agents/skills/` for three domains, including a modular Xiaohongshu workflow. Use them for relevant user requests, including requests written in Chinese. The metadata alone is not the full instruction set.

## Skill routing

- **Xiaohongshu / 小红书**: Default to `.agents/skills/space-xhs-buddy/SKILL.md` for multi-step tasks; use specialized `.agents/skills/space-xhs-positioning/`, `space-xhs-hotspot/`, `space-xhs-writer/`, `space-xhs-title/`, `space-xhs-cover/`, `xhs-html/`, `space-xhs-image/`, `space-xhs-account-audit/`, and `space-xhs-note-analytics/` for focused tasks. Read the actual `SKILL.md` of each selected module before work. Do not claim real-time Xiaohongshu data without an available verified source; external APIs, browser access, image generation, and rendering tools may be unavailable.
- **WeChat Channels / 微信视频号**: For 视频号 positioning, launch, videos, livestreams, growth, WeChat ecosystem and private-domain conversion, read `.agents/skills/wechat-channels-ops-framework/SKILL.md` and its linked methodology at `wechat-channels-ops-framework/SKILL.md`.
- **English learning / 英语学习**: For lessons, grammar, listening, speaking, reading, writing, vocabulary, correction, study plans or error review, read `.agents/skills/english-learning-coach/SKILL.md` and `.agents/skills/english-learning-coach/ORIGINAL_SKILL.md`. For study planning or training-method selection, also consult `.agents/skills/english-learning-coach/references/programmers-guide-methods.md` (an attributed adaptation of an external guide, not another Skill).

## Execution rules

1. When a request clearly falls into one of the categories above, **read the corresponding Skill file before producing substantive advice or teaching**. Do not rely only on the Skill's name or description.
2. Read linked methodology and relevant `references/` as needed. If more than one category applies, use each relevant Skill.
3. Do not claim to have read or invoked a Skill unless its files were actually read. If unavailable, explain the limitation and answer without falsely attributing the result to the Skill.
4. Do not install, copy, or modify Skills merely to answer a normal user question. Keep the user's original task as the priority.
5. Distinguish verified platform rules and measured results from hypotheses or historical anecdotes. Do not guarantee views, followers, revenue, or learning outcomes.
6. Reply primarily in Chinese unless the user requests otherwise. Follow explicit user instructions that override these defaults.

These instructions improve task routing within this repository; they do not guarantee that every Codex environment automatically loads repository guidance.
