# Phase 3 census: State hospital association service arms (notes)
Date checked: 2026-09-24. CSV: /home/user/ktodi2/output/work/phase3/assoc.csv (58 rows: one per state (50) plus TORCH/TMSI, Iroquois/UISS, HASC/AllHealth, Hospital Council N&C/California Hospital Share, APS (KS+MO), NRHP, AES (operator), NRHA Services Corp).
Priority counts: A 24, B 16, C 18.

## Load-bearing re-verifications (fresh fetch 2026-09-24)
- SD: enterprises.sdaho.org/endorsed-partners lists only AblePay, Jackson Physician Search, Medical Solutions, SUNRx. CONFIRMED: no CorroHealth. Caveat: SDAHO posted "Meet CorroHealth: A SDAHO Enterprises Endorsed Business Partner you should know" on 2025-07-01 (https://sdaho.org/tag/corrohealth/), so the drop is recent or the page is stale. Confirm before relying on it.
- IN: partners.ihaconnect.org/_corrohealth: "SERVICES ENDORSED by IHA: Price transparency products and/or services". CONFIRMED.
- KS: kha-net.org KHSC CorroHealth page: "PARAREV, a CorroHealth Company: Price Transparency Solution" (text dates from the 2021 CMS mandate). CONFIRMED price transparency only.
- IA: PARTLY CONFIRMED. The page slug is price-transparency, but the heading is "Reimbursement, Pricing, Coding & Contract Management" and the text says CorroHealth helps with "pricing, coding, reimbursement and compliance". The scope is wider than price transparency, though it does not name denials. ServiShare's services list has no denials category.
- MT: mtha.org MHA Ventures endorsed services: "CorroHealth (formerly ParaRev) | Financial Viability | Revenue cycle management & Price Transparency compliance" (contact Greg Goodale). CONFIRMED. Exa shows the page as published 2025-08-28; Phase 1 cited 2026-05-26.
- WA: WHS Preferred Partners PDF (Jul 2025): Operations and Revenue = Commerce Healthcare (AP), ERA, HSC (enrollment/credentialing), Stericycle, SunRX. No RCM or denials partner. "We only choose one partner per service". CONFIRMED.
- TN: THA Innovative Solutions: "$25,000 plus a revenue share", $6,250 quarterly, "we do not engage competitors of our endorsed partners", 3-6 months, 100+ applications per year with ~2% acceptance, quarterly board, "Access to 160+ THA member hospitals"; the page also cites 57 rural hospitals. The partner list has no denials category. CONFIRMED.

## New findings this pass
- Idaho VENTURES lists Ovation Healthcare under "Revenue Cycle Management Solutions" (https://teamiha.org/partner-category/revenue-cycle-operations-management/). Ovation is a known competitor, so ID risk is now high (it was "unknown" in Phase 1).
- Massachusetts HHA named Pivotal Health its preferred IDR partner on 2026-09-24 (75+ hospitals). The AES Healthcare Association Coalition made Pivotal its exclusive IDR partner in Aug 2026. This is adjacent to denials, not appeals writing.
- Rhode Island (missing from Phase 1): HARI has an affiliate membership only. It lists 15 member hospitals and has 0 CAHs.
- Iroquois 2026 Business Associate tiers are $1,000, $5,000 and $10,000. Membership "does not indicate endorsement" (2026 PDF).
- The NRHA partner program already includes TruBridge (Founding Partner) and InlandRCM (denial resolution). The program is non-exclusive.

## CAH counts
All from Flex Monitoring Team Table 1, 2024 data (Apr 2026 report). CT, DE, MD, NJ and RI are absent from the table (0 CAHs). FMT counts only CAHs with a cost report of at least 360 days, so these are lower bounds.

## Searches run (beyond Phase 1 files C, D, H)
1. FMT CAH Table 1 (Exa fetch; direct curl was blocked by the proxy)
2. Fetch: SDAHO endorsed partners; MHA Ventures endorsed services; WHS preferred partners page + PDF
3. Fetch: ServiShare price transparency; KHSC CorroHealth; IHA CorroHealth
4. Fetch: THA IS become-a-partner + partners list
5. "Hospital Association of Rhode Island corporate partners or endorsed vendor program subsidiary"; "HARI affiliate membership member hospitals"
6. Fetch nrhasc.com/meet-your-partners + nrhapartners.com; search "NRHA Services Corporation rural hospital partner revenue cycle denials"
7. "hospital association endorsed partner announcement 2026 denial management appeals AI platform exclusive endorsement"
8. "Kansas Health Service Corporation KHSC endorsed vendors list 2026 revenue cycle"
9. "ServiShare Iowa Hospital Association endorsed partners revenue cycle denials 2026"
10. "Iroquois Healthcare Association 2026 business associate partner revenue cycle"
11. Fetch AES association-solutions (client list)
12. "Healthcare Business Ventures Idaho Hospital Association endorsed partner revenue cycle"
13. "Wyoming Hospital Association WHA Resources endorsed partner revenue cycle 2025 2026"

## Universe enumerated
There is one primary association or service arm for each of the 50 states (see the CSV). Regional and other extras were considered:
- Included: TORCH/TMSI, Iroquois/UISS, HASC/AllHealth, Hospital Council N&C/California Hospital Share, APS, NRHP, AES, NRHA SC.
- Not given rows: Suburban Hospital Alliance of NY (NSHC/NorMet; AES-run, urban); DFW Hospital Council and South Florida HHA (AES coalition, urban); ACHD and CCAHN (California; better placed under district/network types); Mississippi Healthcare Collaborative (525+ orgs; its program is unverified, so it should be checked under networks); Capstone Health Alliance (NC; a GPO/network type); Great Plains Health Alliance (a network type).

## Dropped / caveats
- MS Healthcare Collaborative: dropped. There was no vendor-program evidence, and it is not an association service arm.
- The MD MHA Prime endorsed names, IL IHA strategic partner list and WY vendor list (image-only) are still NOT_FOUND.
- The OH corporate partner directory is paginated, so the full RCM filter was not read.

## People seen on official pages (for Phase 4)
name | org | title | source URL | date
- Ed Phippen | Washington Hospital Services | President | https://wahospitalservices.com/wp-content/uploads/2025/07/WHS-Preferred-Partners.pdf | 2025-07
- Greg Goodale | CorroHealth (vendor contact on MT and IN pages) | SVP of Provider Contract Management and Pricing Technology | https://partners.ihaconnect.org/_corrohealth | seen 2026-09-24
- Kathleen Livingston | Indiana Hospital Association | Director, Member Solutions | https://partners.ihaconnect.org/_corrohealth | seen 2026-09-24
- Sean Becker | MHA Ventures (MT) | listed contact (3RNET row); title not on page | https://mtha.org/business-solutions/mha-ventures-inc/endorsed-services | seen 2026-09-24
- Steve Poage | KHSC/KHA | KHSC vendor contact | https://www.kha-net.org/Communications/CurrentReportPDFs/d175773.aspx?type=view | undated
- Ariel Jenkinson | Healthcare Business Ventures (ID) | Executive Director | https://teamiha.org/hospital-services/ventures/ | seen 2026-09-24
- Michael Sroczynski | Hospital Association of Rhode Island | President | https://www.hari.org/news/five-questions-with-michael-sroczynski | 2026-03-31
- Nicole Casey | Iroquois Healthcare Association | Director of Human Resources | https://iroquois.org/upstate-works/ | seen 2026-09-24
- Matthew Bobo | AES | Vice President (administers Healthcare Association Coalition) | https://www.financialcontent.com/article/bizwire-2026-8-20-pivotal-health-partnership-brings-idr-expertise-to-more-than-350-hospitals-nationwide | 2026-08-20
- Dan McHale | Massachusetts HHA | SVP Healthcare Finance & Policy | https://www.financialcontent.com/article/bizwire-2026-9-24-massachusetts-health-and-hospital-association-selects-pivotal-health-as-strategic-idr-business-partner | 2026-09-24
- Anne Brandner (SVP), Matt Graves (AVP Business Development) | THA Innovative Solutions | https://thainnovativesolutions.com/about/ | seen 2026-09-24 (Phase 1)
- The other people are carried from the Phase 1 C and D "Named people seen" tables (e.g. Tina Creel AR, Jody Fleming NC, Lara Hewitt SC, Matt Archer WV, Jeffrey Austin ME, Joe Tibbs PA, Al Campanella NY, Brian Stevens AES, Leigh Ann Larson WI, Russell Bishop TMSI, Blayne Osborn NRHP, Kevin Bridwell LA, Shellie Whitaker GA).
