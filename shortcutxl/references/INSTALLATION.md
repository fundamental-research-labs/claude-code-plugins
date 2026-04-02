# ShortcutXL Installation

## Requirements

- **Windows 10/11** with **Excel 2016+** (64-bit)
- **Node.js >= 20**

## Steps

### 1. Open Command Prompt or PowerShell and install Node.js

```bash
winget install OpenJS.NodeJS.LTS
```

### 2. Install ShortcutXL

```bash
npm install -g shortcutxl
```

### 3. Launch ShortcutXL

```bash
shortcut
```

First launch runs an automated setup (Git, Python packages, Excel add-in registration, etc.) and prompts the user to open Excel. After setup, authenticate with `/login` inside the TUI.

**Important:** First launch must be interactive — do NOT run with `-p`. The user must run `shortcut` in a terminal and follow the prompts.
