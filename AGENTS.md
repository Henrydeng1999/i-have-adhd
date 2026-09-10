# Henry Focus repository guide

This repository is Henry Focus, a fork and adaptation of [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd). Preserve the original MIT License, attribution, and multi-platform compatibility files.

## Source of truth

1. `skills/henry-focus/SKILL.md` is the canonical Henry Focus behavior.
2. `.codex-plugin/plugin.json` and `.agents/plugins/marketplace.json` are the canonical Codex plugin entry points.
3. `skills/i-have-adhd/` and the existing platform adapters are retained for upstream compatibility.
4. New Codex documentation and examples should use `$henry-focus`.

## Change rules

- Keep the plugin name, marketplace name, skill directory, repository URL, and install command consistent.
- Do not delete an upstream adapter merely because Codex does not use it.
- Preserve evidence boundaries in research examples and evals.
- Preserve the requested style of formal artifacts.

## Verification

```bash
python -m unittest discover -s tests -v
python -m json.tool .codex-plugin/plugin.json >/dev/null
python -m json.tool .agents/plugins/marketplace.json >/dev/null
```

Confirm that `skills/henry-focus/SKILL.md` has valid YAML frontmatter and that the Codex install command remains:

```bash
codex plugin marketplace add Henrydeng1999/i-have-adhd --ref main
codex plugin add henry-focus@henry-focus
```
