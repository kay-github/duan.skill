# Source Coverage

## Status
- Corpus review status: `complete for current source set`
- Current source set reviewed: `11/11`
- No remaining unreviewed files in `source-markdown/`

## Coverage Table

| Source file | Source type | Role in formal skill | Current handling | Notes |
| --- | --- | --- | --- | --- |
| `source-markdown/html/在斯坦福对话段永平：Stop Doing List（附学习笔记）.md` | direct Q&A | canonical primary | extracted | preferred Stanford source |
| `source-markdown/pdf/在斯坦福对话段永平：Stop Doing List（附学习笔记）.md` | direct Q&A pdf copy | duplicate family support | reviewed, not separately extracted | lower priority than html version |
| `source-markdown/pdf/对话段永平. 2018.09.30 @斯坦福.md` | direct note-style summary | primary support | extracted | concise cross-check source |
| `source-markdown/pdf/段永平：不为清单（Stop Doing List）.md` | direct Q&A republication | duplicate family support | reviewed, used for cross-check | overlaps strongly with Stanford and 49问 |
| `source-markdown/pdf/段永平连答49问：成功秘诀在“Stop Doing List”.md` | direct Q&A republication | primary | extracted in round 2 | best for culture, family, role-boundary details |
| `source-markdown/pdf/段永平投资问答录(投资逻辑篇).md` | long-form direct collection | primary | extracted in round 1 | strong for stop-doing, ability circle, calm mind |
| `source-markdown/pdf/段永平投资问答录(商业逻辑篇).md` | long-form direct collection | primary | extracted in round 1 | strong for culture, integrity, business model, 本分 |
| `source-markdown/pdf/段永平：投资不怕集中，不是一般的集中， 而是绝对的集中.md` | direct article / essay | primary | extracted in round 2 | strongest source for concentration and selling rules |
| `source-markdown/pdf/早期报纸上的段永平.md` | OCR from scanned interview | supporting primary | extracted in round 1 | use with caution when exact wording matters |
| `source-markdown/pdf/段永平的投资逻辑(雪球).md` | secondary article | support only | reviewed and noted in round 2 | useful corroboration, not sole basis |
| `source-markdown/pdf/张昕帆：一次非常精彩的演讲.md` | third-party external commentary | excluded from core persona | reviewed and excluded | not a direct Duan Yongping source |

## Processed Outputs Map

### Round 1 Outputs
- `cleaned-markdown/round-1/investment-logic-excerpts.md`
- `cleaned-markdown/round-1/business-logic-excerpts.md`
- `cleaned-markdown/round-1/early-interview-excerpts.md`
- `analysis/round-1/source-notes.md`
- `analysis/round-1/qa-pairs.md`
- `analysis/round-1/topic-blocks.md`
- `distilled/round-1/persona-dimensions.md`

### Round 2 Outputs
- `cleaned-markdown/round-2/concentration-excerpts.md`
- `cleaned-markdown/round-2/stanford-49-excerpts.md`
- `cleaned-markdown/round-2/xueqiu-investment-logic-notes.md`
- `analysis/round-2/source-notes.md`
- `analysis/round-2/qa-pairs.md`
- `analysis/round-2/topic-blocks.md`
- `distilled/round-2/rule-layer.md`

## Formal-Skill Coverage Conclusion
- Formal skill rules are built from all direct primary source families in the current corpus.
- Duplicate source families were reviewed and de-duplicated rather than repeatedly extracted.
- Secondary and third-party materials were reviewed, classified, and either downgraded to support or excluded from core rule writing.
