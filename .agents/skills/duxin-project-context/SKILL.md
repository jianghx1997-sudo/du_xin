---
name: duxin-project-context
description: Read and summarize the 读心 project startup context. Use when starting, resuming, or orienting work in the D:\AI\du_xin novel project, especially when the user says to continue 读心, asks what the current progress is, starts a new conversation, or needs the current case, chapter, handoff, rules, or project document state restored before writing or editing.
---

# 读心项目启动上下文

## 目标

把 Codex 带回《读心》项目的当前工作状态。只读取和汇总，不写正文，不更新文档。

## 项目根目录

按顺序定位项目根目录：

1. 当前工作目录或其父目录中存在 `AGENTS.md`，且内容为《读心》项目入口。
2. `D:\AI\du_xin` 可访问。
3. 找不到时，向用户询问项目路径。

所有路径都使用绝对路径。

## 固定读取顺序

1. `AGENTS.md`
2. `_series-rules.md`
3. `case-files/session-handoff.md`
4. 如果接力文档指向当前案，读取当前案 `outline.md`

如用户准备写正文，再交给 `duxin-chapter-writing` 的流程，不在本 Skill 中补读最近章节。

## 输出

用很短的中文要点说明：

- 当前案件和阶段。
- 最后一章、本章确认状态、下一章方向。
- 本轮最重要红线。
- 是否有待作者确认或 Obsidian 改稿需要重读。

不要复述全部规则，不要展开案情长摘要。
