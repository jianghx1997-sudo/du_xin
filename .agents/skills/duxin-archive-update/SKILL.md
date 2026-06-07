---
name: duxin-archive-update
description: Update handoff, outline, and tracking documents after the author confirms a 读心 chapter or case stage. Use only when the user explicitly confirms a chapter is accepted, says 可以归档, 确认这章, 更新接力文档, 更新案纲, or asks to archive completed 读心 work after revision and editor review are finished.
---

# 读心确认归档

## 触发边界

只有作者明确确认章节或阶段后才能更新文档。草稿、待确认稿、编辑审查中稿，不归档。

## 必读

1. `case-files/session-handoff.md`
2. 当前案 `outline.md`
3. 已确认章节正文
4. `_workflow.md`

按需读取：

- `_cross-case-tracker.md`：能力、道具、伏笔、破局方式、感情线变化。
- `_series-outline.md`：案件阶段、当前状态变化。
- `_characters.md`：长期人物状态变化。

## 更新范围

固定更新：

- `case-files/session-handoff.md`：最后本地章节、确认状态、下一章方向、本轮工作状态。

必要时更新：

- 当前案 `outline.md`：新增案件事实、人物状态、证据链、未解决隐患、后续可回收点。
- `_series-outline.md`：案件阶段或全书状态变化。
- `_cross-case-tracker.md`：能力、道具、伏笔、破局方式、可回归角色、感情线变化。
- `_characters.md`：长期人物状态或关系阶段变化。

## 写法

- `session-handoff.md` 保持短，只记录最新进度和下一步。
- 不把正文摘要大段塞进全局文档。
- 不重复记录已由正文完整承载、后续不复用的细节。
- 使用 `apply_patch` 做手动编辑。
- 不重命名、不移动、不删除正文文件。
