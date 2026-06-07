# 读心（duxin）项目入口

## 项目定位

现代女频长篇单元刑侦文。

主线：时菱靠读心能力和心理学、微表情、行为分析包装，从江城市局特邀顾问逐步成长为全国级神探。

副线：原生家庭打脸 + 豪门感情线。

全书三阶段：江城立足期 → 名声外传期 → 全国封神期。

## 启动读取顺序

新会话或新任务开始时，按顺序读取：

1. 本文件：项目入口和文档索引。
2. [_series-rules.md](_series-rules.md)：全书硬规则和写作红线。
3. [case-files/session-handoff.md](case-files/session-handoff.md)：当前接力状态。
4. [_workflow.md](_workflow.md)：需要写作或归档时读取。

## 按需读取

- 当前案 `outline.md`：写当前案件或核对案件事实时。
- 最近 1 到 3 章正文原文：每章开写前必须读取。
- [_writing-style-guide.md](_writing-style-guide.md)：每章开写前读取第十节"写作检查清单"；风格跑偏时局部读取正文。
- [_characters.md](_characters.md)：角色状态或声口不确定时。
- [_cross-case-tracker.md](_cross-case-tracker.md)：涉及伏笔、能力、道具、破局方式时（伏笔和能力道具的唯一数据源）。
- [_series-outline.md](_series-outline.md)：设计新案或核对阶段规划时。

## 本地项目技能

本项目有项目专属技能库：`.agents/skills/`。这些文件不一定会被 Codex 自动作为全局 skill 触发；新会话应根据任务按需读取对应 `SKILL.md`，作为项目级流程补充。

- `.agents/skills/duxin-project-context/SKILL.md`：新会话启动、恢复当前进度、确认项目状态时。
- `.agents/skills/duxin-author-revision-learning/SKILL.md`：作者说“改好了”、Obsidian 同步改稿后，开写下一章前。
- `.agents/skills/duxin-chapter-writing/SKILL.md`：写下一章、续写正文、把草稿改成可提交正文时。
- `.agents/skills/duxin-editor-review/SKILL.md`：每章写完后的独立编辑审查和定向复审。
- `.agents/skills/duxin-feedback-capture/SKILL.md`：作者提出修改意见后，判断哪些要沉淀为长期规则时。
- `.agents/skills/duxin-continuity-check/SKILL.md`：核对伏笔、能力、道具、人物状态、案件事实和跨案连续性时。
- `.agents/skills/duxin-archive-update/SKILL.md`：作者确认章节或阶段后，更新接力、案纲和追踪文档时。
- `.agents/skills/duxin-case-design/SKILL.md`：设计新案、案件卡、证据链和章纲时。
- `.agents/skills/duxin-research-brief/SKILL.md`：需要现实刑侦、消防、法律、医学、舆论等资料核验时。
- `.agents/skills/duxin-obsidian-map/SKILL.md`：制作案件关系图、时间线、证据链图或 Obsidian Canvas 时。

## 权威层级

发生冲突时，按以下层级判断：

1. 已发布正文权威：网站发布章节。
2. 规则权威：[_series-rules.md](_series-rules.md)。
3. 案件事实与后续规划：当前案 `outline.md`。
4. 当前进度：[case-files/session-handoff.md](case-files/session-handoff.md)。
5. 本地工作正文：`case-files/` 下单章 Markdown。
6. 参考文档：其他项目文档。

## 核心红线速查

- 时菱能力：两米内免接触读心，只读目标当前最强烈表层念头。
- 能力例外：始终听不到顾晏廷心声。
- 持有道具：以 [_cross-case-tracker.md](_cross-case-tracker.md) 为准；不得擅自新增、使用或改写道具效果。
- 读心后不能立刻行动，中间至少有观察、验证或等待。
- 时菱是顾问，不是警察，不能越权执法。
- 顾晏廷不主动表白、不暧昧调情、不越界肢体接触、不替时菱推理。
- 禁止模板抒情、破折号、英文标点混入、角色同腔调。

## 流程速查

详细流程见 [_workflow.md](_workflow.md)。

- 新案开始前，先询问作者本案想写什么。
- 作者无想法时，AI 可以提供 2 到 3 个案型候选，但必须由作者确认。
- 案件卡确认后，才能扩写并保存案件章纲。
- 每章写前必读：当前案章纲、最近正文原文、写作检查清单。
- 如果当前案缺少 `outline.md`，先补当前案章纲，再继续写正文。
- 作者说“改好了”或通过 Obsidian 同步改稿后，下一章开写前必须先读取最新本地文件，并判断作者改动原因。
- 每章写前完成写前四问。
- 每章写后必须启动独立编辑 subagent 审查，不能由写作 AI 自行模拟。
- 作者确认后再更新接力文档、案纲和必要的全局追踪文档。

## 文档职责

- [_series-rules.md](_series-rules.md)：全书硬规则和写作红线。
- [_workflow.md](_workflow.md)：新案、单章、审查闭环、归档流程。
- [_editor-review.md](_editor-review.md)：独立编辑 subagent 的审查标准、输出格式和复审规则。
- [case-files/session-handoff.md](case-files/session-handoff.md)：当前接力状态。只记录最新进度、下一章方向、本轮工作状态。
- [_series-outline.md](_series-outline.md)：全书阶段、已写案件摘要、备选案池。
- [_cross-case-tracker.md](_cross-case-tracker.md)：跨案伏笔、能力道具、破局方式、可回归角色、感情线进度。伏笔和能力道具的唯一数据源。
- [_characters.md](_characters.md)：长期人物状态。
- 各案 `outline.md`：本案案件卡、章纲、证据链、未解决隐患、后续可回收点。
- `_templates/`：案件卡和案件章纲模板。
