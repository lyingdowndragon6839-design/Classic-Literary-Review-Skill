# Quality Check

## Repository Structure

- [ ] Root documents describe a complete Agent, not a prompt collection.
- [ ] `SKILL.md` exists and has valid frontmatter.
- [ ] Research, learning, writing, revision, AI check, and review modules exist.
- [ ] `examples/` contains at least 10 complete work examples.
- [ ] `docs/` and `assets/` contain reusable support material.

## Workflow Completeness

- [ ] Research -> Learning -> Writing -> Revision -> Review is explicit.
- [ ] Online mode requires search before drafting.
- [ ] Offline mode is documented and cannot fake research.
- [ ] Research Summary is required.
- [ ] Prompt Design Summary is required.
- [ ] Style Banks are required.
- [ ] Reviewer loop is required.

## Writing Quality

- [ ] One central thesis controls the essay.
- [ ] Plot summary stays under 20 percent.
- [ ] The article avoids textbook categories.
- [ ] Every major claim can be tied to textual detail.
- [ ] The ending avoids generic inspiration.

## Humanization

- [ ] Eight revision passes are documented.
- [ ] Template connectors are removed.
- [ ] Paragraph and sentence lengths vary.
- [ ] Reader psychology appears where useful.
- [ ] Observation replaces over-explanation.

## AI Trace

- [ ] Cliche phrases are detected and rewritten.
- [ ] Empty praise is replaced with detail.
- [ ] Mechanical transitions are removed.
- [ ] Repetition is reduced.
- [ ] The article does not sound like a generated essay.

## 读后感提交前检查

- [ ] 是否有明确主判断。
- [ ] 是否不是纯剧情复述。
- [ ] 是否有具体人物或情节支撑。
- [ ] 是否有个人阅读感受。
- [ ] 是否避免了 AI 套话。
- [ ] 是否避免了万能结尾。
- [ ] 是否适合当前提交场景。
- [ ] 是否保留了用户自己的语气。
- [ ] 是否有一两处真正刺人的表达。
- [ ] 是否读起来像一个人写的，而不是模板生成的。

## Markdown Health

- [ ] Mermaid diagrams use valid fenced syntax.
- [ ] Tables render correctly.
- [ ] Relative links point to existing files.
- [ ] No large uninterrupted wall of text dominates a file.
- [ ] Checklists use consistent Markdown.

## Repository Review

- [ ] 所有 Markdown 都不是单行压缩内容。
- [ ] 标题层级清楚，根标题只有一个。
- [ ] 没有空章节。
- [ ] README 中引用的文件与仓库实际文件名一致。
- [ ] 相对路径在 GitHub 中可以打开。
- [ ] Mermaid 代码块使用 `mermaid` 标记。
- [ ] 核心文档之间没有明显内容冲突。
- [ ] 重复内容只保留在必要模板里。
- [ ] Examples 不只是最终文章，至少 5 个案例展示完整流程。
- [ ] README 能让第一次访问的人五分钟内知道怎么使用。
- [ ] PROMPTS.md 能直接复制使用。
- [ ] DECISION_TREE.md 能处理常见用户场景。
- [ ] ROADMAP.md 体现长期维护方向。

## Final Self-Check Command Ideas

```powershell
git status --short
Get-ChildItem -Recurse -File | Select-Object FullName
Select-String -Path *.md,docs/*.md,examples/*.md,assets/templates/*.md -Pattern '\\]\\(([^)]+)\\)'
```
