# Upstream relationship

- **Upstream:** https://github.com/Dicklesworthstone/coding_agent_session_search
- **Divergence (as of 2026-07-24):** +3 ahead / -67 behind upstream default branch
- **Fork type:** Contribution/maintenance fork
- **Sync cadence:** Manual; candidate for upstream PR.

## StartupBros-specific delta

Carries an indexer fix: size-gate the pre-rebuild quick_check integrity preflight (fixes a production indexing stall), with regression test.

## Why this file exists

An org-wide audit on 2026-07-24 found that comparing only the *default* branch made
several forks look like zero-delta mirrors when they actually carried unmerged
StartupBros fixes on side branches. Any future fork-pruning pass must enumerate and
author-check **all** branches, not just default-branch ahead/behind.
