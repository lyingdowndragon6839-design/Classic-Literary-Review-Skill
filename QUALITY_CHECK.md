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

## Markdown Health

- [ ] Mermaid diagrams use valid fenced syntax.
- [ ] Tables render correctly.
- [ ] Relative links point to existing files.
- [ ] No large uninterrupted wall of text dominates a file.
- [ ] Checklists use consistent Markdown.

## Final Self-Check Command Ideas

```powershell
git status --short
Get-ChildItem -Recurse -File | Select-Object FullName
Select-String -Path *.md,docs/*.md,examples/*.md,assets/templates/*.md -Pattern '\\]\\(([^)]+)\\)'
```

