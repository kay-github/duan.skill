# Round 1 Source Notes

## Goal
- Define which source files are primary, which are supporting, and which should be treated as noisy-but-usable.
- Make the first extraction round reproducible even if the chat context is lost.

## Preferred Source Order

### Tier 1: Clean Primary Sources
- `source-markdown/html/在斯坦福对话段永平：Stop Doing List（附学习笔记）.md`
  - Best current source for direct Q/A style investment and life philosophy statements.
  - Preferred over the PDF version of the same event.

- `source-markdown/pdf/对话段永平. 2018.09.30 @斯坦福.md`
  - A concise note-style source for the same Stanford conversation.
  - Useful for quick cross-checking and finding compressed formulations.

### Tier 2: Rich But Noisy Core Sources
- `cleaned-markdown/round-1/investment-logic-excerpts.md`
  - Derived from `段永平投资问答录(投资逻辑篇).md`
  - Best current source for principles such as `不懂不做`、`能力圈`、`平常心`、`Stop Doing List`.

- `cleaned-markdown/round-1/business-logic-excerpts.md`
  - Derived from `段永平投资问答录(商业逻辑篇).md`
  - Best current source for business model, culture, integrity, consumer orientation, and `本分`.

### Tier 3: Early And OCR-Derived Supporting Source
- `cleaned-markdown/round-1/early-interview-excerpts.md`
  - Derived from OCR output of `早期报纸上的段永平.pdf`
  - Useful for early articulation of `产品第一、广告第二`、`守信誉`、`平常心`、`高速公路说`.
  - Treat as supportive rather than decisive when exact wording matters.

## Duplication Notes
- Stanford material currently exists in three forms:
  - `source-markdown/html/在斯坦福对话段永平：Stop Doing List（附学习笔记）.md`
  - `source-markdown/pdf/在斯坦福对话段永平：Stop Doing List（附学习笔记）.md`
  - `source-markdown/pdf/对话段永平. 2018.09.30 @斯坦福.md`
- For extraction and distillation, use the HTML-derived Markdown as the canonical version.
- Use the note-style PDF only as a compact cross-check.

## Known Noise Constraints
- Raw `投资逻辑篇` and `商业逻辑篇` contain many `(cid:...)` artifacts and page layout residues.
- Raw `早期报纸上的段永平.md` contains OCR errors, ad pollution, and some broken characters.
- Cleaned round-1 excerpt files are analysis-ready but not yet full-text normalized editions.

## Round 1 Working Rule
- If a point appears in both Stanford material and one or more long-form collections, treat it as stronger evidence.
- If a point appears only in OCR-derived early material, keep it as supportive rather than core until corroborated.
- When quoting in later synthesis, prefer the cleanest available source text rather than the noisiest earliest source.
