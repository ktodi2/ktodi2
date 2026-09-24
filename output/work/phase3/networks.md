# Phase 3 census: Rural network / hospital-owned co-op (US)

Date checked: 2026-09-24. CSV: /home/user/ktodi2/output/work/phase3/networks.csv (40 rows: 9 A, 25 B, 6 C).

## Load-bearing re-verifications (fresh fetches 2026-09-24)
1. **Montana Health Network shareholders** (https://montanahealthnetwork.com/about-us): the "Shareholders" section says shareholders "are the owning facilities of Montana Health Network and have representation on the Montana Health Network Board of Directors". It lists "Glendive Medical Center, Glendive, MT" among 17 facilities. CONFIRMED. Staff listed: Chris Hopkins (CEO), Lori Backes (CFO), Ward VanWichen (VP of Strategy). The page lists no RCM or denials program. Program areas are 401(k), case management, education, benefits, insurance, staffing, support services, transportation and workers' comp.
2. **Yellowstone HVN members** (https://yellowstonenetwork.org/networks, published 2025-05-19): lists "Glendive Medical Center, Glendive, Montana" among 24 members. CONFIRMED.
3. **RHE RFPs.** There are two separate RHE RFPs, both from March 2026:
   - (a) The contract compliance / zero balance / underpayment / **denials** / credit balance RFP (https://ruralcollaborative.com/wp-content/uploads/2026/04/RHE-RFP-contract-compliance-denial-mgmt-credit-bal.pdf, author Leslie Hiebert):
     - Section 3.4 "Denial appeals management" covers "Claim review and validation", "Appeal letter preparation", "Submission of appeals", "Tracking payer responses" and "Escalation when necessary".
     - Terms include "RHE master services agreement, inclusive of program support administration fee". Pricing must include "group purchasing pricing based upon RHE volume".
     - Timeline: issued March 17, 2026; proposals due April 3, 2026; "Final Vendor Selection: April 15, 2026"; "Final award determined by negotiated contract terms with RHE". Submissions go through Valify.
   - (b) The Hospital & Clinic Billing/RCM RFP (…Request-For-Proposal-Hospital-and-Clinic-Billing-Services-Final-031926.pdf):
     - "3.5 Denials Management (required offering)" includes "Appeals preparation and submission". It carries the same admin-fee clause.
     - Timeline: issued March 19, 2026; due April 17; finalist presentations April 27-30; "Final Vendor Selection: May 29, 2026". "More than one finalist may be selected".
   - **Award announcement: NOT_FOUND.** I ran two targeted searches for the award, plus the RHE contracts page and the TRC homepage. No winner is named anywhere. (judgment) Both selection dates have passed, so assume both are awarded or in negotiation. Ask RHE directly only through normal channels (read-only here).
   - Related: TRC RHTP page says "$5,430,000" of Washington's 2026 RHTP is "ear-marked for TRC" (https://ruralcollaborative.com/rhtp/). A separate RHTP-funded Revenue Cycle Assessment RFP exists (TRC_RCA_Scope_Outline-FINAL.pdf).
4. **Billings Clinic affiliates** (https://billingsclinic.com/about-us/affiliate-hospitals-clinics): still lists "Glendive Medical Center - Glendive, MT". There are 14 MT affiliates (now including Community Medical Center, Missoula, and Billings Clinic Broadwater) and 5 WY affiliates (Hot Springs Health, North Big Horn, Powell Valley, RiverPeak, Three Rivers). CONFIRMED.

## Searches run (Exa; ~25 searches/fetches this phase, plus Phase 1's ~45)
- RHE award (x2); RHE contracts page; TRC homepage; TRC vendors/RC AI contracts.
- RWHC services; Hospital Cooperative ID; HomeTown Health (+ business partners page).
- Kentucky networks; PA/NY networks; Mississippi/Texas networks.
- PMHA (+ revenue cycle page); MS Rural Hospital Alliance.
- Show-Me HVN; Cibolo Missouri; cibolohealth.com/networks.
- Oregon networks (surfaced Cascades HVN via OHA HCMO filings); Texas co-ops (TORCH CIN, TPC, FirstChoice); Iowa/ND/SD networks.
- Wyoming networks; Michigan CAH networks.
- NRHP (+ RCIP page); Monida MT; ICAHN preferred partners.
- Medi-Sota vendors; WHA brochure; PHV about page; Health Future OR.
- Rural co-op RFPs for revenue cycle/denials 2025-26.

## Universe enumerated
- **(a/b) Networks with hospital members:** TRC/RHE, MHN, WHA, ICAHN, Medi-Sota, PHV, Heartland/Bryan, HomeTown Health, RWHC, Hospital Cooperative, NRHP, PMHA, MS RHA, TORCH CIN, ARHP, InSRHN, Utah Rural 9, NMRHN, Northwest Hospital Alliance, LIHNC, Pioneer Health Network, GPHA, Wilderness Health, UPHCS, Northland, Monida, Eastern Plains, NECHN, NCHN.
- **(c) Hospital-owned shared-service/insurance:** MHN (MT); NRHP also runs LiCON liability co-op.
- **(d) Cibolo HVNs:** Yellowstone MT 24, Rough Rider ND 23, Headwaters MN 17, Ohio 24, Nebraska 19, Wisconsin 10, Kansas 7, Cascades OR 11 (pending OHA review, notice accepted 2026-08-27), Show-Me MO 23. Every one is flagged competitor_risk high because of Cibolo's own denial management services and its TruBridge preferred-RCM deal.
- **(e) Purchasing co-ops running RFPs:** RHE is the only co-op found running a live denials/RCM RFP. Others found were supply-focused only (FirstChoice Cooperative, Health Future, Alliant Purchasing via TORCH).
- **Health system affiliate network:** Billings Clinic-Logan Health (one row, as instructed).

## Thin-state results
- **GA:** HomeTown Health (70+, also FL/AL/MS/IA).
- **KY:** no hospital-member rural co-op found. Kentucky Health Collaborative is 10 large systems (not rural, dropped).
- **PA/NY:** PMHA (13 PA hospitals + 2 NY revenue-cycle affiliates).
- **OR:** Cascades HVN (Cibolo).
- **WY:** no WY-only hospital network. WY hospitals reach through The Hospital Cooperative (Star Valley Health) and Billings Clinic affiliates (5 WY). GPCIN is FQHC-only (dropped).
- **MS:** Rural Hospital Alliance (39, 2021).
- **TX:** TORCH CIN (32).
- **MO:** Show-Me HVN.
- **IA:** no standalone hospital co-op found. HomeTown Health runs Iowa Flex FIRES, which includes denials education (Iowa HHS). UIHC CAH network is a system network.
- **ND/SD:** Rough Rider, Northland. No SD-specific network found.

## Dropped (and why)
- Kentucky Health Collaborative: large systems, not a rural co-op.
- Mississippi Healthcare Collaborative: policy coalition, no shared services found.
- GPCIN (Dakotas): FQHCs only.
- Kentucky Integrated Care: FQHC/RHC CIN.
- MICAH QN (MI, 35 CAHs): quality-only network, no business services.
- TPC (TX/AR): 8 health systems with its own revenue cycle program; minimal rural reach.
- FirstChoice Cooperative and Health Future: supply GPOs, no RCM RFPs found.
- Sunflower Health Network and HINK (KS): stale sources, small.
- Rural Health Collaborative (TruBridge + THMA): competitor forum, not hospital-owned.
- Caravan/Signify: ACO-only (Phase 1).
- Out of type but worth passing to the state-programs census: the Hawaii DOH Office of Primary Care and Rural Health solicitation Q26002840, "Critical Access Hospital Claims Denial Dashboard Design and Impl" (Molokai CAH), posted 2026-05-13, due 2026-05-22 (https://www.govcb.com/government-bids/CRITICAL-ACCESS-HOSPITAL-CLAIMS-AND-23616862.htm).

## Caveats
- **Carried from Phase 1 without a fresh fetch** (fetched the same day in Phase 1): Heartland/Bryan, InSRHN, Utah Rural 9, NMRHN, NWHA, Pioneer, GPHA, Wilderness, UPHCS, Northland, ARHP, NCHN, NECHN.
- **Show-Me HVN and Cibolo:** the tie rests on a local-paper quote from the Hermann CEO (2025-12-03). The MHA release and showmehvn.org do not name a manager.
- **Cibolo total:** ~124 hospitals is INFERENCE (a sum of counts).

## People seen on official pages or press (for Phase 4)
| name | org | title | source URL | date |
|---|---|---|---|---|
| Chris Hopkins | Montana Health Network | CEO | https://montanahealthnetwork.com/about-us | seen 2026-09-24 (undated page) |
| Lori Backes | Montana Health Network | CFO | https://montanahealthnetwork.com/about-us | seen 2026-09-24 |
| Ward VanWichen | Montana Health Network | Vice President of Strategy | https://montanahealthnetwork.com/about-us | seen 2026-09-24 |
| Leslie Hiebert | Rural Health Enterprise | CEO (RFP contact) | https://ruralcollaborative.com/wp-content/uploads/2026/04/RHE-RFP-contract-compliance-denial-mgmt-credit-bal.pdf | 2026-03 |
| Tianna Fallgatter | The Rural Collaborative | Director of Contract Services (2024 release); Director of Business Development (LegalOn case study, undated) | https://ruralcollaborative.com/agile-consulting-group-partners-with-the-rural-collaborative-to-deliver-sales-tax-savings-for-members/ | 2024-04-29 |
| Jennifer Gearman | Medi-Sota | Executive Director | https://medi-sota.org/main/index.php/en/current-vendors/business-office-resources | seen 2026-09-24 |
| Nicole Clawson | Pennsylvania Mountains Healthcare Alliance | VP Revenue Cycle & Finance | https://finthrive.com/lp/customer-story-pmha-video ; http://www.pmhalliance.org/pmha-team | undated |
| Joe DeSimone | PMHA | Director of Business Development and Customer Experience | http://www.pmhalliance.org/pmha-team | undated |
| Sandy Sage, RN | HomeTown Health | Revenue Cycle Analyst (leads RISE) | https://hthu.net/rcmprogram/ | undated |
| Craig Thompson | Show-Me HVN / Golden Valley Memorial | Chair / CEO | https://www.mohospitals.org/newsroom/independent-missouri-hospitals-unite-to-launch-show-me-high-value-network/ | 2026-09-09 |
| Todd Ahrens | Show-Me HVN / Hannibal Regional | Vice Chairperson / President & CEO | https://www.nemonews.net/2026/09/16/hannibal-regional-joins-show-me-high-value-network-to-strengthen-care-close-to-home/ | 2026-09-16 |
| Bill Hellebusch | Hermann Area District Hospital (Show-Me HVN) | CEO | https://www.gasconadecountyrepublican.com/stories/hermann-area-district-hospital-joins-consortium-of-independent-hospitals-to-improve-bargain-stance,250334 | 2025-12-03 |
| Curt Zimmerman | ICAHN | business partner contact (title NOT_FOUND) | https://icahn.org/business-partners/ | undated |
| Daniel Grigg | Wallowa Memorial Hospital (Cascades HVN) | CEO | https://www.wweek.com/news/health/2026/09/01/many-small-health-systems-have-been-hoovered-up-rejecting-this-fate-rural-oregon-hospitals-are-uniting/ | 2026-09-01 |

Phase 1 people for these orgs are also valid. They are in /home/user/ktodi2/output/work/phase1/E_networks_systems.md: Linda K. Weiss, Elya Prystowsky, Angelina Salazar, Rodney Triplett, Patrick Ganyo, Curt Colson, Sara Calhoun, Nathan White, Ben Bucher, Steve Todd, Alfred Sams, Mellie Boagni, Stephen Stoddard, Dee Dee Dewell.
