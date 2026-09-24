# Phase 3 census instructions (for census subagents)

Read /home/user/ktodi2/output/work/RULES.md first (hard rules). Then read the Phase 1 file(s) named in your task:
they already hold sourced candidates. Your job: turn them into a COMPLETE census for your type and geography,
filling gaps with targeted searches (6+ differently worded searches per type, then enumerate the known universe,
then a targeted search for each missing org). Normalize URLs (strip scheme/www/trailing slash) before deduping.
Re-verify any fact you carry over from Phase 1 if it is load-bearing for priority (open a source again if quick).

OUTPUT: a CSV written with Python's csv module (QUOTE_ALL), UTF-8, to the path given in your task, with EXACTLY
these columns in this order:

partner_type,organization,website,hq_state,states_served,est_hospitals_reached,reach_source_url,partner_motion,program_evidence,program_source_url,existing_rcm_or_denials_partner,competitor_risk,competitor_risk_reason,montana_or_meditech_tie,priority,priority_reason,date_checked

Column rules
- partner_type: use the exact label given in your task.
- est_hospitals_reached: a number or range + short basis ("39 CAHs in WA (FMT 2024)"); NOT_FOUND if unknown.
- reach_source_url / program_source_url: a URL that supports that cell. Never blank; NOT_FOUND if none.
- partner_motion: one or more of refer / endorse / resell / integrate / contract / fund, separated by "/".
- program_evidence: short quote (in quotes) or paraphrase of the program, with "per <org>" for self-claims.
- existing_rcm_or_denials_partner: named vendors (sourced in program_evidence or in the reason) or "none found".
- competitor_risk: low / med / high. competitor_risk_reason: why, citing the vendor or product.
- montana_or_meditech_tie: "Y: <why>" or "N". A tie = operates in Montana, involves Glendive Medical Center,
  or has a documented MEDITECH or Oracle Health (Cerner) relationship.
- priority: A / B / C using the rubric below. priority_reason: 1-2 sentences, start with "(judgment)".
- date_checked: 2026-09-24.

Priority rubric
- A = all three: (1) denials/appeals slot open or partner is complementary (competitor_risk low, or med with a clear
  sit-next-to angle); (2) meaningful rural reach (>=15 CAHs or >=20 rural/community hospitals, or a firm/agency
  that touches that many); (3) an active, sourced mechanism Aegis can use now (endorsed program taking applications,
  live RFP, funding line naming revenue cycle/denials, referral/alliance program, or documented revenue cycle
  practice). A Montana/MEDITECH/Oracle tie can lift a borderline B to A.
- B = two of the three.
- C = competitor_risk high with no plausible supplier angle, or no program, or minimal rural reach.

Also write a short companion notes file (same path, .md) listing: searches run, universe enumerated, orgs you
dropped and why, and any people you saw on official pages (name | org | title | source URL | date) for Phase 4.
Final reply to the lead: at most 200 words (counts by priority, top 5 A orgs, surprises).
