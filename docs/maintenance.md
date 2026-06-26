# Maintenance Guide

这个文件给维护者使用。新增内容时先判断它是否真的改进写作流程，
而不是让仓库显得更庞大。

## Adding A New Example

Use [assets/templates/example-case.md](../assets/templates/example-case.md).

Required sections:

- 作品简介
- 主判断
- 写作思路
- 文章框架
- 开头示例
- 正文示例
- 结尾示例
- 为什么这样写
- 修改过程
- 最终版本

## Updating The Workflow

Update these files together when the core workflow changes:

| File | Why |
|---|---|
| [workflow.md](../workflow.md) | Public workflow overview |
| [skill.md](../skill.md) | Loading order and required modules |
| [quality-check.md](../quality-check.md) | Delivery and repository audit checklist |
| [README.md](../README.md) | First-reader navigation |
| [modules/decision-tree.md](../modules/decision-tree.md) | Routing behavior |
| [modules/prompt-library.md](../modules/prompt-library.md) | Copyable prompts |

## Style Consistency

- Use tables for protocols.
- Use Mermaid for process diagrams.
- Use callouts sparingly and only for hard rules.
- Keep modules actionable.
- Avoid long motivational prose.
- Keep filenames exactly as linked in README. Case matters on GitHub.

## Release Checklist

- [ ] File names use lowercase kebab-case, except GitHub standard files.
- [ ] Links pass local audit.
- [ ] README, examples index, and module index are current.
- [ ] `changelog.md` records the change.
- [ ] `git status --short` only shows intended files.
