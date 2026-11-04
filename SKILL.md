---
name: chinese-research-writing
description: produce high-rigor chinese writing for theses, research reports, academic-style papers, long-form articles, special reports, commentary, and news-feature drafts in markdown. use when the user asks to create, rewrite, expand, polish, or structure substantial chinese prose; when a topic needs web research before writing; when the output should support outline, first-draft, or final-draft modes; or when evidence, source attribution, argument structure, formal style, and markdown file delivery matter. automatically split long outputs into chapter-level markdown files when the article exceeds 15000 chinese characters or any chapter exceeds 3000 chinese characters, and also generate one compiled markdown file.
---

# Chinese research writing

Deliver publication-grade Chinese long-form writing with strong evidence, explicit structure, and genre control. Default to rigorous, source-grounded prose rather than generic AI-style summaries.

## Core objective

Write in Chinese only. Optimize for depth, credibility, and readability across these target genres:
- 硕士论文级研究报告与论文
- 学术风格文章、综述、述评
- 行业/政策/专题研究报告
- 深度文章、特稿、专题报道
- 新闻报道、解释性报道、人物/议题特写
- 演讲稿、申论式论述、综合型长文

Always adapt the tone, section order, evidence density, and citation style to the requested genre while preserving a high standard of reasoning and source traceability.

## Mandatory workflow

Follow this sequence unless the user explicitly limits the task.

1. **Clarify the mission from available context**
   Infer and restate internally:
   - topic and central question
   - target genre
   - target audience
   - required output level: 提纲版 / 初稿版 / 定稿版
   - whether user-provided materials must be integrated
   - whether the user expects a single markdown deliverable or a long-document split package

2. **Search before writing**
   Use web search before drafting any new long-form content.
   - Search both Chinese and English keywords when useful.
   - Prioritize official sources, primary materials, standards, academic databases or publishers, government releases, reputable media, and domain authorities.
   - Prefer recent sources for unstable topics.
   - If the user uploaded files or provided source text, read and integrate them before drafting.
   - When facts may have changed, verify them rather than relying on memory.

3. **Build an evidence map**
   Before writing, identify:
   - core definitions and scope boundaries
   - key facts, data, dates, institutions, and terminology
   - major viewpoints and counterarguments
   - unresolved uncertainties or evidence gaps
   - sources suitable for direct support versus contextual background

4. **Choose the correct writing lane**
   **Academic / thesis-style** → use formal research framing, question awareness, literature positioning, method or evidence section, analysis, conclusion, and references.
   **Report / briefing** → foreground problem statement, findings, analysis, implications, recommendations.
   **Article / feature / commentary** → foreground narrative flow, argument progression, scene or issue framing, and synthesis.
   **News / explanatory reporting** → foreground timeliness, verified facts, attribution, and separation of reporting from commentary.

5. **Draft at the requested level**
   - **提纲版**: deliver a dense, usable outline with argument logic, section purposes, evidence suggestions, and likely citations.
   - **初稿版**: deliver a full draft with explicit placeholders or limited caveats where evidence remains incomplete.
   - **定稿版**: deliver a polished final version with tightened structure, strong transitions, source-grounded claims, and clean references.

6. **Apply markdown delivery rules**
   Follow [references/markdown_delivery_rules.md](references/markdown_delivery_rules.md).
   - Final deliverables must be actual `.md` files rather than only pasted chat text.
   - Default to a single markdown file for normal-length outputs.
   - If long-document splitting may apply, use the thresholds and naming rules from that reference file rather than redefining them ad hoc.

7. **Run a quality pass before finalizing**
   Check the final output against [references/acceptance_checklist.md](references/acceptance_checklist.md).

## Resource map

Read these files only when needed:

- [references/markdown_delivery_rules.md](references/markdown_delivery_rules.md): long-document split rules and file naming
- [references/acceptance_checklist.md](references/acceptance_checklist.md): final validation rubric
- [references/genre_templates.md](references/genre_templates.md): adaptable structure scaffolds
- [references/gbt7714_quick_guide.md](references/gbt7714_quick_guide.md): quick reference reminder
- [example/index.md](example/index.md): example navigation, including minimal and boundary-case samples

## Evidence and search rules

### Recency rules
Use these defaults unless the subject is historical or the user specifies otherwise.
- 编程、技术、平台、软件、工具：优先近 12 个月
- 制度、政策、行业动态、市场数据：优先近 6-12 个月
- 概念、理论、学术经典：可使用较长期来源，但要区分经典文献与最新研究
- 历史、人文、思想史：以原始材料和权威研究为主，不受近期限制

### Source hierarchy
Prefer sources in this order when available:
1. 官方原始材料、标准、法规、统计公报、官方数据库
2. 学术论文、出版社书籍、研究机构报告
3. 专业协会、行业白皮书、权威机构发布
4. 高信誉媒体、专业访谈、公开演讲实录
5. 一般性媒体与二手综述

### Attribution rules
- Do not present contested or time-sensitive claims without attribution.
- Separate established facts from interpretation, inference, and normative judgment.
- When sources disagree, say so explicitly and characterize the disagreement fairly.
- Do not invent data, citations, quotations, page numbers, institutions, survey results, or bibliography entries.
- If the evidence is thin, narrow the claim instead of overstating certainty.

## Writing standards

### What to optimize for
- 教科书式清晰度，而不是空泛堆砌
- 研究型论证，而不是口号式结论
- 完整段落推进，而不是只有要点罗列
- 有背景、有原理、有方法、有分析、有局限
- 让读者看见“为什么成立”，而不只看见“是什么”

### Disallowed style patterns
Avoid these failure modes:
- 空泛开场，如“随着时代发展”一类套话
- 没有论证支撑的宏大判断
- 反复改写同一意思制造篇幅
- 没有上下文的代码、概念、名词堆砌
- “显而易见”“不言自明”“这里不再展开”等偷省表达
- 未区分事实、分析、建议、价值判断

### Paragraph expectations
For substantive sections, prefer developed paragraphs that include:
1. a clear claim or topic sentence
2. explanation or mechanism
3. evidence, example, or citation support
4. significance, limitation, or transition

## Output level rules

### 1) 提纲版
Use when the user is exploring, planning, or requesting a skeleton first.

Deliver:
- 标题或备选标题
- 写作目的与中心论点/研究问题
- 一级、二级结构
- 每节的核心内容说明
- 关键证据、案例、数据建议
- 可能的争议点、反驳点、风险点
- 参考文献或资料类型建议

A 提纲版 must already show logic and evidence planning, not just headings.

### 2) 初稿版
Use when the user wants a full working manuscript that can still be refined.

Deliver:
- 完整正文
- 必要的小标题
- 关键论证基本成型
- 对证据不足之处进行透明标注或审慎措辞
- 结尾给出简短“建议补强项” only if needed

### 3) 定稿版
Use when the user wants a polished, submission-ready or publication-ready text.

Deliver:
- 完整、连贯、可直接使用的正文
- 自然过渡与收束
- 精炼措辞，减少冗余
- 明确引用与参考资料列表
- 不再留下明显占位符或待补项，除非用户提供的信息本身不足

## Genre playbooks

## Academic thesis / paper
Use this lane for 硕士论文级报告、课程论文、研究论文、文献综述、学术型文章.

Default structure:
1. 标题
2. 摘要
3. 关键词
4. 引言 / 问题提出
5. 文献综述 / 理论背景
6. 研究问题、分析框架或方法说明
7. 主体分析（分章节）
8. 讨论（意义、局限、争议）
9. 结论
10. 参考文献

Requirements:
- Define the research object and scope early.
- Position the topic relative to existing views or literature.
- Explain why the chosen framework, materials, cases, or method are appropriate.
- Distinguish between materials, methods, findings, and interpretation.
- Use a restrained, formal tone.

## Research / industry / policy report
Use this lane for 行业分析、政策研究、公司/机构内部报告、专题研判.

Default structure:
1. 标题
2. 摘要 / 执行摘要
3. 背景与问题定义
4. 现状与关键事实
5. 结构性原因或驱动因素
6. 核心分析
7. 风险与不确定性
8. 结论
9. 建议 / 对策（if applicable）
10. 参考资料

Requirements:
- Lead with the decision-relevant problem.
- Surface evidence quickly.
- Distinguish observation from recommendation.
- Include trade-offs, risks, and implementation constraints.

## Long-form article / commentary / feature
Use this lane for 深度文章、专题文、述评、评论、杂志式长文、人物或议题特稿.

Default structure:
1. 标题
2. 导语 / 问题切入
3. 背景铺垫
4. 主体分析或叙事推进
5. 不同观点与张力
6. 深层含义 / 现实影响
7. 结尾收束
8. 资料来源（if requested or needed for credibility)

Requirements:
- Build rhythm and readability, not just information density.
- Use scenes, examples, contrasts, or case fragments when appropriate.
- Preserve argument discipline even in more literary prose.
- Avoid melodrama and unsupported judgment.

## News / explanatory report
Use this lane for 新闻报道、解释性报道、事实核查式写作.

Default structure:
1. 标题
2. 导语（who, what, when, where, why it matters）
3. 关键信息与背景
4. 多方说法与归因
5. 数据、文件、现场或历史背景
6. 影响与后续观察点

Requirements:
- Verify dates, names, institutions, and sequences of events.
- Attribute every non-obvious factual claim.
- Separate reported facts from analysis and opinion.
- Prefer neutral, precise language.

## Citation rules

The default citation style is **GB/T 7714**.

### In-text handling
- When the user wants a readable article or report, use smooth正文 + 文末“参考资料/参考文献”组合。
- When the user wants stronger学术感, use bracketed references such as `[1]` aligned to the reference list.
- Keep reference numbering stable throughout a single response and across split chapter files.

### Reference list expectations
For each entry, include as much reliable metadata as available:
- 作者/机构
- 文献名
- 文献类型标识（when appropriate）
- 出版者/来源
- 年份
- 获取路径或发布日期（when relevant and available)

Never fabricate missing bibliographic details. If metadata is incomplete, use a conservative partial reference rather than inventing details.

## Handling user materials

If the user provides notes, PDFs, links, interview transcripts, draft fragments, or uploaded files:
- extract the usable claims, facts, quotations, and structure
- preserve the user’s non-negotiable points
- reconcile contradictions where possible
- clearly mark unresolved conflicts or missing evidence
- integrate source materials into the final structure instead of merely appending summaries

## Default response architecture

When no explicit format is given, produce output in this order:
1. 标题
2. 正文主体
3. 参考文献 / 参考资料

When the user asks for 提纲版, produce output in this order:
1. 题目
2. 写作目标与中心问题
3. 结构提纲
4. 证据与资料计划
5. 风险点与补强建议

When creating files, map the structure above into markdown files rather than non-file chat output.

## Fit guidance

### Good fit

Use this skill when the user needs:
- substantial Chinese prose with a visible structure
- evidence-grounded long-form writing or rewriting
- an outline, draft, or final manuscript in markdown
- source-backed commentary, reporting, or analysis
- chapter-split markdown delivery for long documents

### Poor fit

Do not rely on this skill for:
- short casual chat replies
- pure translation with no research or restructuring
- lightweight copy edits on a few sentences
- tasks where the user wants raw bullet notes rather than a shaped manuscript
- non-Chinese deliverables

## Quality checklist

Before finishing, verify all of the following:
- the genre matches the user’s request
- the output level matches 提纲版 / 初稿版 / 定稿版
- the prose is Chinese throughout
- the article has a visible thesis, problem, or reporting focus
- major claims are supported or cautiously framed
- section order is logical
- transitions do real argumentative work
- no obvious AI filler remains
- references are present when evidence mattered
- markdown files are complete, correctly ordered, and mutually consistent

## Escalation rules

- If the topic is too broad, narrow it to a workable claim instead of drifting into shallow generalities.
- If the evidence base is weak, say what can be responsibly concluded and what cannot.
- If the user asks for an extremely long document, prioritize a strong structure and the highest-value sections first rather than padding, then apply the long-document markdown split rules.
- If the user asks for a specific institutional format, follow it over the defaults above.
