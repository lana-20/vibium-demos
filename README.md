# 🎬 Vibium Demo Series

> **The definitive hands-on educational resource for [Vibium](https://github.com/VibiumDev/vibium) — browser automation built for the AI era.**

[![YouTube](https://img.shields.io/badge/YouTube-@LanaBegunova-red?style=flat&logo=youtube)](https://www.youtube.com/@LanaBegunova)
[![Vibium](https://img.shields.io/badge/Framework-Vibium-00e5a0?style=flat)](https://github.com/VibiumDev/vibium)
[![Videos](https://img.shields.io/badge/Videos-16%20planned-orange?style=flat&logo=video)](https://lana-20.github.io/vibium-demos/)

---

## What is Vibium?

Vibium is the next evolution in browser automation — built from the ground up for AI agents, humans, and everything in between. Created by **Jason Huggins**, the original author of Selenium and Appium, Vibium answers a simple question: *what would you build if you were designing test automation today, knowing what we know about AI?*

The answer is a single `~10MB` binary that:

- Gives **AI agents a browser** via a built-in MCP server (no wrappers, no glue code)
- Speaks **WebDriver BiDi** — the modern bidirectional WebSocket protocol, not legacy HTTP REST
- Works as a **CLI skill, MCP server, or JS/Python library** — your choice
- Installs in seconds: `npm install vibium` or `pip install vibium`

If Selenium was built for the web era and Appium for mobile, **Vibium is built for the AI era**.

---

## Why This Repo?

The Vibium ecosystem is new and moving fast. Official docs are excellent for reference, but learning from structured, progressive video walkthroughs is how most developers actually absorb a new tool.

This repository is the companion resource to a **16-video YouTube education series** covering everything from zero-to-hello-world to advanced agent automation, accessibility trees, session tracing, and migration from legacy Selenium/Playwright stacks.

Whether you're a QA engineer modernizing your stack, a developer adding browser control to your AI agent, or a tester who's heard the Vibium buzz and wants a guided on-ramp — **you're in the right place**.

---

## 📺 Video Series Overview

| # | Topic | Level |
|---|-------|-------|
| 01 | Intro to Vibium — What is it? Why Vibium? | Overview |
| 02 | Getting Started — JavaScript / TypeScript API | Beginner |
| 03 | Getting Started — Python API | Beginner |
| 04 | Getting Started — MCP — Claude Code | Advanced |
| 05 | Getting Started — MCP — Gemini CLI | Advanced |
| 06 | Agent Setup — Vibium Skill Overview — Automate Browser with CLI/TUI | Agent |
| 07 | Vibium Agent Skill — Main CLI Commands | Agent |
| 08 | Vibium Agent Skill Continued — DOM Query & Mutation with JS Eval | Agent |
| 09 | Vibium Tracer — Browser Session Tracing and Viewing | Feature |
| 10 | WebDriver BiDi — The Standard Behind Vibium | Explainer |
| 11 | Accessibility Tree — Inspect Page a11y Tree in JS & Python | Feature |
| 12 | Browser Window and Viewport Control | Feature |
| 13 | Detect and Save Browser Downloads | Feature |
| 14 | Test Automation Tool Comparison — Parity with Playwright & Selenium | Reference |
| 15 | Legacy Test Suite Transition — Selenium Compatibility Layer | Reference |
| + | Vibium Prompted & Unfiltered: Jason Huggins Answers the Web's Questions | Interview |

📋 **[View the full interactive series index →](https://lana-20.github.io/vibium-demos/)**

---

## 🗂️ Repo Structure

```
vibium-demos/
├── index.html                  # Interactive video series index (GitHub Pages)
├── demos/
│   ├── 01-intro/
│   ├── 02-getting-started-js/
│   ├── 03-getting-started-python/
│   ├── 04-mcp-claude-code/
│   ├── 05-mcp-gemini-cli/
│   ├── 06-agent-setup/
│   ├── 07-cli-commands/
│   ├── 08-dom-query-mutation/
│   ├── 09-tracer/
│   ├── 10-webdriver-bidi/
│   ├── 11-a11y-tree/
│   ├── 12-window-viewport/
│   ├── 13-downloads/
│   ├── 14-playwright-selenium-parity/
│   └── 15-selenium-compat/
└── README.md
```

Each `demos/` folder contains runnable code that mirrors the corresponding video episode.

---

## ⚡ Quick Start

### Install Vibium

```bash
# JavaScript / TypeScript
npm install vibium

# Python
pip install vibium
```

### Hello World (JS)

```js
const { browserSync } = require('vibium')

const vibe = browserSync.launch()
vibe.go('https://example.com')
const title = vibe.eval('document.title')
console.log(title)
vibe.quit()
```

### Hello World (Python)

```python
from vibium import browser

vibe = browser.launch()
vibe.go("https://example.com")
print(vibe.eval("document.title"))
vibe.quit()
```

### Add Browser Control to Claude Code (MCP)

```bash
claude mcp add vibium -- npx -y vibium mcp
# Then just ask: "Go to example.com and click the first link"
```

### Add Browser Control to Gemini CLI (MCP)

```bash
gemini mcp add vibium npx -y vibium mcp
```

---

## 🧭 Learning Path

**New to browser automation?**
Start at Episode 01 → 02 → 03. Build the mental model before touching MCP.

**Experienced with Selenium or Playwright?**
Jump to Episodes 14–15 for the parity and migration guides, then explore the agent-native features.

**Building AI agents?**
Episodes 04–08 are your fast track: MCP setup, the vibe-check CLI skill, DOM manipulation, and agent patterns.

**Curious about the internals?**
Episode 10 (WebDriver BiDi) and Episode 09 (Tracer) give you the protocol-level understanding that makes everything else click.

---

## 🔗 Official Resources

| Resource | Link |
|----------|------|
| Vibium GitHub | [VibiumDev/vibium](https://github.com/VibiumDev/vibium) |
| npm package | [npmjs.com/package/vibium](https://www.npmjs.com/package/vibium) |
| PyPI package | [pypi.org/project/vibium](https://pypi.org/project/vibium/) |
| Getting Started (JS) | [docs/tutorials/getting-started-js.md](https://github.com/VibiumDev/vibium/blob/main/docs/tutorials/getting-started-js.md) |
| Getting Started (Python) | [docs/tutorials/getting-started-python.md](https://github.com/VibiumDev/vibium/blob/main/docs/tutorials/getting-started-python.md) |
| MCP Setup Guide | [docs/tutorials/getting-started-mcp.md](https://github.com/VibiumDev/vibium/blob/main/docs/tutorials/getting-started-mcp.md) |
| WebDriver BiDi Explainer | [docs/explanation/webdriver-bidi.md](https://github.com/VibiumDev/vibium/blob/main/docs/explanation/webdriver-bidi.md) |

---

## 👩‍💻 About the Author

**Lana Begunova** is a QA engineer, automation advocate, and educator focused on making modern testing tools accessible to everyone. This series grew out of hands-on exploration of Vibium from its earliest public releases.

- 📺 [YouTube — @LanaBegunova - Vibium Playlist TBA](https://www.youtube.com/@LanaBegunova)
- 📝 [Medium — @begunova - Women in Technology Author](https://medium.com/@begunova)

---

## 🤝 Contributing

Found a bug in a demo script? Have a better example? PRs and issues are welcome.

If a video helped you, the best thing you can do is **star this repo** and share it with your team. It helps more people find their way to Vibium.

---

*This repository is an independent educational project and is not officially affiliated with VibiumDev.*
