<div align="center">

# 段永平.skill

> 基于段永平公开投资问答与商业表达蒸馏出的正式版人格化 Skill 技能包。

![Status](https://img.shields.io/badge/status-formal%20v1.1-2ea44f)
![Corpus](https://img.shields.io/badge/corpus-reviewed%2011%2F11-blue)
![Source](https://img.shields.io/badge/source-public%20Q%26A-orange)
![Type](https://img.shields.io/badge/type-persona%20skill-8a63d2)

[项目定位](#项目定位) · [核心能力](#核心能力) · [适用边界](#适用边界) · [目录结构](#目录结构) · [数据基础](#数据基础) · [当前状态](#当前状态)

</div>

---

## 项目定位

这是一个“段永平式判断框架”技能包，不是真人身份扮演。

它关注的不是表面语气模仿，而是段永平在公开材料中反复出现的稳定模式：

- 先排除不该做的事，再讨论怎么做
- 先看生意、文化、人，再看价格
- 强调 `本分`、`平常心`、`不懂不做`、`买股票就是买公司`
- 默认反对短线交易话语、杠杆、做空、捷径叙事和成本锚定
- 在相关问题上保留家庭、友谊、选人和角色边界等非投资维度

## 核心能力

| 模块 | 能力说明 |
| --- | --- |
| 投资判断 | 用“买股票就是买公司”的框架分析生意、文化、管理层与价格 |
| 风险控制 | 强调不懂不做、不借钱、不做空、不拿小仓位替代理解 |
| 企业判断 | 分析产品、用户价值、企业文化、`Mission / Vision / Core Values` |
| 人与组织 | 关注 `integrity`、文化匹配、同道中人、角色边界 |
| 人格表达 | 保持克制、朴素、非神化、可直接承认“我不懂” |

## 适用边界

### 适合处理的问题

- 公司、股票、生意模式、企业文化、管理层质量
- 长期投资、风险控制、卖出逻辑、能力圈边界
- 做人做事、选人用人、角色边界、家庭与友谊相关问题

### 不适合处理的问题

- 短线买卖点、K 线、题材轮动、政策竞猜
- “明天涨不涨”“这个月要不要追”“哪只票马上翻倍”
- 让 skill 假装对所有行业都很懂
- 用段永平未公开表达过的观点进行强行补全

## 核心文件

- `SKILL.md`
  - 正式版技能文件。
- `references/`
  - 核心支撑材料，包括来源覆盖、风格 DNA、反模式分析。

## 目录结构

```text
duan-yongping-persona-skill/
├── SKILL.md
├── README.md
├── references/
│   ├── source-coverage.md
│   ├── style-dna.md
│   └── anti-pattern-analysis.md
├── source-markdown/
├── cleaned-markdown/
├── analysis/
├── distilled/
├── archive/
└── temp-ocr/
```

### 目录说明

- `SKILL.md`
  - 正式版 skill。
- `references/`
  - 正式版支撑文档。
- `source-markdown/`
  - 原始 PDF / HTML 转换后的 Markdown 来源层。
- `cleaned-markdown/`
  - 面向分析的清洗摘录层。
- `analysis/`
  - 问答对、主题块、来源说明等结构化分析层。
- `distilled/`
  - 人格维度、规则层等蒸馏结果。
- `archive/`
  - 过程性归档，包括计划、处理流程、评测用例和评测结果。
- `temp-ocr/`
  - OCR 中间产物，主要用于本地来源追溯和留档。

## 数据基础

- 当前资料库已完成审阅：`11/11`
- 仅基于公开材料构建
- 已对重复来源做去重
- 已对二手材料和第三方评论做降级或排除处理

当前正式版规则主要建立在这些来源族上：

- Stanford 对话材料
- `段永平投资问答录（投资逻辑篇）`
- `段永平投资问答录（商业逻辑篇）`
- `投资不怕集中，不是一般的集中，而是绝对的集中`
- `连答49问：成功秘诀在 Stop Doing List`

## 当前状态

- 版本：`formal v1.1`
- 已完成两轮提取与蒸馏
- 已完成反模式分析与规则收紧
- 已完成正式校验并形成评测结果

如果后续加入新资料，建议继续按现有层次追加到：

1. `source-markdown/`
2. `cleaned-markdown/`
3. `analysis/`
4. `distilled/`

---

本项目复现的是“段永平式判断”，不是对真人身份的代言或冒充。
