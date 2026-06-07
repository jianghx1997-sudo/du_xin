---
name: duxin-feedback-capture
description: Capture the author’s recurring revision feedback for the 读心 D:\AI\du_xin project. Use when the author gives chapter revision comments that may apply beyond the current chapter, says 后续注意, 以后都要, 长期记住, or points out repeated prose, logic, workflow, character-boundary, mind-reading, or review-gate problems.
---

# 读心长期反馈沉淀

## 目标

把作者对当前章的反馈分成“只改当前章”和“以后都要遵守”，防止长期问题反复出现。

## 流程

1. 先按作者意见修改当前正文。
2. 逐条判断反馈类型：
   - 本章局部：只改正文。
   - 本案持续：作者确认后更新当前案 `outline.md` 或 `session-handoff.md`。
   - 全书硬规则：更新 `_series-rules.md` 或 `_cross-case-tracker.md`。
   - 长期语言风格：更新 `_writing-style-guide.md` 第十节；需要审查门禁时同步更新 `_editor-review.md`。
   - 协作流程：更新 `_workflow.md`。
   - 技能入口：更新 `.agents/skills/` 下最相关的 `SKILL.md`。
3. 新规则只写到最直接生效的位置，能并入既有条目的不新增长段。
4. 最终回复作者时，说明哪些反馈已沉淀为长期规则。

## 判断标准

作者用了“以后”“后续”“每次”“一直”“不要再”等表达，或同类问题连续出现两次以上，默认按长期反馈处理。

不要把单章临时剧情意见写成全书规则。
