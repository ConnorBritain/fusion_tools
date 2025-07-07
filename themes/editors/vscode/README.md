# Fusion Health Theme

**One palette – three editors**  
*VS Code · Cursor · Windsurf*

Fusion Health Theme delivers a clinically‑calibrated **dark & light** colour pair.\
Publish it once to the VS Code Marketplace and it works instantly in Cursor and Windsurf (both consume the same extension feed).

Download the theme [here](https://marketplace.visualstudio.com/items?itemName=connorengland.fusion-health).

---

### Previews

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

> **Compatible with VS Code ≥ 1.50, and all Cursor/Windsurf versions.**\
> Cursor & Windsurf read directly from the VS Code Marketplace, so a single listing covers all three.

### 1 · Marketplace *(recommended)*

For easiest installation of the theme, you can access it directly from the [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=connorengland.fusion-health).

Or, from inside your favorite editor, do the following:

1. Press **⌘ Shift X** / **Ctrl Shift X**.
2. Search for **“Fusion Health”** (identifier `connorengland.fusion-health`) and click **Install**.
3. Press **⌘ K T** (*or* **Ctrl K T**) → pick *Fusion Dark* or *Fusion Light*.

### 2 · VSIX sideload

After cloning the repository, navigate to the root directory of the project. The VSIX file should be in the project's root or release directory.

> **Windows Note**: On Windows, VSIX sideloading is the recommended method as manual folder copying does not work reliably. Extensions are automatically unpacked to `%APPDATA%\{Editor}\extensions\` after installation.

For macOS/Linux:

```bash
# one file installs on every editor
VSIX=path/to/fusion-health-1.1.1.vsix  # Update path as needed
code     --install-extension "$VSIX"   # VS Code
cursor   --install-extension "$VSIX"   # Cursor
windsurf --install-extension "$VSIX"   # Windsurf
```

For Windows Command Prompt:

```cmd
:: Use full path with quotes to handle spaces properly
code     --install-extension "C:\path\to\fusion-health-1.1.1.vsix"   
cursor   --install-extension "C:\path\to\fusion-health-1.1.1.vsix"   
windsurf --install-extension "C:\path\to\fusion-health-1.1.1.vsix"   
```

For Windows PowerShell:

```powershell
# IMPORTANT: Use single quotes when setting variable, double quotes when using it
$VSIX = 'C:\path\to\fusion-health-1.1.1.vsix'  # Single quotes for assignment
code     --install-extension "$VSIX"   # Double quotes around variable
cursor   --install-extension "$VSIX"   # Double quotes around variable  
windsurf --install-extension "$VSIX"   # Double quotes around variable
```

**Verify installation**:
```powershell
# Check if extension was installed successfully
windsurf --list-extensions | Select-String fusion
```

### 3 · Manual folder copy *(macOS/Linux only)*

> **Important**: Manual folder copying only works reliably on macOS and Linux. **Windows users should use VSIX sideloading instead** (see method #2 above).

Drop the extension folder into the editor's **extensions directory**. After cloning the repository, use these commands:

| Editor   | macOS / Linux path        |
| -------- | ------------------------- |
| VS Code  | `~/.vscode/extensions/`   |
| Cursor   | `~/.cursor/extensions/`   |
| Windsurf | `~/.windsurf/extensions/` |

```bash
# VS Code on macOS/Linux
cp -r /path/to/fusion_tools/themes/editors/vscode ~/.vscode/extensions/connorengland.fusion-health-1.1.1

# Cursor on macOS/Linux
cp -r /path/to/fusion_tools/themes/editors/vscode ~/.cursor/extensions/connorengland.fusion-health-1.1.1

# Windsurf on macOS/Linux
cp -r /path/to/fusion_tools/themes/editors/vscode ~/.windsurf/extensions/connorengland.fusion-health-1.1.1
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