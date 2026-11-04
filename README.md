# 女娲 · Codex Skills 工作区

本仓库为 Codex 提供三个领域的 Skills。项目级 Skills 位于 `.agents/skills/`，具体路由见 [AGENTS.md](AGENTS.md)。

## 小红书：Creator Buddy（新版，已替换旧版）

基于 [SpaceZephyr/creator-buddy](https://github.com/SpaceZephyr/creator-buddy) 的小红书模块，包含 10 个专项 Skill：

- `space-xhs-buddy`：总控与工作流编排
- `space-xhs-positioning`：零粉起号与账号定位
- `space-xhs-hotspot`：热点研究与选题（真实数据通常需要 API）
- `space-xhs-title`：标题
- `space-xhs-writer`：笔记正文
- `space-xhs-cover`：封面
- `space-xhs-image`：AI 信息图
- `xhs-html`：多页图文排版
- `space-xhs-account-audit`：账号体检
- `space-xhs-note-analytics`：笔记数据复盘

原 `xiaohongshu-ops-framework` 已从当前分支移除，避免与新版重复触发；需要回溯可查看 Git 历史。上游来源和使用限制见 [CREATOR_BUDDY_SOURCE.md](CREATOR_BUDDY_SOURCE.md)。

## 视频号

`wechat-channels-ops-framework`：微信视频号定位、内容、增长、直播和转化。保留原始方法论于 `wechat-channels-ops-framework/SKILL.md`。

## 英语学习

`english-learning-coach`：日常英语学习、语法、听说读写、纠错与复习。附有 A Programmer's Guide to English 的注明来源的学习方法参考文档。

## 使用说明

在以本仓库为工作区的 Codex 中提出任务；为提高确定性，可以明确指定 `$space-xhs-buddy` 或对应专项 Skill。仓库文件存在不等于已验证自动触发。

部分小红书模块依赖外部 API、图像生成或 HTML 渲染环境；未配置时应说明限制，不得编造实时平台数据或声称已完成图片渲染。
