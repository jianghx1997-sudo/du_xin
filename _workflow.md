# 写作工作流

> 本文件规定协作流程：新案怎么启动，单章怎么写，写后怎么审查，确认后怎么归档。编辑审查执行规则见 [_editor-review.md](_editor-review.md)。

---

## 一、权威层级

权威层级见 [AGENTS.md](AGENTS.md)。本流程遵守该层级。

---

## 二、文档调用矩阵

| 场景 | 必读 | 按需读取 | 必更新 |
|------|------|----------|--------|
| 新会话启动 | `AGENTS.md`、`_series-rules.md`、`case-files/session-handoff.md` | 当前案 `outline.md` | 无 |
| 新案设计 | `_series-outline.md`、`_cross-case-tracker.md`、`_templates/case-card.md` | `_characters.md` | 新案 `outline.md` |
| 单章写作 | 当前案 `outline.md`、最近 1 到 3 章正文原文、`_writing-style-guide.md` 第十节 | `case-files/session-handoff.md`、`_characters.md` 本章出场人物条目、`_cross-case-tracker.md`、`_writing-style-guide.md` 相关章节 | 无 |
| 作者反馈修改 | 当前章草稿、作者反馈、`_workflow.md` | `_writing-style-guide.md`、`_editor-review.md`、当前案 `outline.md`、本地技能 `.agents/skills/duxin-feedback-capture/SKILL.md` | 当前章；长期反馈按第六节第4点归档 |
| 写后审查 | 本章草稿、`_editor-review.md`、`_series-rules.md`、当前案 `outline.md`、最近 1 到 3 章正文原文、`_writing-style-guide.md` 第十节 | `_characters.md` 本章出场人物条目、`_cross-case-tracker.md`、`_writing-style-guide.md` 相关章节 | 无 |
| 作者确认后 | 无 | 当前案 `outline.md` | `case-files/session-handoff.md`、当前案 `outline.md`（如有事实变化） |
| 案件收尾 | 当前案 `outline.md`、`_cross-case-tracker.md`、`_series-outline.md` | `_characters.md` | `session-handoff.md`、当前案 `outline.md`、`_cross-case-tracker.md`、`_series-outline.md`、`_characters.md`（如人物状态变化） |

---

## 三、小说内容优先原则

- 本项目首先是长篇小说，不是文档工程。所有流程只服务正文质量。
- 写正文时优先保留：当前案章纲、本章相关事实、最近正文、写作检查清单、出场人物声口。
- 真正的优先级是：章纲事实 > 最近正文语气 > 人物声口 > 文风节奏 > 规则红线 > 流程规范。
- 长文档按需检索，不默认全文加载，但不能为了省上下文牺牲正文质感。
- `_characters.md`、`_cross-case-tracker.md`、`_series-outline.md` 默认不全文读取。
- `_writing-style-guide.md` 每章读取第十节，正文部分按风格问题局部读取。
- 如果上下文紧张，优先丢弃参考性文档，不能丢弃当前案章纲、本章相关事实和最近正文。
- 写作 AI 的上下文优先服务创作；审查细则交给独立编辑 subagent。
- `session-handoff.md` 必须保持短，只记录最新进度、下一章方向、本轮工作状态，不保存正文摘要或项目总览。
- 新规则只写到最直接生效的位置，避免同一要求在多个文档反复铺开；能合并进既有检查项的，不新增长段说明。

---

## 四、章节文件规范

- 不重命名、不移动已写正文文件。
- 历史章节编号不一致时，以正文标题中的章号和已发布网站章节为准。
- 文件名前缀只作为本地排序号，可与正文标题章号不同。
- 新章节文件沿用当前目录风格：`三位排序号_第N章 标题.md`。
- 新章节保存前，先确认应归属的案件目录；新案则先创建对应 `case-XX/outline.md`。

---

## 五、新案流程

**触发**：开始设计新案件之前。

### 1. 询问作者

AI 必须先询问作者本案想写什么。

- 作者有想法：AI 将作者想法整理成案件卡。
- 作者没有想法：AI 提供 2 到 3 个案型候选，供作者选择。
- AI 可以提案，但不能自行决定新案方向。

### 2. 案件卡确认

案件卡至少包含：

- 案件类型与社会影响力。
- 受害者、真凶、核心动机。
- 核心证据，以及证据为什么会留下。
- 破局方式，以及与前案的差异。
- 时菱发挥点，以及对外包装方式。
- 顾晏廷和三队各自承担的功能。
- 本案推进的主线、伏笔或人物关系。

可使用 [_templates/case-card.md](_templates/case-card.md) 作为格式参考。

作者确认案件卡后，才能扩写章纲。

### 3. 章纲保存

案件卡确认后，AI 扩写为当前案 `outline.md` 并保存到对应 `case-files/case-XX/` 目录。

可使用 [_templates/case-outline.md](_templates/case-outline.md) 作为格式参考。

章纲保存后，才开始逐章写正文。

---

## 六、单章流程

**触发**：每章开始写之前。

### 1. 必读上下文

每章开写前，AI 必须读取：

- 新会话首次写作时，先读取 [_series-rules.md](_series-rules.md)
- 当前案 `outline.md`
- 最近 1 到 3 章正文原文
- [_writing-style-guide.md](_writing-style-guide.md) 第十节

如果当前案目录已有正文但缺少 `outline.md`，必须先补当前案章纲。章纲不需要把未确认真相写死，但必须记录已确认事实、线索等级、人物状态、章节功能和本案红线。

按需读取：

- [case-files/session-handoff.md](case-files/session-handoff.md)：当前进度和下一章方向
- [_characters.md](_characters.md)：本章涉及主要人物时，读取相关人物条目
- [_cross-case-tracker.md](_cross-case-tracker.md)：涉及伏笔、道具、能力、破局方式时
- [_writing-style-guide.md](_writing-style-guide.md) 相关章节：风格明显跑偏时

`session-handoff.md` 不保存正文摘要，必须直接读正文原文。

### 1.5 作者改稿学习

作者说“改好了”或通过 Obsidian 同步改稿后，开写下一章前必须先读取最新本地文件；如果文件名不确定，先列目录确认。读取后用极短要点判断：

- 作者删掉了什么，以及为什么删。
- 作者加强了什么，以及下一章要承接什么。
- 作者是否改变了章节功能、线索等级或人物判断时机。
- 下一章哪些东西不能提前揭示、提前拔高或提前下结论。

这一步只服务下一章写作，不写进正文，也不写进 `session-handoff.md`。

### 2. 写前四问

动笔前先完成四问。四问只用于定位，不写入正文；除非方向不明，不需要作者确认。

```markdown
## 写前四问

1. 本章唯一功能：
2. 本章必须承接：
3. 本章风险红线：
4. 本章不能提前完成或揭示：
```

要求：

- 每问一句话。
- 本章唯一功能只能有一个。
- 风险红线只写本章最可能踩的一到两条。
- “不能提前完成或揭示”用于控制线索、嫌疑人判断、情绪结论和感情线进度。

### 3. 正文写作

正文必须遵守：

- 当前案章纲。
- `_series-rules.md` 全书规则。
- 已确认正文事实。
- 作者已确认的方向。
- 单章正文控制在 3000 字以内，除作者明确要求加更或扩写外，不写成长章。

写作 AI 不得擅自改变真凶、关键证据、人物关系阶段、系统奖励或案件走向。

旧案、跨地协作或重启案件中，优先尊重原办案人的既有工作：女主先提出工作方式或观察角度，再通过亲自观察、心声和证据复核推动进展，不能一入场就替多年侦查下结论。

### 4. 作者反馈沉淀

作者对草稿提出修改意见时，写作 AI 必须先修改当前正文，再判断每条反馈是否需要长期沉淀。

分类规则：

- **本章局部问题**：只修改当前章，不写入项目文档。
- **本案持续问题**：影响当前案后续事实、线索、人物状态或章节方向时，作者确认后更新当前案 `outline.md` 或 `session-handoff.md`。
- **全书硬规则**：涉及能力、道具、身份边界、顾晏廷红线、系统机制时，更新 `_series-rules.md` 或 `_cross-case-tracker.md`。
- **长期语言风格**：涉及句子过短、提纲式表达、心声信息量、对话逻辑、情绪判断时机等写作习惯时，优先更新 `_writing-style-guide.md` 第十节；需要编辑门禁检查的，同步更新 `_editor-review.md`。
- **流程要求**：涉及写前、写后、审查、字数、归档等协作方式时，更新 `_workflow.md`。
- **本地技能要求**：如果某条长期反馈会影响对应任务入口，同步更新 `.agents/skills/` 下最相关的 `SKILL.md`。

沉淀原则：

- 新规则只写到最直接生效的位置，避免多处重复。
- 能合并进既有检查项的，不新增长段说明。
- 最终回复作者时，简短说明哪些反馈已归档为长期规则。

---

## 七、写后审查闭环

**触发**：每章正文写完后，提交作者前。审查是强制门禁。

详细审查标准、输出格式和定向复审规则见 [_editor-review.md](_editor-review.md)。本节只保留写作 AI 必须执行的流程门禁。

### 固定流程

1. 写作 AI 完成正文。
2. 强制启动独立编辑 subagent 做全量审查。
3. 编辑 subagent 只报问题，不直接改稿，不写好评，不总结正文成果。
4. 写作 AI 根据问题修改正文。
5. 强制启动编辑 subagent 做定向复审。
6. 复审通过后，提交作者确认。

### 作者强调补充

- 编辑审查意见不能直接作为最终交付。
- 写作 AI 必须先把编辑提出的问题改进正文，再完成定向复审。
- 最终回复作者时，开头先标注本章当前正文字数。
- 最终回复作者时，只汇报已修改内容和复审结果；除非作者要求，不把未处理的审查意见抛给作者。
- 作者指出流程遗漏时，必须立刻补做“修改正文 + 定向复审”，并将该要求纳入后续工作默认流程。

### 循环限制

- 最多两轮"修改加定向复审"。
- 两轮后仍无法解决，提交作者决策。
- 涉及故事方向、关键证据、人物关系阶段、已确认事实的修改，必须先问作者。

### 禁止

- 写作 AI 自行模拟编辑 subagent 审查。
- 未经独立编辑 subagent 审查就提交作者。
- 编辑 subagent 直接改正文。

---

## 八、确认与归档

**触发**：作者确认章节后。

### 1. 每章确认后

更新：

- [case-files/session-handoff.md](case-files/session-handoff.md)：最新进度、下一章方向、本轮工作状态。

必要时更新：

- 当前案 `outline.md`：正文改变案件事实、证据链、人物状态、未解决隐患时。

### 2. 案件结束后

更新：

- [_cross-case-tracker.md](_cross-case-tracker.md)：跨案伏笔、能力道具、破局方式、可回归角色、感情线进度。
- [_series-outline.md](_series-outline.md)：案件摘要和阶段进度。
- [_characters.md](_characters.md)：人物长期状态发生变化时。

### 3. 不需要归档的内容

以下内容不写入全局文档：

- 单章临时情绪。
- 普通场景调度。
- 不影响后续的对话细节。
- 已由正文完整承载、无需复用的信息。
