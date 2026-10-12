<div align="center">

<img src="assets/banner.svg" alt="pendrayg — Claude Code plugin marketplace" width="100%">

### The front door to **pendrayg**'s Claude Code plugins.

A catalogue of Claude Code plugins. Each plugin lives in **its own repo** and updates independently — this repo only carries the `marketplace.json`.

[![plugins](https://img.shields.io/badge/plugins-4-14b8a6?style=for-the-badge)](#-plugins)
[![Claude Code](https://img.shields.io/badge/Claude_Code-marketplace-14b8a6?style=for-the-badge&logo=anthropic&logoColor=white)](https://docs.claude.com/en/docs/claude-code)

```sh
/plugin marketplace add pendrayg/marketplace
/plugin install memory
```

</div>

---

## 🚀 Usage

Add the marketplace once, then install any plugin:

```text
/plugin marketplace add pendrayg/marketplace
/plugin install memory
/plugin install agents
```

Update a plugin (it pulls from its source repo — this catalogue doesn't need to change):

```text
/plugin update memory
```

## 🧩 Plugins

### 🧠 [`memory`](https://github.com/pendrayg/memory) &nbsp; ![v](https://img.shields.io/badge/v0.12.0-8b5cf6?style=flat-square)

Persistent memory for Claude Code in **local SQLite**. Capture via hooks, hybrid **BM25 (FTS5) + semantic** search (sqlite-vec + local transformers.js embeddings, q8), cross-encoder reranking, auto-recall, core memories, doc ingestion, migration from claude-mem. Embedded: zero server, zero daemon, zero cloud.

```text
/plugin install memory
```

### 🤖 [`agents`](https://github.com/pendrayg/agents) &nbsp; ![v](https://img.shields.io/badge/v1.6.0-f59e0b?style=flat-square)

Specialized development agents as skills: `dotnet-developer`, `react-developer`, `nodejs-developer`, `ios-game-developer` (implementation, tests, review, refactoring) and `code-architect` (architecture design through GoF design patterns, ADRs, dev plan).

```text
/plugin install agents
```

### 🔀 [`microsoft-tfs`](https://github.com/pendrayg/microsoft-tfs) &nbsp; ![v](https://img.shields.io/badge/v1.42.0-0078d4?style=flat-square)

On-premise Microsoft TFS MCP server (Node/TypeScript, stdio) — **work items, builds, pull requests, repos, branches, releases** across 42 tools.

```text
/plugin install microsoft-tfs
```

### 📊 [`status-line`](https://github.com/pendrayg/status-line) &nbsp; ![v](https://img.shields.io/badge/v1.1.1-2ea043?style=flat-square)

Powerline status line with green→red gradient gauges for the context window and 5h / 7d rate-limit quotas, plus model, dir and branch. Run `/install-statusline` once to enable (truecolor terminal + node + Nerd Font recommended).

```text
/plugin install status-line
/install-statusline
```

---

<div align="center">

© Yoann Yviquel · Each plugin is independently versioned and MIT-licensed in its own repo.

</div>
