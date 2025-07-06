# Changelog

_All notable changes to **Fusion Themes** are documented here. The project follows [Keep a Changelog](https://keepachangelog.com/) and [Semantic Versioning](https://semver.org/)._

---

## [1.1.1] – 2025‑07‑06

### Fusion Dark
- **Error indicators streamlined** – removed thick error/warning _borders_; issues now surface only via subtle gutter glyphs, minimap marks, and overview ruler colours (#FF6B6B / #FFD166).
- **Brand‑orange tab rail** – active, hover, unfocused, and modified states all use `#FE9D26` with graduated opacity for instant context without glare.
- **Callable vs. type clarity** – function & method scopes switch to **Cyan‑Blue `#4FC3F7`**; types/classes sit at **Light Blue `#81C7F5`** for sharper separation.
- **Literal hues refined** – numbers → Mint `#A6D4A0`, strings → Soft Salmon `#E69A87`, constants → Green `#5FD687`; comments remain Muted Blue `#9BB6CF` (italic).

### Fusion Light
- **Full 8‑colour palette refresh** (Dark+ semantics, light‑friendly values):
  | Role | New Hue |
  |------|---------|
  | Language structure | **Orange `#E05D00`** |
  | Functions & callables | **Blue `#2B88D8`** |
  | Types & namespaces | **Periwinkle `#7C4DFF`** |
  | Variables / properties | **Deep Teal `#006064`** |
  | Constants & enum members | **Bold Green `#00855D`** |
  | Numbers | **Vibrant Green `#218041`** |
  | Strings | **Magenta `#B83280`** |
  | Comments / meta | **Blue‑Grey `#6B7A99`** |
- **Selection & cursor contrast** tuned to new palette.

### Shared Improvements
- **Semantic‑token parity** – every TextMate role now mirrors into `semanticTokenColors` for IntelliSense accuracy.
- **Git decorations** aligned to brand palette.
- **Extension metadata** – new 256 × 256 icons, gallery banners, and README files; version bumped to `1.1.1` across VS Code, Cursor, and Windsurf packages.

---

## [1.0.1] – 2025‑05‑12
- Initial public release: Fusion Dark & Fusion Light themes for VS Code 1.50+.

