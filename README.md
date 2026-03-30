# ShortcutXL Plugin for Claude Code

Control [ShortcutXL](https://shortcut.ai) — an AI-powered Excel agent — from Claude Code.

## Install

```
/plugin marketplace add fundamental-research-labs/claude-code-plugins
/plugin install shortcutxl@shortcut
```

## Sync

Source of truth is `shortcutxl/claude-code-plugin/` in the monorepo. To sync to the published repo:

```bash
cd shortcutxl/claude-code-plugin
rsync -av --exclude='.git' --exclude='README.md' ./ /tmp/claude-code-plugins/
cd /tmp/claude-code-plugins && git add -A && git commit -m "Sync from monorepo" && git push
```
