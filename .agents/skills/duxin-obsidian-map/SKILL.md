---
name: duxin-obsidian-map
description: Create or update visual maps for the 读心 D:\AI\du_xin project, including Obsidian Canvas files, Mermaid diagrams, relationship maps, evidence chains, timelines, chapter flow maps, and foreshadowing recovery graphs. Use when the user asks for a 案件关系图, 证据链图, 时间线, 伏笔图, Obsidian Canvas, Mermaid 图, or visual organization of cases and characters.
---

# 读心 Obsidian 图谱

## 目标

把复杂案件、人物、证据和伏笔转成可视化结构，辅助后续写作。

## 资料来源

按图谱类型读取：

- 案件关系、证据链、时间线：当前案 `outline.md` 和相关正文。
- 跨案伏笔、能力、道具、破局方式：`_cross-case-tracker.md`。
- 长期人物关系：`_characters.md`。
- 全书阶段和已写案件：`_series-outline.md`。

## 输出选择

- 用户只要图：优先输出 Markdown Mermaid。
- 用户要 Obsidian Canvas：创建或更新 `.canvas` 文件。
- 用户要 Obsidian 笔记：使用 Obsidian Markdown 语法，内部链接用 wikilink。

## 文件位置

只有用户明确要求保存文件时才写入磁盘。

默认建议位置：

- 当前案图谱：`case-files/case-XX/maps/`
- 全书图谱：项目根目录下 `_maps/`

创建新目录前说明用途。不要移动或重命名正文文件。

## 图谱要求

- 一张图只表达一个概念。
- 关系边写清楚“证据”“怀疑”“排除”“待确认”“伏笔”。
- 未确认真相必须标注“待确认”或“创作方向”，不能画成既定事实。
- 图谱用于辅助写作，不替代案纲权威。
