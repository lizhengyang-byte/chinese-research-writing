# Markdown delivery rules

Use this file whenever the deliverable is an article, report, thesis-style draft, or any other substantial Chinese long-form text.

## 1. Default deliverable type
The final deliverable should be markdown files.

- Prefer `.md` over `.docx`, `.pdf`, or plain chat text unless the user explicitly asks for another format.
- The chat reply can briefly explain what was generated, but the real deliverable should be the markdown file(s).

## 2. When to split
Split the output into separate chapter markdown files when either condition is met:
- the full article exceeds about 15000 Chinese characters, or
- any chapter exceeds about 3000 Chinese characters.

This is a practical threshold, not a rigid counting ritual. Estimate by the main prose length.

## 3. How to split
When splitting is required:
- keep one file per first-level chapter or major logical section
- preserve the agreed title and section order
- keep headings stable across files
- avoid over-fragmentation
- also generate one compiled markdown file that concatenates the full article in order

## 4. Naming convention
Use numeric prefixes so the files sort correctly.

Examples:
- `00-摘要.md`
- `01-引言.md`
- `02-研究背景.md`
- `03-主体分析.md`
- `04-结论.md`
- `99-全文汇总.md`

For non-academic writing, adapt the Chinese names to the actual section titles.

## 5. Compiled markdown file
The compiled file must:
- be directly readable as the single complete manuscript
- include all sections in the correct order
- preserve citation numbering and reference formatting
- resolve obvious cross-file transition issues if needed

## 6. Reference handling across files
- Keep one unified reference system.
- Do not renumber references differently in each chapter unless the user explicitly requests chapter-local references.
- If only the compiled file includes the full reference list, chapter files should still keep the in-text citation markers consistent with the compiled file.
