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

## Loading Order

When this skill triggers, read the files that match the task:

1. [modules/system.md](modules/system.md)
2. [workflow.md](workflow.md)
3. [usage.md](usage.md), when the user needs usage guidance
4. [modules/decision-tree.md](modules/decision-tree.md), when the request is incomplete
5. [modules/prompt-library.md](modules/prompt-library.md), when the user needs copyable prompts
6. [modules/research.md](modules/research.md), when internet research is allowed
7. [modules/prompt-learning.md](modules/prompt-learning.md), when studying public prompt repositories is useful
8. [modules/style-learning.md](modules/style-learning.md)
9. [modules/outline.md](modules/outline.md)
10. [modules/writing.md](modules/writing.md)
11. [modules/revision.md](modules/revision.md)
12. [modules/humanization.md](modules/humanization.md)
13. [modules/ai-check.md](modules/ai-check.md)
14. [modules/reviewer.md](modules/reviewer.md)
15. [quality-check.md](quality-check.md)

Read only the relevant file from [examples/](examples/) when the target work matches or closely re
sembles an existing example.

## Core Rule

If internet access is available:

- research first;
- do not draft from memory;
- produce Research Summary, Style Learning Summary, Main Judgment, Outline, Draft, Reviewer Notes, Revision Report, AI Check Report, and Final Essay.

If internet access is unavailable:

- follow [docs/offline-mode.md](docs/offline-mode.md);
- mark claims as non-researched;
- never invent source URLs or external consensus.

## Non-Negotiables

- Read at least 20 external pieces before drafting when online.
- Learn writing moves, not sentences.
- Never copy, paraphrase, patchwork, or imitate a single source too closely.
- Keep plot summary under 20 percent of the final essay.
- Build the essay around one main thesis.
- Run the humanization passes in [modules/humanization.md](modules/humanization.md).
- Run AI trace rewriting before final delivery.
- Run Reviewer Agent until no obvious structural problem remains.
