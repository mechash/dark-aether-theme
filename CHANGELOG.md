# Changelog

Changes to Dark Aether Theme, newest first.

---

## [0.0.6] — 2026-04-21

### Changed
- Fixed a handful of typos in token names (`"puntuation"`, `"funcation call"`, `"funcation member"`, `"define and inclued"`) — these were just display names so nothing broke, but still
- Added `galleryBanner`, `homepage`, and better keywords to `package.json` so the Marketplace page doesn't look completely bare
- Rewrote `README.md` — proper color palette table, language support breakdown, recommended settings

---

## [0.0.5] — 2024

### Added
- Proper C/C++ semantic tokens — this took a while to get right. Local variables, global variables, function calls, function definitions, and member functions each get their own color now instead of everything blending together
- `#define` / `#include` directives in Bold Plum (`#9d489e`)
- Preprocessor macro names in Lime Green (`#7dae59`)
- `storage.modifier.specifier` for things like `const`, `volatile`

---

## [0.0.4] — 2024

### Added
- HLSL support — semantic variables, texture/sampler types
- Groovy tokens for imports, methods, variables, and class inheritance
- Elixir symbols

### Changed
- Assignment operators moved to Deep Rose (`#DF3775`) — they were getting lost before

---

## [0.0.3] — 2024

### Added
- Go tokens — assignment, arithmetic, address operators, package names
- SQL variable tokens
- Swift and VB/ASP type support
- INI file default text styling

---

## [0.0.2] — 2024

### Added
- PHP: Blade templates, heredoc/nowdoc, function calls, type hints
- Python: decorators, `self`, function parameters, type hints
- Rust: lifetimes, `std` functions, language variables

### Changed
- Comments are now italic — makes them visually separate without needing a different color
- Numbers switched to Soft Violet (`#ba73cf`)

---

## [0.0.1] — 2024-05-20

### Added
- First release
- Deep-ocean dark background (`#182126`) with teal UI chrome
- Tokens for JavaScript, TypeScript, Python, Java, C#, PHP, CSS/SCSS, Markdown, JSON, and Diff
- Full UI color customization — activity bar, sidebar, status bar, tabs, terminal, panels, widgets
