# VS Code + GitHub Quick Reference  
_Alpen Confections — Development Setup Guide_

---

## 🧭 Environment Overview
- **Mac Mini (M1)** running macOS 26.0.1  
- **VS Code** (with GitHub extensions)  
- **Python 3.14 (Homebrew)**  
- **GitHub account:** alpenconfections  

---

## 🪄 Essential VS Code Commands

| Task | Shortcut / Command | Notes |
|------|--------------------|-------|
| Open Command Palette | `⌘⇧P` | Access any VS Code command |
| Open Integrated Terminal | `` Ctrl+` `` | Run shell commands inside VS Code |
| Open Source Control | `⌃⇧G` or click Branch icon | Manage commits, branches, push/pull |
| Run Python file | `⌃⌥N` or `Run ▶` button | Executes the active script |
| Format code | `⌥⇧F` | Requires Python extension |
| Install extension (CLI) | `code --install-extension <id>` | Example: `ms-python.python` |

---

## 🧩 Git + GitHub Basics

### Create a Branch
```bash
git checkout -b new-feature
```

### Stage + Commit Changes
```bash
git add .
git commit -m "Describe your change"
```

### Push to GitHub
```bash
git push -u origin new-feature
```

### Merge via Pull Request
- Open the **GitHub Pull Requests** sidebar  
- Click **Create Pull Request** → review → **Merge**

---

## 🤖 Copilot & Actions

### Enable GitHub Copilot
1. Install extensions:  
   - `GitHub.copilot`  
   - `GitHub.copilot-chat`
2. Sign in via the Account icon  
3. Use `⌘I` to trigger inline suggestions

### GitHub Actions
- Sidebar → **Actions** tab → monitor automated workflows  
- YAML files live in `.github/workflows/`

---

## ⚙️ Workspace Tips

| Setting | Purpose |
|----------|----------|
| `autoSave: afterDelay` | Saves files automatically |
| `formatOnSave: true` | Auto-formats on save |
| `terminal.integrated.defaultProfile.osx: "zsh"` | Uses your default shell |
| `python.defaultInterpreterPath` | Should point to `/opt/homebrew/bin/python3` |

---

## 🧁 Recommended Extensions

| Extension | Purpose |
|------------|----------|
| `ms-python.python` | Core Python support |
| `ms-toolsai.jupyter` | Interactive Notebooks |
| `GitHub.vscode-pull-request-github` | Manage PRs in VS Code |
| `GitHub.copilot` + `GitHub.copilot-chat` | AI code assistant |
| `eamodio.gitlens` | Deep Git insights |
| `GitHub.vscode-github-actions` | Manage workflows visually |

---

## 🧠 Quick Troubleshooting

| Issue | Fix |
|--------|------|
| `code` not found in terminal | Run *Shell Command: Install ‘code’ in PATH* |
| Wrong Python version | Check `which python3` → `/opt/homebrew/bin/python3` |
| GitHub login issues | Run `gh auth login` again |
| Push fails | Run `git pull --rebase origin main` and retry |

---

**Version:** 1.0 • Maintained by Lin & Mike ("The Chocolate Boys") 🍫  
**Location:** `/Users/lindsleymckay/VSCode_trusted/alpen_test_repo/VSCode_GitHub_QuickRef.md`
