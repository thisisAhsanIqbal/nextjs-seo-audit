# nextjs-seo-audit

A comprehensive **Agent Skills** collection for SEO auditing. Compatible with [Cursor](https://cursor.com), [Claude Code](https://claude.ai/code), [VS Code](https://code.visualstudio.com), [Gemini CLI](https://geminicli.com), [Roo Code](https://roocode.com), [Amp](https://ampcode.com), and any other [Agent Skills](https://agentskills.io/)-compatible tool.

---

## What is this?

This project contains **11 `SKILL.md` files** that teach AI agents how to perform comprehensive SEO audits on HTML pages. When a user clones this into their project, any compatible AI agent automatically discovers and uses these skills.

**No code to run. No dependencies to install.** The AI agent reads the instructions and performs the audit using its own capabilities.

---

## Skills included

| # | Skill | What it audits |
|---|---|---|
| 🏠 | **Root** ([SKILL.md](SKILL.md)) | Full 10-area audit orchestration, global thresholds |
| 1 | **On-Page** ([SKILL.md](skills/onpage-optimization/SKILL.md)) | Headings, keyword density, internal links |
| 2 | **Schema JSON** ([SKILL.md](skills/schema-json-optimization/SKILL.md)) | JSON-LD validation, Article & LocalBusiness schema |
| 3 | **Meta Data** ([SKILL.md](skills/meta-data-optimization/SKILL.md)) | Title, description, OG, Twitter Cards |
| 4 | **Semantic Layout** ([SKILL.md](skills/semantic-layout/SKILL.md)) | HTML5 elements, ARIA, accessibility, div-soup |
| 5 | **Site Speed** ([SKILL.md](skills/site-speed-optimization/SKILL.md)) | Scripts, stylesheets, inline CSS, images |
| 6 | **Mobile** ([SKILL.md](skills/mobile-optimization/SKILL.md)) | Viewport, responsive design, touch targets |
| 7 | **Backlinks** ([SKILL.md](skills/backlink-monitoring/SKILL.md)) | Dofollow/nofollow, domain diversity, anchor text |
| 8 | **International SEO** ([SKILL.md](skills/international-seo/SKILL.md)) | Hreflang, multi-language, regional targeting |
| 9 | **Technical SEO** ([SKILL.md](skills/technical-seo/SKILL.md)) | Sitemap, robots.txt, canonical, crawlability |
| 10 | **Core Web Vitals** ([SKILL.md](skills/core-web-vitals/SKILL.md)) | LCP, CLS, INP, performance scoring |

---

## How to use

### 1. Clone into your project

```bash
git clone https://github.com/your-username/nextjs-seo-audit.git .agent/skills/nextjs-seo-audit
```

Or add as a Git submodule:

```bash
git submodule add https://github.com/your-username/nextjs-seo-audit.git .agent/skills/nextjs-seo-audit
```

### 2. That's it

Your AI agent will automatically discover the `SKILL.md` files and activate them when you ask SEO-related questions:

- *"Audit this page for SEO issues"*
- *"Check the schema markup on my homepage"*
- *"Is my site mobile-friendly?"*
- *"Optimise the meta tags for this page"*
- *"Run a full SEO audit on index.html"*

### Compatible agents

| Agent | Discovery method |
|---|---|
| **Cursor** | Scans workspace for `SKILL.md` files |
| **Claude Code** | Auto-discovers `SKILL.md` in workspace |
| **VS Code** (Copilot) | Reads `SKILL.md` from workspace |
| **Gemini CLI** | Scans project for skills at startup |
| **Roo Code** | Discovers via workspace root |
| **Amp** | Auto-discovered in workspace |
| **Goose** | Configured skill directories |

---

## Project structure

```
nextjs-seo-audit/
├── SKILL.md                              # Root skill — full audit instructions
├── README.md
├── LICENSE
└── skills/
    ├── onpage-optimization/
    │   └── SKILL.md
    ├── schema-json-optimization/
    │   └── SKILL.md
    ├── meta-data-optimization/
    │   └── SKILL.md
    ├── semantic-layout/
    │   └── SKILL.md
    ├── site-speed-optimization/
    │   └── SKILL.md
    ├── mobile-optimization/
    │   └── SKILL.md
    ├── backlink-monitoring/
    │   └── SKILL.md
    ├── international-seo/
    │   └── SKILL.md
    ├── technical-seo/
    │   └── SKILL.md
    └── core-web-vitals/
        └── SKILL.md
```

---

## How it works

1. Agent discovers `SKILL.md` files at startup and loads metadata (name + description)
2. When a user asks an SEO question, the agent matches it to the relevant skill(s)
3. The agent reads the full `SKILL.md` instructions — which contain exact rules, thresholds, and checklists
4. The agent analyses the HTML using its own capabilities and reports findings as ✅ PASS / ⚠️ WARN / ❌ FAIL

---

## Author

**Muhammad Ahsan Iqbal** — Digital Strategy & SEO Expert

- 🌐 [muhammadahsaniqbal.com](https://muhammadahsaniqbal.com/)
- 💼 [LinkedIn](https://www.linkedin.com/in/ahsan-iqbal-digitalmarketingexpert/)

---

## License

MIT — see [LICENSE](LICENSE)
