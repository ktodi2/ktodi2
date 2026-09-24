# Phase 3 census: State Office of Rural Health / Flex + RHTP state program / intermediary
Date checked: 2026-09-24. Companion to state_funders.csv (53 rows: 33 SORH/Flex, 20 RHTP).

## Process caveat (read first)
- After the first two web searches and one fetch, the session's auto-mode safety classifier blocked all further web searches and all script execution for the rest of the conversation. So:
  - Only 2 fresh searches and 1 fetch were run in Phase 3, not the 6+ per type the instructions require. Everything else is carried over from the Phase 1 files (A_rhtp.md, B_sorh_flex_funders.md, plus C/D/E/F for cross-checks). Those files cite a URL for every fact, fetched 2026-09-24.
  - I could not run the Python csv writer. state_funders.csv was written by hand in QUOTE_ALL format: every field is double-quoted, and no field has an internal double quote (quotes inside fields use single quotes). The generator script is at the scratchpad path below if the lead wants to re-run it: /tmp/claude-0/-home-user-ktodi2/8a62eea2-8e87-5aff-b297-25e7453f32a8/scratchpad/build_state_funders.py
  - Recommended follow-up (lead or a fresh session): run the remaining targeted searches listed under "Gaps" below.

## Searches run in Phase 3
1. Exa: "Montana DPHHS Rural Health Transformation Center of Excellence implementation contract awarded vendor". This found the Billings Gazette / Montana State News Bureau story of 2026-09-18 (below).
2. Exa: "Kansas Healthworks Revenue Support Program RFP award ... selected". No award found. Returned the Healthworks RHTP page (RFPs still listed), the civicoperator.com Kansas profile (no award), ruralcarejourney.com and KDHE pages.
3. Fetch: billingsgazette.com article_46e523e6 (headline, lede and captions are in clear text; the body is obfuscated character-shifted text).
4. The next search, for the MT CoE Implementation awardee and the Indelible conflict story, was blocked by the classifier.

## Critical findings on the two RFPs
- **Montana CoE.** Billings Gazette, 2026-09-18, by Carly Graf. Headline: "After false start, DPHHS to award multimillion-dollar rural health contract to Deloitte". Page title: "Deloitte poised to receive $20M to overhaul MT healthcare". Clear-text lede: "Following a potential conflict of interest that halted earlier contract negotiations with an out-of-state consultant, the Montana Department of Public Health and Human Services will award a large sum of federal dollars to a different firm to oversee rural health improvements." https://billingsgazette.com/news/state-regional/article_46e523e6-8217-5dc8-afca-fd40449d5345.html
  - INFERENCE: I decoded the shifted body text by hand, and it has not been re-verified in a clean copy. It appears to say:
    - the state procurement site was updated to show Deloitte as the selected contractor;
    - the original top bidder, Indelible Health Solutions LLC (Florida), was thrown out over a potential conflict of interest involving its subcontractor McKinsey & Company, which had helped Montana win the RHTP funds;
    - Deloitte's roughly $20M proposal scored second to Indelible's roughly $25M proposal;
    - the winner "will lead the Center of Excellence" (statewide analysis and facility-specific financial-stability recommendations);
    - the CoE sunsets at the end of 2028;
    - hospitals that adopt its recommendations get payments;
    - about 89% of MT hospitals operate in the red.
  - Related headlines on the same page (clear text): "Next steps unclear for $25M in rural health funds following potential conflict of interest" and "DPHHS Director Charlie Brereton to leave department for private sector at end of October".
  - INFERENCE: this is the **CoE Strategy & Analytics** RFP (DPHHS-RFP-2026-0671), because DPHHS says the CoE is "created and operated by the CoE Strategy and Analytics vendor". **The CoE Implementation RFP awardee is NOT_FOUND as of 2026-09-24.** That contract is the one that holds the shared back-office and RCM scope.
- **Kansas Revenue Support Program RFP** (Healthworks/KHA Foundation, due 2026-07-30): **awardee NOT_FOUND as of 2026-09-24.**
  - The Healthworks page still lists the RFPs and Q&A: https://www.kha-net.org/aboutkha/healthworks/projects/rhtp/
  - The civicoperator KS profile lists no award: https://www.civicoperator.com/work/rht/states/kansas/
  - The same profile notes a CMS site visit to Kansas on Sept 22-23, 2026, and the Oct 30, 2026 obligation deadline. INFERENCE: an award announcement is likely before Oct 30.

## Universe enumerated
- **SORH/Flex:** all 31 required states (MT, ND, SD, NE, KS, IA, MN, WI, MI, IL, IN, OK, TX, CO, ID, WA, OR, WY, NM, GA, KY, MO, AR, MS, ME, NY, PA, CA, VA, HI, AK), plus NOSORH and the National Rural Health Resource Center (TASC). That is 33 rows. Standing FOI contractors are named inside rows: MHREF/MHA (MT), HomeTown Health (IA, GA RISE), KRHOP/HealthWorks (KS), and THA (TN, named in the TN RHTP row).
- **RHTP:**
  - MN MDH ORHPC
  - KS: Healthworks RTSO/RSP; UKHS Care Collaborative
  - MT: DPHHS RHTP; Deloitte CoE; MHA/MHREF
  - WA HCA Provider Technology Fund
  - MS RTG
  - ID, WY, ND
  - SD Health Link
  - OK provider collaborative
  - OR, WI, TN (+THA), AR, IA, TX

  That is 20 rows.
- There are 53 rows in total, against a target of about 40. I kept every state the task listed as required rather than cut any.
- MN has two rows (Flex billing/coding grant vs. RHTP formula grants). MT has three RHTP-side rows plus the Flex row: Flex FOI (MHREF), DPHHS RHTP, Deloitte, and MHA/MHREF as an RHTP implementing partner. These are distinct programs, and each row is labeled.

## Dropped and why
- Utah (UHA runs Flex FOI; 13 CAHs) and Tennessee SORH as separate rows: not on the required SORH list. The TN Flex/THA role is noted in the TN RHTP row. UHA is in the C_assoc file.
- AL, AZ, FL, LA, NV, NH, NC, OH, SC, VT, WV, MA SORHs: not required, and most have fewer than 20 CAHs. MA is useful only as an RCM collaborative precedent with 3 CAHs.
- Flex Monitoring Team: an evidence source, not a channel.
- DRCHSD/DSIP, ARH-TAC, USDA/NRHA TA, Helmsley, CoBank, TX HHSC Office of Rural Hospital Finance, GA HEART: different partner types (federal TA and other funders), covered in B file part 2.
- The Rural Collaborative (WA) and CO/KS networks: network type (E file).
- Georgia RHTP (no RCM language), Kentucky RHTP (public-health focus) and Nebraska RHTP (the RFA lists "Administrative IT systems" as limited; NETECH is startup funding): no revenue-cycle hook in the program, so no RHTP row. Nebraska SORH is included.
- Colorado RHTP (HCPF): no explicit RCM language. The CRHC SORH row carries its RHTP TA-contractor role.

## Gaps to close (searches that were blocked)
- MT CoE Implementation awardee: check bids.mt.gov/eMACS, the MHA newsletter, and Montana Free Press.
- A clean re-verification of the Deloitte article body.
- The KS Revenue Support Program awardee: check the KHA Healthworks news page and the KHA "Kansas Hospital News".
- MS RTG awardee list.
- The OK provider collaborative management vendor.
- WY centralized billing awardee.
- MN BP2 work-plan deadline.
- WA PTF awardees.
- ND Y2 implementation grants.
- TN Health Tech awards.
- Current Flex coordinator names for MN, TX, WA, KS.

## People seen on official pages (for Phase 4; verify before use)
| name | org | title | source URL | date |
|---|---|---|---|---|
| Charlie Brereton | Montana DPHHS | Director (leaving end of Oct 2026 per Billings Gazette headline) | https://billingsgazette.com/news/state-regional/article_46e523e6-8217-5dc8-afca-fd40449d5345.html | 2026-09-18 |
| Sadie Jones | MT DPHHS OIG | Flex Coordinator | https://dphhs.mt.gov/Panels/OIG/RuralHospital | seen 2026-09-24 (Phase 1) |
| Leslie Howe | MT DPHHS OIG | Flex Program Manager | https://dphhs.mt.gov/Panels/OIG/RuralHospital | seen 2026-09-24 (Phase 1) |
| Casey Driscoll | MHA / MHREF | Director of Quality Programs, Flex lead | https://mtpin.org/wp-content/uploads/2025/05/2025-Quality-Update.pdf | 2025 |
| Jack King | MHA | Finance & Operations Program Specialist | https://mtpin.org/wp-content/uploads/2025/05/2025-Quality-Update.pdf | 2025 |
| Shannan Flach | Healthworks / KHA | Contact for RTSO and RFPs | https://www.kha-net.org/aboutkha/healthworks/projects/rhtp/ | seen 2026-09-24 |
| Jennifer Findley | HealthWorks (KRHOP) | VP, Education and Special Projects | https://krhop.org/contact | seen 2026-09-24 (Phase 1) |
| Desiree Brown | KDHE | Primary Care & Rural Health Coordinator (KRHOP contact) | https://krhop.org/contact | seen 2026-09-24 (Phase 1) |
| Nicole Threadgold | UND Center for Rural Health | SORH Director; Flex/SHIP Coordinator | https://www.ruralcenter.org/spotlight/university-north-dakota-center-rural-health | undated |
| Holly Long | UND Center for Rural Health | ND Flex CAH Subcontract contact | https://www.ruralhealthinfo.org/funding/2253 | undated |
| Samantha Peck | Wisconsin ORH | Flex/SHIP Coordinator | https://www.ruralcenter.org/spotlight/wisconsin-office-rural-health | undated |
| Crystal Barter | Michigan Center for Rural Health | Flex Coordinator | https://www.ruralcenter.org/spotlight/michigan-center-rural-health | undated |
| Sarah Andersen | Oregon ORH (OHSU) | Flex Coordinator | https://www.ruralcenter.org/spotlight/oregon-office-rural-health | undated |
| Stephanie Sayegh | Oregon ORH (OHSU) | SHIP Coordinator | https://www.ruralcenter.org/spotlight/oregon-office-rural-health | undated |
| Wanda Hilton | Iowa HHS | SHIP/Flex Coordinator (conflict: NOSORH lists Jason Clinton) | https://hhs.iowa.gov/health-prevention/providers-professionals/rural-health/rural-hospital-programs | live page (Phase 1) |
| Dawn Waldrip | Georgia DCH SORH | Flex/SHIP Coordinator | https://www.ruralcenter.org/spotlight/georgia-office-rural-health | undated |
| Scott Daniels | Hawaii DOH OPCRH | Flex/SHIP Coordinator | https://www.ruralcenter.org/spotlight/hawaii-department-health-office-primary-care-rural-health | undated; RFQ May 2026 |
| Brandon Rivenbark | Virginia DOH | Flex/SHIP Coordinator | https://www.ruralcenter.org/spotlight/virginia-department-health | undated |
| Diana Winder | Missouri DHSS | Flex Coordinator | https://www.ruralcenter.org/spotlight/missouri-department-health-and-senior-services-office-rural-health | undated |
| Terri Nihil | South Dakota DOH | Flex/SHIP Coordinator | https://www.ruralcenter.org/spotlight/south-dakota-department-health | undated |
| Nancy Jo Hansen | Nebraska DHHS | Flex/SHIP Coordinator | https://www.ruralcenter.org/spotlight/nebraska-department-health-and-human-services | undated |
| Marcy Cameron | Colorado Rural Health Center | Flex Coordinator | https://www.ruralcenter.org/spotlight/colorado-rural-health-center | undated |
| Lara Brooks | Oklahoma ORH (OSU-CHS) | Flex Coordinator | https://www.ruralcenter.org/spotlight/oklahoma-office-rural-health | undated |
| Medina Tipton | Kentucky ORH | Flex Coordinator | https://scholars.uky.edu/en/projects/medicare-rural-hospital-flexibility-program-flex-2/ | FY2024 |
| Ashley Muninger | NOSORH | Communications Director (partner contact) | https://nosorh.org/exhibiting-information/ | 2026 |
| Juliet Charron | Idaho DHW | Director | https://healthandwelfare.idaho.gov/news/healthcare-infrastructure-support-funding-specifically-idahos-rural-healthcare-providers | 2026-08-28 |
| Stefan Johansson | Wyoming Dept of Health | Director | https://891khol.org/how-200-million-will-be-doled-out-to-wyoming-health-care-providers/ | 2026-05-26 |
| Megan Clark | WA HCA | RFA Coordinator (2026HCA12) | https://www.hca.wa.gov/assets/program/2026hca12-amendment-1.pdf | 2026-07-21 |
| Carly Graf | Montana State News Bureau | Reporter (source of Deloitte story; not a partner contact) | Billings Gazette URL above | 2026-09-18 |
