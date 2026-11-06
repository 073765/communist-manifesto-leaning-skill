# 《共产党宣言》精读学习技能

**Communist Manifesto Study Skill** — 一个用于系统精读《共产党宣言》的 Agent Skill。

它不是把书压缩成摘要，而是把文本拆成可检查的论证：每一章有论证路线、核心概念、精读片段、易误读处、自测题与参考答案；另附全书论证地图、术语表、分析模式、速查表、14 天学习计划与历史时间线。

## 30 秒体验

1. 准备一个支持 Agent Skills 的宿主：OpenCode、Claude Code、Codex、Cursor 等。
2. 安装（目录名用 `communist-manifesto`，与 `SKILL.md` 里的 `name` 一致）：

```bash
git clone https://github.com/073765/communist-manifesto-leaning-skill.git ~/.agents/skills/communist-manifesto
```

项目级安装（OpenCode）：克隆到项目的 `.opencode/skills/communist-manifesto`。

3. 新开一个会话，直接说：

> 用《共产党宣言》技能，考我第一章，别先给答案。

技能会先确认你的进度，再出题、等回答、点评，不会一次把答案倒给你。

## 适合谁

- 第一次系统阅读《共产党宣言》，需要有人按论证顺序带着读
- 读过片段，但说不清全书论证链条
- 想用苏格拉底式提问、自测和写作任务来检验理解
- 想区分「原文说了什么」「恩格斯注/编者注说了什么」「后人怎么解释」

## 内容

| 文件 | 作用 |
|---|---|
| `SKILL.md` | 技能入口与教学协议（讲解 / 提问 / 测验 / 原文定位） |
| `chapters/ch00-preface.md` | 七篇序言：版本史、自我修订、俄国道路、策略变化 |
| `chapters/ch01-bourgeois-proletarians.md` | 资产者和无产者：阶级斗争、资产阶级生成、危机、掘墓人 |
| `chapters/ch02-proletarians-communists.md` | 无产者和共产党人：消灭私有制、十项措施、联合体 |
| `chapters/ch03-socialist-literature.md` | 五类社会主义的阶级基础与历史作用 |
| `chapters/ch04-opposition-parties.md` | 联合与独立、德国问题、全世界无产者联合起来 |
| `argument-map.md` | 全书论证地图、五条推理链、五个可检验前提 |
| `glossary.md` | 术语表，含「慎用：常见误传术语」 |
| `patterns.md` | 九种分析模式与论证手法 |
| `cheatsheet.md` | 核心命题、十项措施、五类社会主义、误读对照 |
| `study-guide.md` | 14 天精读计划、自测题库、结课短文与评分标准 |
| `timeline.md` | 1847–1920 文本与历史双线时间线 |

## 安装

### 方式一：克隆到 Agent Skills 目录

个人级（跨 Agent，OpenCode / Claude Code / Codex 等）：

```bash
git clone https://github.com/073765/communist-manifesto-leaning-skill.git ~/.agents/skills/communist-manifesto
```

项目级（OpenCode）：

```bash
git clone https://github.com/073765/communist-manifesto-leaning-skill.git .opencode/skills/communist-manifesto
```

Windows 对应路径为 `%USERPROFILE%\.agents\skills\communist-manifesto`。

目录名要用 `communist-manifesto`，与 `SKILL.md` 的 `name` 字段保持一致；仓库名不同不影响使用。

### 方式二：skills CLI

```bash
npx skills add 073765/communist-manifesto-leaning-skill
```

加 `-g` 安装到全局，加 `-a opencode`（或 `-a claude-code`）直接指定宿主。

## 使用

安装后在新会话中直接说：

- 「用《共产党宣言》技能，按 14 天计划开始第 1 天」
- 「讲讲第一章的论证，标出原文页码和最容易读错的地方」
- 「考考我第一章，别直接给答案」
- 「第 37 页‘魔法师失控’那段什么意思」
- 「马克思说的‘消灭私有制’到底消灭什么？」

技能会按 `SKILL.md` 的教学协议工作：先定位章节，再讲解；区分原文、注释与后人解释；每次回答留一个检查问题。

## 关于页码与版本

- 所有页码均为技能制作时所用 PDF 的页码（中共中央马恩列斯著作编译局译本），**不是纸质书页码**。
- 不同版本页码会不同；引用时请以你手边的版本为准。
- 本仓库**不包含**《共产党宣言》全文或 PDF，只包含二次整理的讲解、结构与短引文。

## 版权与免责声明

- 《共产党宣言》原文（1848）已进入公有领域；本仓库所参考中文译本的著作权归原译者/出版方所有。
- 本仓库不收录原文全文；章节中的短引文仅用于评论、解释与学习，引用时标注页码。
- 本技能是学习辅助材料，不是学术定本，也不构成对任何政治制度的倡导或背书。
- 书中解释为编写者的阅读整理，欢迎批评指正。

## 生成方式

结构参考 [book-to-skill](https://github.com/virgiliojr94/book-to-skill)：把书拆成 `SKILL.md`、章节文件、术语表、模式、速查表与索引。本技能针对政治文本做了调整：`patterns.md` 改为分析模式与论证手法，并增加 `study-guide.md` 与 `timeline.md`。

---

如果这个技能对你有帮助，欢迎 star、提 issue 或提交 PR 改进章节与自测题。
