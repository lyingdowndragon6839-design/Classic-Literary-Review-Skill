# Search Module

## Rule

Every online writing run begins with search. The Agent must not draft before completing a source pass.

## Source Priority

| Priority | Source Type | Search Intent |
|---:|---|---|
| 1 | 知乎高赞回答 | Find sharp public arguments and reader pain points |
| 2 | 豆瓣长评 | Find long-form reader essays and structural moves |
| 3 | 微信公众号文学评论 | Find polished Chinese essay pacing |
| 4 | B站读书 UP 主文字稿 | Find oral explanation rhythm and audience hooks |
| 5 | 中国知网公开摘要 | Find academic angles without importing jargon |
| 6 | 文学网站评论 | Find specialized criticism |
| 7 | Foreign Literary Review | Find international critical frames |
| 8 | Medium | Find contemporary essay structures |
| 9 | Reddit Books | Find raw reader reactions and debate points |
| 10 | GitHub Prompt Repository | Find agent workflow and prompt design patterns |

## Query Plan

Use Chinese and English queries.

```text
<作品名> 读后感 长评
<作品名> 豆瓣 长评
<作品名> 知乎 高赞 解读
<作品名> 微信公众号 文学评论
<作品名> B站 读书 文稿
<作品名> CNKI 摘要
<English title> literary review
<English title> criticism
<English title> reddit books
```

## Minimum Reading Standard

- Read at least 20 relevant pieces.
- Record title, platform, URL, author if visible, date if visible.
- Separate “what the article argues” from “how the article writes”.
- Do not copy sentences.
- Do not paraphrase distinctive metaphors.
- Do not build the final essay by stitching source viewpoints.

## What To Learn

| Learn | Questions |
|---|---|
| 行文节奏 | Where does the article slow down or accelerate? |
| 思考方式 | What problem does it choose instead of summarizing plot? |
| 段落组织 | How does each paragraph move the argument forward? |
| 观点推进 | What changes between opening, middle, and ending? |
| 修辞方式 | Does it use questions, contrast, repetition, scene return? |
| 结构设计 | Does it begin with detail, conflict, quote, or rereading moment? |
| 转场技巧 | How does it avoid “first, second, third”? |

## Research Summary Template

Use [assets/templates/research_summary.md](assets/templates/research_summary.md).

Required sections:

1. `Search Scope`
2. `Source Table`
3. `Common Angles`
4. `Underused Angles`
5. `Disagreements`
6. `Writing Moves Learned`
7. `Risks To Avoid`
8. `Possible Main Thesis`

## Search Integrity

> [!CAUTION]
> Research is not decoration. If a source was not opened or read, do not count it.

When access is blocked:

- mark `blocked`;
- keep the attempted URL or query;
- replace with another accessible source;
- do not invent the source content.

