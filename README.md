# PPT SVG 生成器

> 🎨 将 Markdown 文稿转化为精美、可编辑的 PPT 页面

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## ✨ 项目简介

**PPT SVG 生成器** 是一个 [OpenCode](https://github.com/opencode-ai/opencode) Skill，帮助你将 Markdown 文稿快速转化为可导入 PowerPoint 的 SVG 文件。

### 🎯 核心特性

- **智能文稿分析** - 自动拆解内容，生成结构化页面清单
- **多风格支持** - 5 种预设风格 + 自定义配色 + AI 智能推荐
- **PPT 原生兼容** - 生成的 SVG 支持「转换为形状」后二次编辑
- **批量生成** - 一键输出所有 PPT 页面

### 📐 输出规格

| 规格 | 说明 |
|------|------|
| 尺寸 | 1920 × 1080 px (16:9) |
| 格式 | SVG（矢量，无损缩放） |
| 字体 | Microsoft YaHei / SimHei / PingFang SC |
| 兼容性 | PowerPoint 2016+ / WPS |

---

## 🚀 快速开始

### 前置要求

- 安装 [OpenCode](https://github.com/opencode-ai/opencode)
- 将本项目放置于 OpenCode 的 skills 目录

### 使用流程

```
┌─────────────────────────────────────────────────────────────────┐
│                        PPT SVG 生成流程                          │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  步骤 1️⃣  /ppt-analyze @文稿.md                                  │
│           → 分析文稿，输出页面结构清单                            │
│                                                                 │
│  步骤 2️⃣  /ppt-design                                            │
│           → 选择风格（预设/自定义/AI推荐）                        │
│                                                                 │
│  步骤 3️⃣  /ppt-generate                                          │
│           → 批量生成 SVG 文件                                    │
│                                                                 │
│  步骤 4️⃣  导入 PPT → 转换为形状 → 微调完成 ✅                     │
└─────────────────────────────────────────────────────────────────┘
```

### 快速示例

```
我有一份文稿 @report.md，请帮我：
1. 分析内容，拆解成 PPT 页面
2. 使用「品牌蓝」风格
3. 生成所有 SVG 文件
```

---

## 🎨 预设风格

| 风格 | 特点 | 适用场景 |
|------|------|---------|
| **极简主义** | 纯白背景，大量留白 | 产品发布、设计分享 |
| **商务咨询** | 深蓝稳重，McKinsey 风 | 方案汇报、咨询报告 |
| **科技暗黑** | 霓虹渐变，玻璃拟态 | 技术分享、产品演示 |
| **瑞士平面** | 强烈对比，包豪斯风 | 创意提案、品牌展示 |
| **品牌蓝** | 蓝紫青配色，现代专业 | 企业培训、通用演示 |

---

## 📁 项目结构

```
ppt-svg-generator/
├── SKILL.md              # Skill 配置文件
├── commands/             # 命令定义
│   ├── analyze.md        # /ppt-analyze 文稿分析
│   ├── design.md         # /ppt-design 风格设计
│   └── generate.md       # /ppt-generate 批量生成
├── specs/                # 规范文档
│   ├── svg-compatibility.md  # SVG→PPT 兼容性规范
│   ├── design-system.md      # 设计系统（字体、间距）
│   └── page-templates.md     # 页面模板（封面、观点等）
└── styles/               # 风格定义
    ├── 00-style-index.md     # 风格索引
    ├── 01-minimalism.md      # 极简主义
    ├── 02-consulting.md      # 商务咨询
    ├── 03-tech-dark.md       # 科技暗黑
    ├── 04-swiss-style.md     # 瑞士平面
    └── 05-brand-blue.md      # 品牌蓝
```

---

## 🔧 PPT 导入说明

1. **导入 SVG** - 将生成的 SVG 文件拖入 PowerPoint
2. **转换为形状** - 右键点击 → 选择「转换为形状」
3. **二次编辑** - 现在可以修改文字、颜色、位置等

> ⚠️ **注意**：阴影效果需要在 PPT 中手动添加（格式 → 形状效果 → 阴影）

---

## 📖 详细文档

| 文档 | 说明 |
|------|------|
| [SVG 兼容性规范](specs/svg-compatibility.md) | PPT 转换的 5 条核心规则 |
| [设计系统](specs/design-system.md) | 字体、间距、组件规范 |
| [页面模板](specs/page-templates.md) | 各类页面的布局定义 |

---

## 📄 许可证

本项目采用 [MIT 许可证](LICENSE) 开源。

---

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

如果这个项目对你有帮助，请给个 ⭐ Star 支持一下！
