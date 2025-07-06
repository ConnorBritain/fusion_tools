# Fusion Theme for Obsidian

A two‑tone light/dark skin that layers Fusion Health’s blue–orange palette on top of **kepano’s Minimal** base theme.

> **Why a separate README?**\
> Obsidian themes aren’t packaged like VS Code. They’re just a folder you drop into your vault — and because we *inherit* from Minimal, there are a couple of gotchas you’ll want to get right.

---

## 📦 What’s in the folder

```
obsidian/
└─ Fusion/               #  <‑‑ Folder name must be exactly "Fusion"
   ├─ manifest.json       # No "id" field, just   "name": "Fusion"
   └─ theme.css           # All Fusion colour variables + overrides
```

### Why no `id` in `manifest.json`?

Obsidian looks for a folder whose name **matches **``.  Omitting `"id"` prevents mismatches and keeps the theme selectable in the GUI drop‑down.

---

## 🔧 Prerequisite – install **Minimal**

Fusion re‑uses the Minimal component classes.

1. Open **Settings → Appearance → Themes**
2. Click **Manage** → **Community Themes** → search *Minimal* → **Install & Use**

Once Minimal is present you can safely apply Fusion.

---

## 🖇️ Installation steps

1. **Download / clone** the repo.
2. Copy the `` folder to ``\
   *Mac & Linux example:*\
   `cp -R fusion-themes/obsidian/Fusion "~/vault/.obsidian/themes/Fusion"`
3. In Obsidian: **Settings → Appearance → Themes → Fusion**.
4. Toggle **Base colour scheme** (top of that panel) between *Light* and *Dark* — Fusion adapts to both.

> **Tip for power‑users**\
> If the theme doesn’t appear, open `<vault>/.obsidian/appearance.json` and set\
> `"theme":"Fusion"` manually, then restart Obsidian.

---

## 🔄 Updating the theme

1. Pull or download the latest `theme.css`.
2. Replace the existing file inside `…/themes/Fusion/`.
3. Obsidian hot‑reloads CSS; if not, toggle themes twice or restart.

---

## 🗑️ Uninstalling

Delete the `Fusion` folder from `…/themes/` and switch back to another theme in **Settings → Appearance**.

---

## ❓ Troubleshooting

| Issue                       | Fix                                                                                   |
| --------------------------- | ------------------------------------------------------------------------------------- |
| **Fusion not in drop‑down** | Confirm Minimal is installed **and** the folder is called `Fusion`. Restart Obsidian. |
| **Looks unstyled / raw**    | Minimal missing or outdated → reinstall Minimal.                                      |
| **Still sees old colours**  | Obsidian caches CSS — toggle to a different theme and back, or restart the app.       |

---

© 2025 Connor England   •   MIT Licensed  (see root `LICENSE`)

