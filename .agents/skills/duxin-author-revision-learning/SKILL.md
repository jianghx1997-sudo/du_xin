---
name: duxin-author-revision-learning
description: Learn from the author’s latest Obsidian-synced revisions in the 读心 D:\AI\du_xin project. Use when the user says 改好了, 已修改, Obsidian 同步了, or asks to continue after manually editing a chapter, so Codex rereads the newest local manuscript, infers what the author changed and why, and carries those constraints into the next chapter without relying on stale context.
---

# 读心作者改稿学习

## 目标

用户说“改好了”后，先学习作者最新本地稿，再继续写下一章。

## 读取流程

1. 定位项目根目录，优先当前 `D:\AI\du_xin`。
2. 读取 `case-files/session-handoff.md` 判断最后章节。
3. 列当前案目录，确认最新正文文件名。
4. 读取作者最新本地正文原文。
5. 如可用，查看该文件的 `git diff`，只用于理解改动，不回滚。
6. 必要时读取前 1 到 2 章，判断节奏和承接。

## 判断要点

用极短要点在思考中归纳：

- 作者删掉了什么，以及可能为什么删。
- 作者加强了什么，包括情绪、节奏、细节、对话、线索等级。
- 是否改变章节功能、人物判断时机或案件事实。
- 下一章不能提前揭示、提前拔高、重复强调什么。

如果用户只是让继续写，不必把这份分析完整发给用户，直接带入 `duxin-chapter-writing`。

## 边界

- 不把作者改动写入 `session-handoff.md`。
- 不覆盖作者稿。
- 不用旧上下文替代最新本地文件。
- 只在作者确认章节后，才交给 `duxin-archive-update` 更新接力或案纲。
