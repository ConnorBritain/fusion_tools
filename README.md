# Fusion Tools

> **A free grab‑bag of Fusion Health utilities, themes, and scripts.** Everything here is MIT‑licensed and intentionally free of proprietary IP.

---

## 🗂️ Directory overview

```
repo‑root/
├─ themes/
│  ├─ editors/
│  │   └─ vscode/           # single Marketplace extension (works in Cursor & Windsurf)
│  └─ notes/                # Obsidian (Minimal‑based) and, soon, Notion
├─ utils/
│  ├─ sql/                  # version‑checkers, driver installers, etc.
│  ├─ data/                 # small open CSV / JSON test fixtures
│  └─ pipelines/            # reusable Airflow / Prefect tasks
├─ docs/                    # longer how‑tos & architecture notes (Markdown)
└─ .github/                 # Actions CI – lint JSON, validate CSS, build .vsix
```

---

## 📚 Sections at a glance

| Folder                  | What lives there                                                     | Status      |
| ----------------------- | -------------------------------------------------------------------- | ----------- |
| `themes/editors/vscode` | **Fusion Health Theme** – dark & light for VS Code, Cursor, Windsurf | **stable**  |
| `themes/notes`          | Obsidian theme (inherits **Minimal**); Notion WIP                    | **active**  |
| `utils/sql`             | PowerShell / Bash / Python scripts → detect ODBC, SNAC, OleDB        | **planned** |
| `utils/pipelines`       | Reusable Python functions for Pandas ↔ Snowflake / Redshift          | **planned** |
| `docs/`                 | Markdown deep‑dives (e.g. “How to debug SNAC”)                       | **open**    |

---

## 🎨 Quick‑start – themes

### VS Code / Cursor / Windsurf

```bash
# Marketplace (recommended)
# 1. Press ⌘⇧X / Ctrl⇧X ➜ search "Fusion Health Theme" ➜ Install

# Sideload via VSIX (all three editors accept the same file)
code     --install-extension fusion-health-theme-1.1.1.vsix  # VS Code
cursor   --install-extension fusion-health-theme-1.1.1.vsix  # Cursor
windsurf --install-extension fusion-health-theme-1.1.1.vsix  # Windsurf
```

### Obsidian

1. Install **Minimal** from Community Themes.
2. Copy `themes/notes/obsidian/Fusion` → `<vault>/.obsidian/themes/`.
3. Settings → Appearance → **Fusion**.

Full instructions live in [`themes/notes/obsidian/README.md`](themes/notes/obsidian/README.md).

---

## 🤝 Contributing

PRs & bug reports welcome! Please keep contributions generic—no internal connection strings or NDA’d snippets.

---

## 🪪 License

© 2025 Connor England / Fusion Health — released under the **MIT License**.

