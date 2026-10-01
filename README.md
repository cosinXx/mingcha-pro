# 明察Pro（Ming Cha Pro）

> **明察秋毫，挖得深，看得清。**
> 适合所有场景的深入研究工作流：深度联网调研 + 多专家视角验证 + 可视化交互报告，一条流水线跑完。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-3.2.1-blue.svg)]()

## 这是什么

「明察Pro」是一套 **AI Agent 技能（Skill）**，把三件事合成一条流水线：

```
深度联网调研（8 阶段 · 多源交叉 · 置信度标注）
        ↓
多专家视角验证（4-6 视角并行 · 反方 Red Team 攻击）
        ↓
报告交付（默认：单文件交互式 HTML 报告）
```

**与普通搜索的区别**：普通搜索给十条链接；明察Pro 给一份结论固化、来源可溯、矛盾明示的报告——查了什么、信了什么、为什么信、哪里有分歧，一目了然。

## 核心能力

- **8 阶段研究流水线**：问题解构 → 搜索策略 → 原子搜索 → 信源分级 → 交叉验证 → 迭代反思 → 结论输出 → 报告生成
- **稀疏混合式注意力搜索**：关键词 + 语义向量混合召回
- **多专家视角验证**：4-6 个专家视角并行，含反方 Red Team 主动攻击结论
- **置信度标注**：每条结论标注高（>90%）/ 中（70-90%）/ 低（<70%）置信度
- **单文件交互式 HTML 报告（默认交付物）**：SVG 图表、时间线、置信度徽章、矛盾信息清单；自动适配系统浅色 / 深色，多端布局自适应
- **三档深度**：基础档（10-15 轮搜索）/ 标准档（15-20 轮）/ 深度档（20-30 轮）

## 适用场景

行业研究、企业尽调、竞品分析、技术调研、学术综述、舆情分析、市场调研、政策解读、产品分析、投资研究、事件复盘、人物背景调查……凡是需要"把一件事彻底查清楚"的场景，都是它的主场。

## 仓库结构

```
明察Pro/
├── SKILL.md                  # 技能主文件（触发条件 + 工作流 + 红线）
├── README.md                 # 本文件
├── references/               # 参考手册
│   ├── methodology.md        # 方法论
│   ├── search-playbook.md    # 搜索战术手册
│   ├── detailed-playbook.md  # 详细执行手册
│   ├── report-standards.md   # 报告规范
│   └── case-walkthrough.md   # 案例走查
└── assets/
    └── report-template.html  # 交互式 HTML 报告模板
```

## 安装

把整个文件夹放到你的 AI Agent 的 skills 目录下即可。常见路径：

- Claude Code: `~/.claude/skills/`
- Cursor: `~/.cursor/skills/`
- GitHub Copilot / 其他 Agent: 对应 skills 目录

## License

MIT
