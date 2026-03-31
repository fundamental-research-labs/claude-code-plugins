# ShortcutXL Plugin

Control [ShortcutXL](https://shortcut.ai) — an AI-powered Excel agent — from Claude Code or Codex.

## Install

### Claude Code

```
/plugin install shortcutxl
```

### Codex

```
$plugin-installer shortcutxl
```

## Supported Agents

- **Claude Code** — via `.claude-plugin/`
- **Codex** — via `.codex-plugin/`

Both use the same SKILL.md skill definitions.

## Sync

Source of truth is `shortcutXL/claude-code-plugin/` in the monorepo. To sync to the published repo:

```bash
cd shortcutXL/claude-code-plugin
rsync -av --exclude='.git' --exclude='README.md' ./ /path/to/shortcutxl-plugin/
cd /path/to/shortcutxl-plugin && git add -A && git commit -m "Sync from monorepo" && git push
```
