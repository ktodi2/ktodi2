# Decisions log

Judgment calls made during the run, logged instead of asking mid-run.

- 2026-09-24: Research is parallelized with subagents, one per partner-type cluster. Each subagent writes a sourced section file under output/work/phase1/; the lead synthesizes 01_landscape.md from those files.
- 2026-09-24: Search stack: Exa (web_search_exa / web_fetch_exa) primary, WebSearch/WebFetch as fallback.
