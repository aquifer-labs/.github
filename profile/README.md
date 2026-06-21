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
  retrieval (~1 k tokens/query), optional master·worker·judge orchestration, and self‑repair
  across context compaction. Apache‑2.0.
- **[ocf](https://github.com/aquifer-labs/ocf)** — *Open Cognitive Format.* A portable snapshot of
  what an agent holds in force right now — bounded committed working state + a qualify log — so any
  runtime can **resume** rather than re‑retrieve. Composes with PAM / AMP / files; **artesian** is
  the reference implementation. CC‑BY‑4.0 / Apache‑2.0.

## Principles

`memory control` · `non‑intrusive` · `MCP‑first` · `Rust` · `pluggable backends` · `open (Apache‑2.0)`

> Use as little or as much as you want: just retrieval, or the full agent loop with a qualify gate.
