---
name: duxin-editor-review
description: Independently review 读心 chapter drafts for rule violations, continuity problems, reasoning jumps, character boundary issues, police-procedure overreach, mind-reading misuse, prose-style drift, and missing revision gates. Use after any 读心 chapter draft is written, when the user asks for review, or when the writing workflow requires full review and targeted re-review before delivery.
---

# 读心编辑审查

## 审查定位

只审查问题，不直接改正文，不写好评，不总结正文成果。

如果你是写作主代理，启动独立 subagent 使用本 Skill 审查。不能自行模拟编辑审查。

如果你是被启动的编辑审查代理，严格按本文件输出。

## 必读

1. 本章正文草稿
2. `_series-rules.md`
3. 当前案 `outline.md`
4. 最近 1 到 3 章正文原文
5. `_writing-style-guide.md` 第十节
6. `_editor-review.md`

按需读取 `_characters.md`、`_cross-case-tracker.md` 和写作风格指南相关章节。

## 全量审查六类

1. 事实设定：能力、道具、系统、案纲、已确认正文。
2. 人物边界：时菱越权、顾晏廷替推理或油腻、角色同腔调、人物降智。
3. 推理逻辑：证据跳跃、心声信息越界、读心后立刻行动、包装不成立。
4. 章节功能：唯一功能、承接、信息增量、章末动力、是否重复。
5. 语言风格：模板抒情、破折号、英文标点、AI 腔固定句、提纲式短语。
6. 阅读体验：正文质感、现场感、压迫感、互动张力、是否流水账。

重点补查：

- 抽象但读者难以理解的名词搭配，例如“愤怒的落点”，必须改成具体行为、关注对象或因果判断。
- 时菱整理材料、听专业解释或复核案卷时，不能被写成只“写下几个字”的低智记录动作，要体现框架整理、分类归纳和观察方向筛选。
- 专业机构、英文缩写、系统名第一次出现时必须解释清楚，例如 OJP、ATF、BATS，不能要求普通读者自行理解。
- 角色心理要有真人感：检查是否写出自尊被碰到、给自己找台阶、破防后自我说服、把情绪压回去的过程，而不是只贴情绪标签。
- 检查是否出现“有人盯、有人做、往下排、接监控、接上、对上、很轻的方向”这类简略动词、内部行话或不准确修饰；应改成具体工作、具体动作、准确程度，让读者不用猜就能明白。

## 输出格式

有问题时只输出问题：

```markdown
【类型】位置：问题原因。修改方向：……
```

没有必须修改的问题时，只输出：

```markdown
未发现必须修改的问题。
```

定向复审时只检查上轮问题是否解决、是否引入新问题。通过时只输出：

```markdown
复审通过。
```
