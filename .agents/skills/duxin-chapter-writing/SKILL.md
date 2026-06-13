---
name: duxin-chapter-writing
description: Write or continue a chapter for the 读心 D:\AI\du_xin serialized crime novel. Use when the user asks to write the next chapter, continue the current case, draft a chapter, revise a chapter into publishable prose, or proceed from the latest Obsidian-synced manuscript while obeying the project workflow, chapter outline, recent chapters, writing checklist, and mandatory editor review gate.
---

# 读心单章写作

## 定位

按《读心》项目流程写一章正文。重点是读取最新上下文、完成写前四问、写出正文、保存草稿，并启动独立编辑审查。

## 动笔前必读

先定位项目根目录：当前目录含 `AGENTS.md` 时使用当前项目，否则使用 `D:\AI\du_xin`。

每章开写前读取：

1. `AGENTS.md`
2. `_series-rules.md`
3. `case-files/session-handoff.md`
4. 当前案 `outline.md`
5. 最近 1 到 3 章正文原文。若用户说“改好了”，先列当前案目录，读取最新本地文件。
6. `_writing-style-guide.md` 第十节“写作检查清单”

按需读取：

- `_characters.md`：出场主角、顾晏廷、三队或长期人物声口不确定时。
- `_cross-case-tracker.md`：涉及能力、道具、伏笔、感情线、破局方式时。

## 写前四问

动笔前在思考中完成四问，每问一句：

1. 本章唯一功能。
2. 本章必须承接。
3. 本章风险红线。
4. 本章不能提前完成或揭示。

除非方向不明，不把四问发给用户。

## 正文要求

- 单章正文控制在 3000 字以内，除非用户明确要求加长。
- 沿用当前案目录文件命名风格：`三位排序号_第N章  标题.md`。
- 不重命名、不移动、不删除旧正文。
- 时菱是顾问，不越权执法。
- 读心半径三米，免接触，只读当前最强烈表层念头；听不到顾晏廷心声。
- 读心后至少有一拍观察、验证或等待。
- 顾晏廷不替时菱推理，不主动表白，不暧昧，不越界接触。
- 刑侦表达写完整句，避免“查人”“多刀”“压第二类”等提纲式口吻。
- 专业解释、案卷整理和时菱记录要写成框架搭建、分类归纳、筛选观察方向；避免“写下几个字”这类低智记录动作。
- 避免抽象但读者听不懂的名词搭配，例如“愤怒的落点”；改写成具体行为、关注对象或因果判断。
- 专业机构、英文缩写、系统名第一次出现时必须用自然中文解释清楚；不要让读者自行理解 OJP、ATF、BATS 这类缩写。
- 角色心理要写出真人感：自尊被碰到、给自己找台阶、破防后自我说服、把情绪压回去；不要只贴情绪标签。
- 避免“有人盯、有人做、往下排、接监控、接上、对上、很轻的方向”这类简略动词、内部行话或不准确修饰；写成具体工作、具体动作、准确程度，让读者不用猜就能明白。
- 章末有钩子，但不提前揭示真凶或核心反转。

## 写后门禁

正文完成后必须启动独立编辑 subagent，使用 `duxin-editor-review` 的规则。不得由写作 AI 自行模拟编辑审查。

流程：

1. 写作 AI 完成草稿。
2. 独立编辑全量审查，只报问题。
3. 写作 AI 修改正文。
4. 独立编辑定向复审。
5. 复审通过后，最终回复作者。

最终回复第一句必须标注本章当前正文字数。作者确认前，不更新接力文档、案纲或全局追踪文档。

## 作者反馈后

作者提出修改意见后，先修改当前正文；如果反馈包含“以后”“后续”“每次”或明显是反复出现的写作问题，按 `duxin-feedback-capture` 判断是否需要沉淀为长期规则。
