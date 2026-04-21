# Requirement to PRD UI

从需求到网页原型的完整工作流工具链，帮助你快速将产品想法转化为可交互的网页原型。

## 功能概览

| 技能 | 描述 | 命令触发 |
|------|------|----------|
| [requirement-to-prd](./skills/requirement-to-prd/README.md) | 将用户需求转化为结构化的 PRD 文档，支持文档自检 | `/prd-generate`、`/prd-check` |
| [prd-to-prototype](./skills/prd-to-prototype/README.md) | 将 PRD 中的 UI 设计稿转化为可交互的 HTML 原型 | `/prototype-generate` |

## 快速开始

### 1. 生成 PRD 文档

直接告诉我你的产品想法：

```
我想做一个任务管理应用
```

或使用命令：

```
/prd-generate
```

### 2. 生成网页原型

在获得 PRD 文档后，继续：

```
根据这个 PRD 生成网页原型
```

或使用命令：

```
/prototype-generate
```

## 完整工作流

```
用户需求
    ↓
[requirement-to-prd] → 需求澄清 → 生成 PRD 文档 → 文档自检
    ↓
[prd-to-prototype] → 设计解析 → 生成 HTML 原型
    ↓
可交互的网页原型（可在浏览器直接打开）
```

## 项目结构

```
.
├── skills/
│   ├── requirement-to-prd/      # 需求转 PRD 技能
│   │   ├── SKILL.md
│   │   ├── README.md
│   │   └── reference/
│   │       └── PM.md            # PRD 生成规范
│   └── prd-to-prototype/        # PRD 转原型技能
│       ├── SKILL.md
│       ├── README.md
│       └── reference/
│           └── UIPrototypeGen.md # 原型生成规范
├── CLAUDE.md                     # Claude Code 配置
└── README.md
```

## 相关链接

- GitHub: https://github.com/ddddyyyy/requirement-to-prd-ui
