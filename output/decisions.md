# Decisions log

Judgment calls made during the run, logged instead of asking mid-run.

- 2026-09-24: Research is parallelized with subagents, one per partner-type cluster. Each subagent writes a sourced section file under output/work/phase1/; the lead synthesizes 01_landscape.md from those files.
- 2026-09-24: Search stack: Exa (web_search_exa / web_fetch_exa) primary, WebSearch/WebFetch as fallback.
- 2026-09-24 (Phase 2): Scored 21 partner types 1-5 on reach, trust, fit, speed, cost (unweighted total; a Fit/Trust double-weight check did not change the top 6). Top 6: CPA/advisory; rural networks + hospital-owned co-ops + their group RFPs (merged B1/B3/H2 because they share the same buyer and motion); SORH/Flex; RHTP; association service arms (with AES as the multi-state route); complementary finance-office vendors (patient-pay, cost-report software, coding-only firms).
- 2026-09-24 (Phase 2): EHR partner programs demoted to "ignore for now" because MEDITECH (Claim Denial Agents, Mar 2026) and Oracle Health (appeal management, announced 2026-09-23) launched native appeal drafting. Integration work stays; channel ambition does not.
- 2026-09-24 (Phase 3): Census geography: associations = all 50 states + national/rural extras; SORH/Flex = states with 20+ CAHs or documented revenue-cycle Flex work; RHTP = states whose plans name revenue cycle/denials/back-office tech. Keeps total rows near the 60-150 target.
- 2026-09-24 (Phase 3): competitor_risk and its reason are split into two columns (competitor_risk, competitor_risk_reason) for sorting; montana_or_meditech_tie is "Y: why" or "N".
