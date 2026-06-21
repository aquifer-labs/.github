<!-- Aquifer Labs — organization profile -->

# Aquifer Labs

**Open infrastructure for AI‑agent memory control.**

An *aquifer* is where water is stored under pressure and rises without pumping when a well reaches
it — our metaphor for agent context: the right knowledge surfaces automatically, without flooding
the prompt.

## Projects

- **[artesian](https://github.com/aquifer-labs/artesian)** — *memory control for AI agents.* A
  Rust, MCP‑first system that layers a **control plane** over any retrieval store: bounded
  committed context, qualify‑gate, pluggable backends (files / sqlite‑vec / Qdrant), hybrid
  retrieval (~1 k tokens/query), optional master·worker·judge orchestration (wellfield teams),
  autonomous run‑until‑done loops, and self‑repair across context compaction. Apache‑2.0.
  📖 **[Documentation »](https://aquifer-labs.github.io/artesian/)**
- **[ocf](https://github.com/aquifer-labs/ocf)** — *Open Cognitive Format.* A portable snapshot of
  what an agent holds in force right now — bounded committed working state + a qualify log — so any
  runtime can **resume** rather than re‑retrieve. Composes with PAM / AMP / files; **artesian** is
  the reference implementation. CC‑BY‑4.0 / Apache‑2.0.
- **[artesian-zed](https://github.com/aquifer-labs/artesian-zed)** — Zed extension that registers
  Artesian's MCP server as a Zed context server, giving Zed's agent durable, qualify‑gated memory.
- **[homebrew-tap](https://github.com/aquifer-labs/homebrew-tap)** — install Artesian with one line.

## Install

```sh
brew install aquifer-labs/tap/artesian
```

Then follow the **[documentation](https://aquifer-labs.github.io/artesian/)** to wire it into your agent.

## Principles

`memory control` · `non‑intrusive` · `MCP‑first` · `Rust` · `pluggable backends` · `open (Apache‑2.0)`

> Use as little or as much as you want: just retrieval, or the full agent loop with a qualify gate.
