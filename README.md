# yc-editor

A fast, native macOS editor for structured data — JSON, XML, YAML, and plain text. Built with Tauri 2 (Rust), React 18, and CodeMirror 6.


---

## Download

**[⬇ Download .dmg (macOS)](https://github.com/yashas809/yc-texteditor_dmg)**

Open the `.dmg`, drag yc-editor to your Applications folder, and launch. No install wizard, no account required.

---

## Features

### Structured Data Editing
- **JSON, XML, YAML syntax highlighting** — full CodeMirror 6 language support with bracket matching and auto-indent
- **One-click Format** — pretty-print your file with configurable indent (2 spaces / 4 spaces / Tab)
- **Validate with line/column errors** — know exactly where a parse fails without scanning the whole file
- **Collapsible JSON Tree panel** — live side-by-side visual tree that updates as you type; collapse and expand any node

### General Editor
- Works as a **plain text editor** too — open any file and start typing; structured data features are there when you need them, invisible when you don't
- **Multi-tab editing** — open and switch between multiple files simultaneously with per-tab dirty state tracking
- **Find & Replace** — case-sensitive, whole-word, and cross-document search
- **Word wrap toggle** and **indent width control** (2 / 4 / Tab)
- **Dark and Light theme**
- Status bar — live cursor position, document size, encoding, language selector

### Native & Fast
- Built with **Tauri 2 (Rust)** — uses macOS's built-in WKWebView instead of bundling a Chromium runtime
- Tiny binary, instant cold start, low memory footprint
- All file I/O flows through the Rust layer — the WebView has zero direct filesystem access
- Full offline — no telemetry, no internet connection required

---


## Tech Stack

| Layer | Technology |
|---|---|
| Native shell | Tauri 2 (Rust) |
| UI framework | React 18 |
| Editor engine | CodeMirror 6 |
| File I/O | tauri-plugin-fs + tauri-plugin-dialog |
| Build tool | Vite |

---

## AI-First Repo

This project was built using an **AI-first development methodology**. Rather than using AI to generate boilerplate, the entire workflow is structured around a living knowledge base:

- **`CLAUDE.md`** — a codebase overview that routes Claude to per-feature skill docs before touching any file
- **`.claude/skills/`** — per-feature skill documents covering constraints, state ownership, and architecture decisions
- Every feature branch, refactor, and architectural decision is documented as a first-class artifact

The result is a codebase that is well-documented, constraint-aware, and straightforward to extend — whether by a human or an AI agent.

---

## License

[MIT](LICENSE)
