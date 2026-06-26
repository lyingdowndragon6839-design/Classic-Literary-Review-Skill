# Maintenance Guide

仓库维护者参考。新增内容时先判断它是否真的改进写作流程，
  而不是让仓库显得更庞大。

## Adding A New Example

使用 [assets/templates/example-case.md](../assets/templates/example-case.md) 作为模板。

必须包含的章节：

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

核心流程变更时，同步更新以下文件：

| File | Why |
|---|---|
| [workflow.md](../workflow.md) | Public workflow overview |
| [skill.md](../skill.md) | Loading order and required modules |
| [quality-check.md](../quality-check.md) | Delivery checklist |
| [README.md](../README.md) | First-reader navigation |
| [modules/decision-tree.md](../modules/decision-tree.md) | Routing behavior |
| [modules/prompt-library.md](../modules/prompt-library.md) | Copyable prompts |

## Style Consistency

- 表格用于协议和对照关系
- Mermaid 用于流程图
- 模块保持短小、可执行
- 避免长篇空泛描述
- 文件名保持与 README 中的链接一致

## Release Checklist

发布前逐项确认：

- [ ] 文件名统一使用小写 kebab-case，GitHub 标准文件除外
- [ ] 每个 Markdown 文件只有一个一级标题
- [ ] 标题层级从 `#`、`##`、`###` 逐级展开，不跳级
- [ ] 没有空章节、空文件或单行压缩内容
- [ ] 表格、列表、引用和代码块能正常渲染
- [ ] Mermaid 代码块使用 `mermaid` 语言标记
- [ ] README 链接到的文件全部存在且可访问
- [ ] `examples/` 中每本书有独立文件，格式一致
- [ ] `modules/` 中每个模块各自成文，职责明确
- [ ] 重复内容只出现在必要的模板文件中
- [ ] 语言自然、克制，没有营销或 AI 风格表达
- [ ] `changelog.md` 记录了本次变更
- [ ] `git status --short` 只显示预期的文件
