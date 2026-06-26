---
name: classic-literary-review-agent
description: Agentic Chinese literary review writing system for classic books. Use when the user asks Codex to write, revise, humanize, review, or build a Chinese reading response or literary long-form essay about a classic literary work, especially when internet research, style learning, multi-round revision, anti-AI-trace editing, or editor-style critique is required.
---

# Classic Literary Review Agent

## Mandatory Loading Order

When this skill triggers, read these files before writing:

1. [SYSTEM.md](SYSTEM.md)
2. [WORKFLOW.md](WORKFLOW.md)
3. [SEARCH.md](SEARCH.md)
4. [GITHUB_PROMPT_LEARNING.md](GITHUB_PROMPT_LEARNING.md)
5. [STYLE_LEARNING.md](STYLE_LEARNING.md)
6. [WRITING.md](WRITING.md)
7. [REVISION.md](REVISION.md)
8. [HUMANIZATION.md](HUMANIZATION.md)
9. [AI_CHECK.md](AI_CHECK.md)
10. [REVIEWER.md](REVIEWER.md)
11. [QUALITY_CHECK.md](QUALITY_CHECK.md)

Read only the relevant example file from [examples/](examples/) when the target work matches or resembles that example.

## Core Rule

If internet access is available, research first. Do not draft from memory. Produce Research Summary, Prompt Design Summary, Style Learning Summary, Main Thesis, Draft, Revision Log, AI Check Report, Reviewer Report, and Final Essay.

If internet access is unavailable, ask whether the user accepts offline mode. If the user accepts, follow [docs/offline_mode.md](docs/offline_mode.md) and mark all claims as non-researched.

## Non-Negotiables

- Read at least 20 external pieces before drafting when online.
- Learn writing moves, not sentences.
- Never copy, paraphrase, patchwork, or imitate a single source too closely.
- Keep plot summary under 20 percent of the final essay.
- Build the essay around one main thesis.
- Run at least eight humanization revision passes.
- Run AI trace rewriting automatically.
- Run Reviewer Agent until no obvious structural problem remains.

