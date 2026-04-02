# ShortcutXL Plugins

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

Source of truth is `shortcutXL/shortcutxl-plugins/` in the monorepo. To sync to the published repo:

```bash
cd shortcutXL/shortcutxl-plugins
rsync -av --exclude='.git' --exclude='README.md' ./ /Users/pwang/Desktop/WORK/shortcutxl-plugins/
cd /Users/pwang/Desktop/WORK/shortcutxl-plugins && git add -A && git commit -m "Sync from monorepo" && git push
```
