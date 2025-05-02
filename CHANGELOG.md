# Changelog

All notable changes to dns-lookup are documented here.

### [2025-12-29]
- refactor: simplify token parsing pipeline and reduce cognitive complexity

### [2026-01-13]
- perf: optimize memory allocation in buffer pool

### [2026-01-15]
- fix: resolve memory leak in idle connection reaper

### [2026-02-06]
- perf: minimize redundant heap allocations in hot loop

### [2026-02-13]
- docs: clarify prerequisite installation steps in README

### [2026-03-01]
- feat: add graceful shutdown signal handler (SIGINT/SIGTERM)

### [2026-03-01]
- feat: add support for custom timeout configuration via CLI flags

### [2026-03-03]
- docs: add example configuration commands to quickstart guide

### [2026-03-19]
- test: add fuzzing harness for packet decoding routine

### [2026-04-06]
- fix: resolve memory leak in idle connection reaper

### [2026-04-13]
- test: add fuzzing harness for packet decoding routine

### [2026-04-17]
- feat: improve error logging with contextual debug traces

### [2026-05-29]
- refactor: decouple configuration loader from runtime engine

### [2026-07-16]
- security: harden cryptographic salt generation against entropy dips

### [2026-07-25]
- fix: resolve memory leak in idle connection reaper

### [2026-07-26]
- perf: minimize redundant heap allocations in hot loop

### [2026-07-28]
- fix: handle malformed HTTP header parsing without crashing

### [2026-07-29]
- chore: streamline build flags and compiler optimization settings

### [2026-07-31]
- security: harden cryptographic salt generation against entropy dips

### [2026-08-25]
- feat: add support for custom timeout configuration via CLI flags

