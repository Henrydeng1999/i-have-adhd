# Henry Focus

**ADHD-friendly focus layer for research, coding, debugging, and technical work.**

Henry Focus is not a short-answer mode. It reduces cognitive switching, exposes the important result early, preserves necessary technical depth, makes next actions obvious, and separates facts from interpretation.

> 中文简介：Henry Focus 面向科研、代码、Debug 与复杂任务。它不是单纯压缩回答，而是在保留技术深度和证据边界的同时，降低注意力切换成本。

## Main behavior

- Answer or decision → evidence → action → optional detail
- Coding and debugging → problem → cause → exact fix → verification
- Research → current conclusion → evidence → uncertainty → next test
- Small visible working set, usually 3–5 active points per section
- No invented timing, confidence, probability, or performance claims

## Install in Codex

```bash
codex plugin marketplace add https://gitee.com/Henrydeng1999/i-have-adhd.git --ref main
codex plugin add henry-focus@henry-focus
```

Start a new Codex thread, then invoke:

```text
$henry-focus
```

Examples:

```text
$henry-focus Debug this CUDA out-of-memory error.
$henry-focus Compare these two transient-absorption models.
$henry-focus Turn this implementation plan into bounded steps.
```

## Good fits

- Research interpretation and experiment planning
- Coding, code review, and repository work
- Root-cause debugging
- Technical comparisons and decisions
- Multi-step tasks where resuming context is costly

## Artifact exception

Emails, papers, reports, proposals, slides, formal documentation, social posts, and code comments should follow their own requested style. Henry Focus primarily shapes the surrounding collaboration.

## Compatibility

The original multi-platform files remain in the repository so existing Claude, Gemini, Cursor, OpenCode, Pi, OMP, Qwen, Kimi, and other integrations are not broken. `henry-focus` is the new canonical Codex skill; the old `i-have-adhd` skill remains for upstream compatibility.

## Attribution

Henry Focus is a fork and adaptation of [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd), created by Ayoub Ghriss and contributors. It extends the original idea for research rigor, coding, debugging, evidence boundaries, and complex technical work.

The original MIT License and copyright notice are retained in [LICENSE](./LICENSE).
