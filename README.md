# FM26 Scout Player Analyst

[中文](#中文) | [English](#english)

## 中文

这是一个个人使用的 Codex skill，用于根据 Football Manager 2026 的球员属性截图进行球员分析，尤其适合 FM Scout Engine / FMST26 这类球探工具的球员页面。

### 功能

- 从球员截图中提取可见属性和关键信息
- 评价球员当前能力、成长价值、强项和风险
- 推荐适合位置，以及 FM26 的有球/无球角色
- 给出战术适配建议，例如压迫、反击、传中、控球、低位防守等
- 推荐个人训练重点、角色训练方向和可考虑的球员习惯
- 区分截图证据、官方机制、球探工具数据和社区经验

### 安装

将这个仓库克隆到 Codex 的 skills 目录：

```bash
cd ~/.codex/skills
git clone https://github.com/likun199702/fm26-scout-player-analyst.git
```

如果目录已经存在，可以先备份旧版本，再替换或拉取更新。

### 使用方式

在新的 Codex 对话中显式调用：

```text
请使用 $fm26-scout-player-analyst 分析这个 FM26 / FM Scout Engine 球员截图。
```

推荐同时提供：

- 球员属性截图
- 年龄、位置、惯用脚、身高
- CA / PA 和隐藏属性，如果 FM Scout Engine / FMST26 中可见
- 你的战术：阵型、节奏、压迫高度、传中方式
- 你关心的问题：是否值得买、怎么用、练什么位置、练什么角色、是否出租

### 示例请求

```text
请使用 $fm26-scout-player-analyst。
这是一个 18 岁中卫，CA100 PA150。
帮我判断他是否值得重点培养，最适合的位置、有球/无球角色、个人训练重点，以及未来能不能踢主力。
```

### 说明

这个 skill 会参考 Football Manager 官方信息、FM Scout / FMST26 资料，以及社区角色属性经验。但它是玩家自用分析工具，不代表 Sports Interactive、Football Manager、FM Scout 或 FMST26 的官方观点。

## English

This is a personal Codex skill for analyzing Football Manager 2026 player screenshots, especially player pages from scouting tools such as FM Scout Engine / FMST26.

### What It Does

- Extracts visible player attributes and key profile details from screenshots
- Evaluates current ability, development value, strengths, and risks
- Recommends suitable positions and FM26 in-possession / out-of-possession roles
- Suggests tactical fit, including pressing, counter-attacking, crossing, possession, and low-block contexts
- Recommends individual training priorities, role training, and suitable player traits
- Separates screenshot evidence, official mechanics, scouting-tool data, and community heuristics

### Install

Clone this repository into your Codex skills folder:

```bash
cd ~/.codex/skills
git clone https://github.com/likun199702/fm26-scout-player-analyst.git
```

If the folder already exists, back up the old version before replacing or pulling updates.

### Usage

In a new Codex conversation, invoke the skill explicitly:

```text
Please use $fm26-scout-player-analyst to analyze this FM26 / FM Scout Engine player screenshot.
```

Helpful context to include:

- Player attribute screenshot
- Age, position, preferred foot, and height
- CA / PA and hidden attributes, if visible in FM Scout Engine / FMST26
- Your tactic: formation, tempo, pressing height, and crossing style
- Your question: whether to buy, how to use the player, which position or role to train, or whether to loan him out

### Example Prompt

```text
Please use $fm26-scout-player-analyst.
This is an 18-year-old centre-back with CA100 and PA150.
Tell me whether he is worth developing, his best position, in-possession and out-of-possession roles, individual training focus, and whether he can become a future starter.
```

### Notes

This skill may refer to official Football Manager information, FM Scout / FMST26 data, and community role-attribute heuristics. It is a fan-made personal analysis skill and is not affiliated with Sports Interactive, Football Manager, FM Scout, or FMST26.
