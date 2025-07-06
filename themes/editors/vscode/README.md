# Fusion Health Theme

**One palette – three editors**  *VS Code · Cursor · Windsurf*

Fusion Health Theme delivers a clinically‑calibrated **dark & light** colour pair.\
Publish it once to the VS Code Marketplace and it works instantly in Cursor and Windsurf (both consume the same extension feed).

![Fusion Dark Theme Preview](images/preview-dark.png)
![Fusion Light Theme Preview](images/preview-light.png)

---

## ✨ Highlights

|                                                      | Dark | Light |
| ---------------------------------------------------- | ---- | ----- |
| Hand‑tuned **TextMate & semantic** colours           | ✔    | ✔     |
| Clear separation of keywords, types, functions, data | ✔    | ✔     |
| Ergonomic palette for long C/C++ sessions            | ✔    | ✔     |
| Retina‑ready icon & Marketplace banner               | ✔    | ✔     |

---

## 📦 Installation (all editors)

> **Compatible with VS Code ≥ 1.90, Cursor ≥ 1.90, Windsurf ≥ 1.90.**\
> Cursor & Windsurf read directly from the VS Code Marketplace, so a single listing covers all three.

### 1 · Marketplace *(recommended)*

1. Press **⌘ Shift X** / **Ctrl Shift X**.
2. Search for **“Fusion Health”** (identifier `connorengland.fusion-health`) and click **Install**.
3. Press **⌘ K T** (*or* **Ctrl K T**) → pick *Fusion Dark* or *Fusion Light*.

### 2 · VSIX sideload

```bash
# one file installs on every editor
VSIX=fusion-health-1.1.1.vsix
code     --install-extension $VSIX   # VS Code
cursor   --install-extension $VSIX   # Cursor
windsurf --install-extension $VSIX   # Windsurf
```

### 3 · Manual folder copy *(offline/portable)*

Drop the extension folder into the editor’s **extensions directory**.

| Editor   | macOS / Linux path        | Windows path                          |
| -------- | ------------------------- | ------------------------------------- |
| VS Code  | `~/.vscode/extensions/`   | `%USERPROFILE%\.vscode\extensions\`   |
| Cursor   | `~/.cursor/extensions/`   | `%USERPROFILE%\.cursor\extensions\`   |
| Windsurf | `~/.windsurf/extensions/` | `%USERPROFILE%\.windsurf\extensions\` |

```bash
# example – VS Code on macOS/Linux
EXT=~/.vscode/extensions/connorengland.fusion-health-1.1.1
mkdir -p "$EXT"
# assuming you cloned this repo
cp -R themes/editors/vscode/* "$EXT"
```

Restart the editor → **⌘K T / CtrlK T** → select *Fusion Dark* or *Fusion Light*.

---

## 🔧 Recommended settings snippet

```jsonc
{
  "workbench.colorTheme": "Fusion Dark",
  "editor.fontFamily": "Fira Code, JetBrains Mono, monospace",
  "editor.fontLigatures": true,
  "workbench.colorCustomizations": {
    "editorIndentGuide.activeBackground": "#FE9D26"
  }
}
```

---

## 🖼️ How it looks in other editors

### Cursor
![Fusion Dark in Cursor](images/preview-dark-cursor.png)
![Fusion Light in Cursor](images/preview-light-cursor.png)

### Windsurf
![Fusion Dark in Windsurf](images/preview-dark-windsurf.png)
![Fusion Light in Windsurf](images/preview-light-windsurf.png)

---

## 🛠️ Contributing & scope tweaks

1. Place the cursor on any token.
2. Run **Developer: Inspect Editor Tokens and Scopes**.
3. Open an issue with the scope list + screenshot.

---

## 🗒️ Changelog & licence

See [CHANGELOG.md](../CHANGELOG.md) for release notes.\
Released under the **MIT License** by Fusion Health.

