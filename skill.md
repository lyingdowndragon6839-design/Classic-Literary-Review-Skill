---
name: classic-literary-review-agent
description: >-
  Agentic Chinese literary review writing system for classic books. Use when
  the user asks to write, revise, humanize, review, or build a Chinese reading
  response or literary long-form essay about a classic literary work,
  especially when internet research, style learning, multi-round revision,
  anti-AI-trace editing, or editor-style critique is required.
---

# Classic Literary Review Agent

## Loading Order

触发此 Skill 时，按任务加载对应文件：

1. [modules/system.md](modules/system.md)
2. [workflow.md](workflow.md)
3. [usage.md](usage.md) — 用户需要使用指导时
4. [modules/decision-tree.md](modules/decision-tree.md) — 请求不完整时
5. [modules/prompt-library.md](modules/prompt-library.md) — 用户需要可复制的提示词时
6. [modules/research.md](modules/research.md) — 允许联网搜索时
7. [modules/prompt-learning.md](modules/prompt-learning.md) — 学习公开 prompt 仓库时
8. [modules/style-learning.md](modules/style-learning.md)
9. [modules/outline.md](modules/outline.md)
10. [modules/writing.md](modules/writing.md)
11. [modules/revision.md](modules/revision.md)
12. [modules/humanization.md](modules/humanization.md)
13. [modules/ai-check.md](modules/ai-check.md)
14. [modules/reviewer.md](modules/reviewer.md)
15. [quality-check.md](quality-check.md)

当目标作品与已有示例匹配或接近时，只读 [examples/](examples/) 中的对应文件。

## Core Rule

如果可以联网：

- 先搜索再写
- 不凭记忆草稿
- 产出 Research Summary、Style Learning Summary、Main Judgment、Outline、
  Draft、Reviewer Notes、Revision Report、AI Check Report、Final Essay

如果不能联网：

- 按 [docs/offline-mode.md](docs/offline-mode.md) 执行
- 标记所有主张为"未检索"
- 不编造来源 URL 或外部共识

## Non-Negotiables

- 联网时至少阅读 20 篇外部文章再动笔
- 学习写法，不学习句子
- 不复制、改写、拼贴或过度模仿单一来源
- 剧情总结不超过最终文章的 20%
- 围绕一个主判断构建全文
- 执行 [modules/humanization.md](modules/humanization.md) 中的降 AI 味流程
- 最终交付前完成 AI 痕迹改写
- 运行 Reviewer Agent 直到没有明显的结构问题
