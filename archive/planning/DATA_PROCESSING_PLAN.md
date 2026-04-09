# Duan Yongping Data Processing Plan

## Purpose
- Build a repeatable data-processing workflow for the Duan Yongping persona skill package.
- Prevent context loss: if the conversation restarts, this file should still explain how source material is collected, cleaned, extracted, and distilled.
- Separate raw-source ingestion from later trait extraction and final skill packaging.

## Fixed Scope
- Persona target: `段永平`
- Core material type: `公开投资问答`
- Current source folder: `D:\skills\段永平资料库`
- Current skill folder: `D:\skills\duan-yongping-persona-skill`

## Current Source Inventory

### PDF Files
1. `段永平：不为清单（Stop Doing List）.pdf`
2. `段永平：投资不怕集中，不是一般的集中， 而是绝对的集中.pdf`
3. `段永平的投资逻辑(雪球).pdf`
4. `段永平连答49问：成功秘诀在“Stop Doing List”.pdf`
5. `段永平投资问答录(商业逻辑篇).pdf`
6. `段永平投资问答录(投资逻辑篇).pdf`
7. `对话段永平. 2018.09.30 @斯坦福.pdf`
8. `在斯坦福对话段永平：Stop Doing List（附学习笔记）.pdf`
9. `早期报纸上的段永平.pdf`
10. `张昕帆：一次非常精彩的演讲.pdf`

### HTML File
1. `在斯坦福对话段永平：Stop Doing List（附学习笔记）.html`

## Output Layout

### Source-Derived Markdown
- `source-markdown/pdf/`: Markdown converted from PDF files
- `source-markdown/html/`: Markdown extracted from HTML source files

### Later Analysis Files
- `analysis/`: structured extraction notes by dimension
- `distilled/`: reusable rules, style DNA, anti-patterns, evaluation cases
- `references/`: supporting notes or mapping files if needed later
- `cleaned-markdown/`: analysis-ready cleaned excerpts derived from noisy source markdown

## Execution Stages

### Stage 1. Source Ingestion
- Keep the original source files unchanged in `D:\skills\段永平资料库`.
- Convert each PDF into Markdown.
- Extract readable article content from HTML and save it as Markdown.
- Preserve one output file per source file.

### Stage 2. Source Review
- Check whether each Markdown file is readable enough for later extraction.
- Note obvious issues such as OCR noise, broken line order, footer pollution, duplicated paragraphs, or truncated content.
- If a file is too noisy, mark it for secondary cleaning rather than forcing immediate analysis.

### Stage 3. Structured Segmentation
- Split long materials into smaller analysis units when needed.
- Preferred unit: one `Q/A pair`, one `topic block`, or one `speech segment`.
- Preserve source traceability: each extracted unit should still point back to source file and location.

### Stage 4. Trait Extraction
- Extract recurring patterns across multiple materials, not isolated quotes.
- Build notes by dimension, including but not limited to:
  - investment philosophy
  - circle of competence
  - risk and downside thinking
  - valuation and pricing logic
  - portfolio concentration
  - patience and holding period
  - market volatility and emotion control
  - expression style and rhetorical habits
  - refusal patterns and explicit boundaries

### Stage 5. Distillation
- Convert repeated patterns into reusable rules.
- Separate `judgment logic` from `language style`.
- Keep unstable, disputed, or one-off remarks out of the core persona rules unless later corroborated.

### Stage 6. Skill Packaging
- Write the final `SKILL.md` only after enough evidence has been accumulated.
- Pair the final skill with references, anti-patterns, and evaluation cases.

## Working Rules
- Source first, interpretation second.
- Public material only unless the user explicitly expands scope.
- Repetition across sources is stronger than a single quote.
- Do not treat third-party summaries as equal to first-hand answers.
- Distill stable thinking patterns before surface-level tone imitation.

## Handling Rules For This Project
- PDF files should be converted with `markitdown` when the extracted text quality is acceptable.
- HTML files should be ingested by extracting the readable article content directly, then saving it as Markdown.
- Converted Markdown should stay close to the source rather than being prematurely summarized.
- Cleaning and thematic extraction happen after the initial conversion pass.

## Current Immediate Tasks
1. Create Markdown output directories in the skill package.
2. Convert the current PDF batch into Markdown.
3. Extract the current HTML content into Markdown.
4. Review the generated files and identify any low-quality conversions.
5. Start the next round of structured extraction after the user confirms the conversion baseline is acceptable.

## Initial Baseline Status
- Baseline conversion date: `2026-04-09`
- PDF Markdown output folder: `source-markdown/pdf/`
- HTML Markdown output folder: `source-markdown/html/`
- Current conversion result:
  - `10/10` PDF sources now have Markdown counterparts
  - `9` PDFs were converted with `markitdown`
  - `1` scanned PDF (`早期报纸上的段永平.pdf`) was converted with a Windows OCR fallback after `markitdown` failed on the malformed, image-based source
  - `1` HTML source was extracted directly into Markdown

## Known Conversion Noise
- `段永平投资问答录(投资逻辑篇).md` contains `(cid:...)` artifacts from PDF text encoding.
- `段永平投资问答录(商业逻辑篇).md` may contain similar PDF encoding noise and should be reviewed during the cleaning pass.
- `早期报纸上的段永平.md` is OCR-derived and may contain recognition errors, footer contamination, and advertisement noise.
- `markitdown` emitted repeated `FontBBox` warnings during part of the PDF batch, but most target files were still generated successfully.

## Round 1 Progress
- Created `cleaned-markdown/round-1/` for analysis-ready cleaned excerpts.
- Created `analysis/round-1/` for structured extraction by `source / Q&A / topic block`.
- Created `distilled/round-1/` for first-pass persona and investment trait distillation.
- Round 1 currently prioritizes these source families:
  - Stanford Q&A material
  - `投资逻辑篇`
  - `商业逻辑篇`
  - early newspaper interview OCR support material

## Round 2 Progress
- Created `cleaned-markdown/round-2/` for newly added cleaned excerpts and support notes.
- Created `analysis/round-2/` for second-pass extraction focused on:
  - concentration and position sizing
  - selling rules and re-evaluation rules
  - culture definition and hiring rules
  - role boundaries, family, friendship, and social style
- Created `distilled/round-2/rule-layer.md` as a pre-SKILL compression layer.
- Created formal `SKILL.md` v1 based on round-1 and round-2 evidence.

## Formalization Status
- Formal skill package status: `v1.1 complete`
- Formal references added:
  - `references/source-coverage.md`
  - `references/style-dna.md`
  - `references/anti-pattern-analysis.md`
  - `archive/evaluation/eval-cases.md`
- `SKILL.md` tightened using the anti-pattern analysis so the current version is no longer only a draft rule set.

## Next Iteration Protocol
- When the user provides new material, place it into the source folder first.
- Add or update the relevant source-derived Markdown file.
- Record any conversion issues before starting trait extraction.
- Only after source ingestion is complete should the project move to thematic analysis and persona distillation.
