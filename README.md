<div align="center">

<img src="icon.png" width="128" height="128" alt="Dark Aether Theme Icon"/>

# Dark Aether Theme

**A dark VS Code theme built around a deep teal palette — easy on the eyes for long sessions.**

[![Version](https://img.shields.io/badge/Version-0.0.6-30b0b6.png?style=flat-square&labelColor=182126)](https://marketplace.visualstudio.com/items?itemName=MechAsh.dark-aether-theme)
[![Marketplace](https://img.shields.io/badge/VS_Marketplace-Install-de9409.png?style=flat-square&labelColor=182126)](https://marketplace.visualstudio.com/items?itemName=MechAsh.dark-aether-theme)
[![License](https://img.shields.io/badge/License-MIT-577c7a.png?style=flat-square&labelColor=182126)](LICENSE)

</div>

---

## ✨ Overview

Dark Aether started as my personal theme — I wanted something dark that wasn't just another clone of One Dark or Dracula. The background (`#182126`) is a deep teal-black that doesn't feel flat, operators stand out in rose-pink, strings sit in olive-gold, and teal covers functions and types. It's been tuned over time to work well across a lot of languages, but honestly the C/C++ support is where it gets specific.

---

## 🎨 Color Palette

| Role | Color | Hex |
|---|---|---|
| **Background** | ![#182126](https://placehold.co/14x14/182126/182126.png) Deep Ocean | `#182126` |
| **Foreground / Text** | ![#b4b9bb](https://placehold.co/14x14/b4b9bb/b4b9bb.png) Silver Mist | `#b4b9bb` |
| **Keywords** | ![#e15763](https://placehold.co/14x14/e15763/e15763.png) Coral Red | `#e15763` |
| **Control Flow** | ![#c25dc4](https://placehold.co/14x14/c25dc4/c25dc4.png) Orchid | `#c25dc4` |
| **Functions** | ![#56b6c2](https://placehold.co/14x14/56b6c2/56b6c2.png) Aether Teal | `#56b6c2` |
| **Types / Classes** | ![#30b0b6](https://placehold.co/14x14/30b0b6/30b0b6.png) Deep Teal | `#30b0b6` |
| **Strings** | ![#aea926](https://placehold.co/14x14/aea926/aea926.png) Olive Gold | `#aea926` |
| **Numbers** | ![#ba73cf](https://placehold.co/14x14/ba73cf/ba73cf.png) Soft Violet | `#ba73cf` |
| **Operators** | ![#DF3775](https://placehold.co/14x14/DF3775/DF3775.png) Deep Rose | `#DF3775` |
| **Variables / Params** | ![#de9409](https://placehold.co/14x14/de9409/de9409.png) Amber | `#de9409` |
| **Preprocessor / Macros** | ![#9d489e](https://placehold.co/14x14/9d489e/9d489e.png) Plum | `#9d489e` |
| **Comments** | ![#577c7a](https://placehold.co/14x14/577c7a/577c7a.png) Muted Sea | `#577c7a` |
| **Cursor** | ![#00ffff](https://placehold.co/14x14/00ffff/00ffff.png) Cyan | `#00ffff` |

---

## 🚀 Installation

### Via VS Code Extension Marketplace (Recommended)

1. Open **VS Code**
2. Press `Ctrl+Shift+X` (or `Cmd+Shift+X` on macOS) to open the Extensions panel
3. Search for **`Dark Aether Theme`**
4. Click **Install**
5. Press `Ctrl+K Ctrl+T` → select **Dark Aether Theme**

### Via Command Line

```bash
code --install-extension MechAsh.dark-aether-theme
```

### Via Marketplace

👉 [Open on Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=MechAsh.dark-aether-theme)

---

## 🖥️ Language Support

Token scopes have been written or adjusted for each of these — it's not just "inherits the default":

| Language | Support Level |
|---|---|
| **C / C++** | ⭐⭐⭐⭐⭐ Full — macros, preprocessor, local/global vars, function types |
| **Python** | ⭐⭐⭐⭐⭐ Full — decorators, self, type hints, builtins |
| **JavaScript / TypeScript** | ⭐⭐⭐⭐⭐ Full — JSX/TSX, template literals, modules, DOM |
| **Rust** | ⭐⭐⭐⭐ Lifetimes, traits, std functions |
| **Go** | ⭐⭐⭐⭐ Operators, package names, goroutine keywords |
| **PHP** | ⭐⭐⭐⭐ Blade templates, heredoc, type hints |
| **Java / C#** | ⭐⭐⭐⭐ Imports, annotations, generics |
| **JSON / YAML** | ⭐⭐⭐⭐ Keys, values, structure |
| **HTML / CSS / SCSS** | ⭐⭐⭐⭐ Tags, selectors, pseudo-classes |
| **Markdown** | ⭐⭐⭐⭐ Headings, bold, italic, inline code, links |
| **SQL, Ruby, Groovy, Haskell, Elm, and more** | ⭐⭐⭐ Good baseline coverage |

---

## 🎨 Design Highlights

### Deep-Ocean Dark Background
`#182126` is the background. It's dark without being pure black, which keeps the colored tokens visible without cranking up their saturation. Works well on both LCD and OLED displays.

### Semantic Differentiation for C/C++
This is the part that took the most time. A lot of themes just throw everything into two or three colors for C. Here, each token type has its own slot:
- `#define` / `#include` directives → **Bold Plum** (`#9d489e`)
- Preprocessor macro names → **Lime Green** (`#7dae59`)
- Global variables → **Amber** (`#bc7c06`)
- Local variables → *italic* **Orange** (`#dd8143`)
- Function definitions → **Olive Green** (`#8daf3d`)
- Function calls → *italic* **Green** (`#59a353`)

### Italic Styling
Comments, local variables, and function calls are italicized. It adds a layer of visual distinction without needing more colors.

### Teal UI Shell
The activity bar, sidebar, status bar, tabs, and terminal all share the same teal-dark palette. Nothing jumps out unexpectedly — the UI stays out of the way of your code.

---

## ⚙️ Recommended Settings

These work well alongside Dark Aether:

```jsonc
{
  // A clean proportional font with good ligature support
  "editor.fontFamily": "'JetBrains Mono', 'Fira Code', 'Cascadia Code', monospace",
  "editor.fontSize": 14,
  "editor.fontLigatures": true,
  "editor.lineHeight": 22,

  // Cursor that pops against the dark background
  "editor.cursorStyle": "line",
  "editor.cursorBlinking": "smooth",

  // Reduce visual noise
  "editor.renderLineHighlight": "gutter",
  "editor.minimap.enabled": false,
  "workbench.colorTheme": "Dark Aether Theme"
}
```

---

## 📋 Changelog

See [CHANGELOG.md](CHANGELOG.md) for version history.

---

## 🛠️ Contributing

Found a language that looks off, or want to add support for something new?

1. Fork the [repository](https://github.com/mechash/dark-aether-theme)
2. Edit `themes/Dark Aether Theme-color-theme.json`
3. Hit **F5** to open an Extension Development Host and test it live
4. Open a Pull Request — describe what you changed and what it fixes

Language-specific token improvements are especially welcome.

---

## 📄 License

[MIT](LICENSE)

---

<div align="center">

Made by **[Ashish Jaiswal (MechAsh)](https://github.com/mechash)**

*Enjoying the theme? A ⭐ on the [Marketplace](https://marketplace.visualstudio.com/items?itemName=MechAsh.dark-aether-theme) goes a long way.*

</div>
