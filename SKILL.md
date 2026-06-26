---
name: classic-literary-review-agent
description: >-
  Agentic Chinese literary review writing system for classic books. Use when
  the user asks Codex to write, revise, humanize, review, or build a Chinese
  reading response or literary long-form essay about a classic literary work,
  especially when internet research, style learning, multi-round revision,
  anti-AI-trace editing, or editor-style critique is required.
---

# Classic Literary Review Agent

## Mandatory Loading Order

When this skill triggers, read these files before writing:

1. [SYSTEM.md](SYSTEM.md)
2. [WORKFLOW.md](WORKFLOW.md)
3. [USAGE.md](USAGE.md) when the user asks how to use the skill,
   provides a reading-response scenario, or needs prompt guidance.
4. [DECISION_TREE.md](DECISION_TREE.md) when the user request is incomplete or
   scenario-specific.
5. [PROMPTS.md](PROMPTS.md) when the user needs prompt examples.
6. [SEARCH.md](SEARCH.md)
7. [GITHUB_PROMPT_LEARNING.md](GITHUB_PROMPT_LEARNING.md)
8. [STYLE_LEARNING.md](STYLE_LEARNING.md)
9. [WRITING.md](WRITING.md)
10. [REVISION.md](REVISION.md)
11. [HUMANIZATION.md](HUMANIZATION.md)
12. [AI_CHECK.md](AI_CHECK.md)
13. [REVIEWER.md](REVIEWER.md)
14. [QUALITY_CHECK.md](QUALITY_CHECK.md)

Read only the relevant example file from [examples/](examples/) when the target work matches or
resembles that example.

## Core Rule

If internet access is available:

- research first;
- do not draft from memory;
- produce Research Summary, Style Learning Summary, Main Judgment, Outline,
  Draft, Reviewer Notes, Revision Report, AI Check Report, and Final Essay.

If internet access is unavailable:

- ask whether the user accepts offline mode;
- follow [docs/offline_mode.md](docs/offline_mode.md);
- mark all claims as non-researched.

## Non-Negotiables

- Read at least 20 external pieces before drafting when online.
- Learn writing moves, not sentences.
- Never copy, paraphrase, patchwork, or imitate a single source too closely.
- Keep plot summary under 20 percent of the final essay.
- Build the essay around one main thesis.
- Run at least eight humanization revision passes.
- Run AI trace rewriting automatically.
- Run Reviewer Agent until no obvious structural problem remains.
