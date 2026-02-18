# 配图助手 (Image Assistant)

> 本技能来自 [yunshu0909/yunshu_skillshub](https://github.com/yunshu0909/yunshu_skillshub)，由云舒老师原创。我将其独立提取出来以便单独使用和维护。

---

[English](#english) | [中文](#中文)

---

## 中文

### 📖 简介

配图助手是一个 Claude Code Skill，帮助你把文章或模块内容转换成统一风格、少字高可读的 16:9 信息图提示词。

### ✨ 适用场景

- 文章需要配图但不知道怎么设计
- PPT、海报、社媒图需要统一风格
- 内容太多字，想要更趣味、更好读的视觉呈现
- 需要批量生成配图提示词

### 🎯 核心功能

- 📋 **需求澄清**：挖掘内容、场景、受众和字数偏好
- 🗂️ **配图规划**：拆分内容，定义图清单（几张图/每张讲什么）
- ✍️ **文案定稿**：逐字定稿"图上写什么"（Copy Spec）
- 🎯 **提示词封装**：生成可复制的生图提示词，支持批量出图
- 🔄 **迭代润色**：根据反馈减字、换隐喻、提升可读性
- 💬 **会话状态恢复**：每阶段标注当前进度，中断后可无缝继续

### 🚀 快速开始

#### 安装

**使用 Claude Code CLI 安装**

直接跟 AI 说：

```
安装这个 GitHub 库：https://github.com/ssdiwu/image-assistant
```

**手动安装**

```bash
# Claude Code 默认 Skills 目录通常是 ~/.claude/skills/
cd ~/.claude/skills/

# 克隆本仓库
git clone https://github.com/ssdiwu/image-assistant.git
```

#### 使用

在 Claude Code CLI 中：

```
# 使用配图助手
/image-assistant

# 或者直接描述需求
这段内容做个图/配几张图？
给我两张出图提示词
字太多不好看，帮我更趣味、更好读
```

### 📂 项目结构

```
.
├── SKILL.md                 # Skill 定义文件
├── README.md                # 项目说明文档
├── stages/                  # 各阶段详细说明
│   ├── 01-brief.md         # 需求澄清
│   ├── 02-plan.md          # 配图规划
│   ├── 03-copy.md          # 文案定稿
│   ├── 04-prompts.md       # 提示词封装
│   └── 05-iterate.md       # 迭代润色
├── templates/               # 风格模板和配图模板
│   ├── style-block.md      # 默认风格块
│   ├── 16x9-infographic.md # 信息图模板
│   ├── 16x9-contrast-2cards.md   # 对比卡片模板
│   ├── 16x9-3cards-insights.md   # 三卡见解模板
│   ├── 16x9-cover-roadmap.md     # 封面路线图模板
│   ├── 16x9-5panel-comic.md      # 五格漫画模板
│   └── checklist.md        # 检查清单
└── examples/                # 使用示例
    └── ai-tools-selection.md
```

### 🤝 致谢

本技能由 [云舒](https://github.com/yunshu0909) 原创，首发于 [yunshu_skillshub](https://github.com/yunshu0909/yunshu_skillshub) 项目。

### 📄 许可证

本项目继承原项目的 [MIT License](./LICENSE)。

---

## English

### 📖 Introduction

Image Assistant is a Claude Code Skill that helps you convert article or module content into unified-style, text-minimal, highly readable 16:9 infographic prompts.

### ✨ Use Cases

- Need illustrations for articles but don't know how to design
- PPT, posters, or social media graphics need a unified style
- Too much text, want more engaging and readable visual presentation
- Need to batch generate illustration prompts

### 🎯 Core Features

- 📋 **Requirement Clarification**: Extract content, scenario, audience, and text density preferences
- 🗂️ **Illustration Planning**: Split content, define image list (how many/what each explains)
- ✍️ **Copy Finalization**: Word-by-word finalization of "what text goes on the image" (Copy Spec)
- 🎯 **Prompt Packaging**: Generate copy-ready image generation prompts, support batch generation
- 🔄 **Iterative Refinement**: Reduce text, change metaphors, improve readability based on feedback
- 💬 **Session State Recovery**: Stage progress is tracked so you can resume seamlessly after interruption

### 🚀 Quick Start

#### Installation

**Using Claude Code CLI**

Simply tell the AI:

```
Install this GitHub repository: https://github.com/ssdiwu/image-assistant
```

**Manual Installation**

```bash
# Claude Code default Skills directory is usually ~/.claude/skills/
cd ~/.claude/skills/

# Clone this repository
git clone https://github.com/ssdiwu/image-assistant.git
```

#### Usage

In Claude Code CLI:

```
# Use Image Assistant
/image-assistant

# Or just describe your needs
Make an image for this content
Give me two image generation prompts
Too much text, make it more engaging and readable
```

### 📂 Project Structure

```
.
├── SKILL.md                 # Skill definition file
├── README.md                # Project documentation
├── stages/                  # Detailed stage descriptions
│   ├── 01-brief.md         # Requirement clarification
│   ├── 02-plan.md          # Illustration planning
│   ├── 03-copy.md          # Copy finalization
│   ├── 04-prompts.md       # Prompt packaging
│   └── 05-iterate.md       # Iterative refinement
├── templates/               # Style templates and layout templates
│   ├── style-block.md      # Default style block
│   ├── 16x9-infographic.md # Infographic template
│   ├── 16x9-contrast-2cards.md   # Contrast cards template
│   ├── 16x9-3cards-insights.md   # Three-card insights template
│   ├── 16x9-cover-roadmap.md     # Cover roadmap template
│   ├── 16x9-5panel-comic.md      # Five-panel comic template
│   └── checklist.md        # Checklist
└── examples/                # Usage examples
    └── ai-tools-selection.md
```

### 🤝 Credits

This skill was originally created by [Yunshu](https://github.com/yunshu0909) and first published in the [yunshu_skillshub](https://github.com/yunshu0909/yunshu_skillshub) project.

### 📄 License

This project inherits the original project's [MIT License](./LICENSE).
