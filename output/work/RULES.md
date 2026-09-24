# Rules for every research subagent (Aegis channel partner discovery)

Context: Aegis (aegishealth.us, YC-backed) sells an agentic AI platform that writes and files insurance
claim denial appeals for hospitals (~10x faster than in-house, ~10% of in-house cost). Buyers: rural
hospitals, critical access hospitals (CAHs), regional community hospitals. Buyer = CFO; revenue cycle /
PFS / business office directors evaluate. Works inside MEDITECH and Oracle Health (Cerner). Customer
proof: Glendive Medical Center (Montana CAH). Aegis wants channel partners that already hold trusted,
repeated relationships with rural/community hospital finance leaders.

Partner motions: refer (existing model: 15% of first-year revenue per referred hospital), endorse
(association endorsed/preferred vendor list), resell/bundle, integrate/marketplace (EHR/clearinghouse),
contract vehicle (GPO), fund/subsidize (state programs, grants, networks).

Competitor test: if an org sells its own denial-management/appeals product or fully outsourced RCM that
includes denials, competitor_risk = high. Known: Ovation/Amplify RCM, TruBridge, Waystar, MEDHOST, R1
(via Premier), LateralCare (Colorado HA partner), CorroHealth (endorsed by several state assocs). CorroHealth
and AblePay are endorsed in MT, MN, ND, SD.

HARD RULES
1. Every factual claim carries a source URL you actually fetched or saw in search results. No citation, no claim.
2. Keep each fact at the strength of its source. "Per <org>" for self-claims. A logo on a site is not "customer".
   A blog mention of denials is not "runs a denials practice". A LinkedIn snapshot is "per LinkedIn, seen <date>".
3. Never invent names, titles, LinkedIn URLs, emails, numbers. If not found: NOT_FOUND.
4. Mark your own judgment as "(judgment)" / "INFERENCE".
5. READ-ONLY. Never contact anyone, submit forms, sign up, subscribe, request demos, pay, or apply.
   Never touch any CRM/Slack/outreach tool.
6. Never list Jim Merlin (MEDITECH; deceased July 2026). Katrina Holman (one "l") is an Aegis advisor.
7. No em-dashes in any outreach-flavored text.
8. Today is 2026-09-24. Prefer sources from 2025-2026. Flag stale sources with their date.

TOOLS: Prefer Exa tools (mcp__Exa__web_search_exa, mcp__Exa__web_fetch_exa; load via ToolSearch
"select:mcp__Exa__web_search_exa,mcp__Exa__web_fetch_exa"). Fallback: WebSearch / WebFetch (load via ToolSearch).
Run many differently-worded searches. Normalize URLs (strip www, trailing slash) before deduping.
