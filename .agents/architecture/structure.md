# Architecture & Technical Standards — PaperMC

This repository is the standalone `papermc` platform of MCPaimon. It is published
as `io.github.mcpaimon:papermc` and shaded into the runnable `MCAgentsPaperMC`
plugin jar via the Shadow plugin.

## Scope

- Platform-specific implementation that hosts the AI provider on PaperMC servers
  and manages MCExtension plugins.
- Threading rules: see `.agents/platforms/papermc/concurrency.md`.

## Dependencies

Depends on `io.github.mcpaimon:api` and `io.github.mcpaimon:common` using
**static** versions (for example `2026.0.7-8`), plus the relevant
`io.github.mcengine` artifacts. Versions are pinned because each module is
released independently and may diverge.
