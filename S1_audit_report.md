# Agent S1 – Evidence Extraction Audit: Supplementary Table S1

**Status: PARTIAL (Phase 1 of 2). S1 has NOT been edited and no tracked changes have been applied.**

## 0. Limits of this audit (read first)

| Requirement | Status |
|---|---|
| Original full-text sources (54 papers) | **Not available.** Only the S1 .docx was supplied. PubMed, Europe PMC, Crossref and doi.org are blocked by the sandbox network policy (HTTP 403 at proxy), so no source could be retrieved. |
| Manuscript | **Not supplied**, so "in manuscript but absent from S1" and "in S1 but never used" cannot be determined. |
| What was done | (a) structural audit of S1 against the 16 required fields; (b) internal-consistency audit (arithmetic, cross-row contradictions, citation metadata, terminology, overlap); (c) list of source-checks still required. |
| Verdict rule applied | No row is marked **Verified** against a source. Where only internal arithmetic/consistency was checkable, that is stated. Nothing below is a corrected value; corrections are *proposals* that need the source. Values marked "(recalled)" come from model memory and must be confirmed against the paper before use. |

Per the brief ("do not rewrite S1 until the audit is complete") and because no correction is source-confirmed, tracked changes are deferred to Phase 2.

## 1. Structural audit: S1 columns vs. the 16 required fields

S1 has 8 columns (ID/route, Publication, Setting, Evidence type, Index event, Population/follow-up, Operational elements, Contribution/provenance). The 16 audit fields are not separate columns.

| # | Required field | Where it sits in S1 | Coverage problem |
|---|---|---|---|
| 1 | Author/year | Publication | Present for all 54 |
| 2 | Country/setting | Col 3 | Present; some generic ("International", "Europe") |
| 3 | Study design | Evidence type | Present; labels inconsistent (see §5) |
| 4 | Population | Population/follow-up | Free text, uneven |
| 5 | Sample size | Population/follow-up | Absent or vague for S01, S04, S05, S07–S10, S12, S35, S37, S38, S46, S49 (S35: "BEST-CLI participants") |
| 6 | Diabetes status | Ad hoc in a few rows (S06, S19, S22, S24, S25, S27, S40) | **NR required** for S17, S18, S20 (all diabetic by title only), S34, S35, S36, S43, S44, S49, S54, S08–S10, S32 |
| 7 | Index event/state | Col 5 | Present; wording inconsistent (see §5) |
| 8 | Intervention/exposure | "Operational elements mapped" | Mixes framework labels with exposures; not a true field |
| 9 | Comparator | none | Only implicit (S13, S14, S15, S25, S28, S29, S31, S50, S53, S54). **No column** |
| 10 | Follow-up | Population/follow-up | Missing for S01, S04, S05, S07–S10, S12, S32, S37, S38, S43, S46, S47 → NR; S49 already states NR |
| 11 | Outcomes | none (embedded in col 8) | **No column** |
| 12 | Numerical results | Embedded in col 8 | Metric type (crude / KM / pooled / adjusted) rarely stated |
| 13 | Surveillance/follow-up schedule | none | Absent for S14, S16, S17, S18, S19, S44, S54, S13, S50 even though surveillance is the framework's subject. **No column** |
| 14 | Recurrence/reintervention/amputation definitions | none | Absent for every row that reports recurrence, reintervention or amputation |
| 15 | Main finding | Col 8 | Present |
| 16 | Relevance to framework | Col 8 ("Provenance") | Present, but see S36, S43, S46, S48 (indirect) |

**Finding G1 (Major discrepancy, structural):** fields 9, 11, 13 and 14 have no home in S1. Any audit or correction for them requires either new columns or a companion table.

## 2. Row-level findings (issues only)

Column key: "Original source" = *not accessed* unless stated. Verdicts use the requested vocabulary.

| S1 row | Field | Current value | Original source | Verdict | Correction / action |
|---|---|---|---|---|---|
| Scope note | NR definition | "NR indicates information not reported **or not verified** in the current extraction" | n/a | **Major discrepancy** | NR must mean "not reported in the source". "Not verified/not yet extracted" is a different state and hides extractor gaps. Split into NR (source silent) vs. a temporary "NE" (not yet extracted), and remove NE before submission. |
| Scope note | Linked-report list | Lists S34/S35, S30/S31, S11/S47, S41/S42, S33⊂S02 | S1 internal | **Major discrepancy** | Incomplete. Also overlapping/companion: **S06 ⊃ S02 DFU data** (stated in S06 row but not in scope note); **S06 reuses BEST-CLI (S34/S35) data**; **S29 ↔ S30/S31** (same Singapore LEAPP programme; patient overlap NR, check); **S06 + S48** (same author group, compiled outcomes). See §3. |
| S11 / S47 | Companion link | S11 = clinician's guide to the **2024** VA/DoD CPG (pub. 2026); S47 = Webster 2019 (update of the earlier VA/DoD CPG) | Cited years in S1 | **Major discrepancy** (on S1's own citations) | These describe different guideline versions, not one guideline family. Verify in S47 which CPG edition it summarises. If it is the 2017 CPG, relabel as "predecessor/successor guideline versions", not "linked reports of the same guideline". Both rows currently say "linked". |
| S26 | Numerical results | "median survival 69 months; 5-year mortality 50%" | not accessed | **Major discrepancy** (internal impossibility) | If median survival is 69 months (>60), 5-year mortality must be <50%. One figure is wrong or refers to a different denominator/time origin. Re-extract both; state the origin of time (admission, discharge, amputation). |
| S29 | Outcomes / terminology | "fewer 1-year amputations" | not accessed | **Major discrepancy** (unspecified level) | Amputation level not stated. S30/S31 report *no* reduction in (major) amputations and *more* minor. Re-extract with minor vs major separated, plus effect size and metric. |
| S06 | Numerical results | "3-year DFU recurrence 58%; 3-year reintervention 50.1% after endovascular therapy" | not accessed | **Minor discrepancy** | (i) metric type (crude, KM, cumulative incidence) NR-in-S1; (ii) "reintervention" ≠ restenosis ≠ MALE – state the source definition; (iii) 58% vs S02's ~60% at 3 years, and S03's 29.3% at 12 months vs S02's ~40% at 1 year: add one line explaining population/definition differences (all healed DFU vs remission cohorts). |
| S06 | Overlap | "DFU data largely overlap S02" | S1 internal | **Minor discrepancy** | Also overlaps S34/S35 (BEST-CLI) and possibly S14/S15 (RCT usual-care arms), S33. Disclose; do not count as independent evidence. |
| S34 | Numerical result | "MALE-or-death 42.6–57.4% in cohort 1" | not accessed | **Minor discrepancy** | Range hides the arm assignment. Proposed: state arm-specific values (recalled: 42.6% surgery vs 57.4% endovascular, HR ≈0.68) and that the composite is MALE **or death**, with the trial's MALE definition (recalled: major amputation or major reintervention). Do not use it as a "reintervention" figure. Confirm all values. |
| S35 | Sample size / follow-up / result | "BEST-CLI participants" | not accessed | **NR required** (or extract) | No n, follow-up, or numeric result. Source almost certainly reports these; extract them. Check whether the analysis cohort matches the n=1,434 quoted in S06. |
| S39 | Terminology | "Ipsilateral and contralateral reamputation … contralateral 20.5% at 5 years" | not accessed | **Minor discrepancy** | A contralateral amputation is a new-limb event, not "reamputation". Label "ipsilateral re-amputation" vs "contralateral amputation". State pooled-proportion vs KM. Fix inconsistent precision (19% vs 37.1%). |
| S51 | Numerical result | "129 inpatients … re-amputation 32.5%" | not accessed | **Minor discrepancy** | 32.5% × 129 = 41.9; nearest integer counts give 32.6% (42/129) or 31.8% (41/129). Check numerator/denominator (analysed n may differ from 129). Also re-amputation definition (same level, higher level, any limb) is NR. |
| S22 | Population | Index "Diabetes-related transmetatarsal amputation"; 88% diabetes | not accessed | **Minor discrepancy** | 12% not diabetic; relabel "TMA (88% with diabetes)". |
| S24 | Design / diabetes | "Vascular minor amputation", 79.5% diabetes | not accessed | Verified (arithmetic only: 79.5% of 200 = 159) | Keep; confirm KM values are the only 5-year figures cited. |
| S25 | Design vs claim | Comparative n=11 vs 130 historical controls; provenance "comparative empirical" | not accessed | **Minor discrepancy** | Feasibility/pilot, not efficacy. Change provenance to "implementation-based (pilot)"; n=11 precludes effect inference. |
| S15 | Main finding | High-adherence subgroup "prespecified"; "effectiveness depends on adherence" | not accessed | **Minor discrepancy** | Adherence is post-randomisation, so subgroup comparison is observational, not causal. Confirm "prespecified" in the paper; reword to "in the exploratory high-adherence subgroup recurrence was lower (25.7% vs 47.8%; n=79), an association". ITT values NR-in-S1: add them. |
| S14 | Numerical result | Any-site recurrence "was lower" (no number) | not accessed | **NR required → extract** | Add effect estimate. Keep "primary-site" (same-site) vs "any-site" distinction; add the source's definition of each. |
| S13 | Numerical / design | 21.1% vs 41.8% (8/38 vs 38/91 recomputed) | not accessed | Verified (arithmetic only) | Arithmetic reconciles. Add: recurrence definition NR; confounding by indication; crude proportions. |
| S53 | Numerical / follow-up | 59.2% vs 32.7% (77/130, 49/150 reconcile) | not accessed | Verified (arithmetic only); follow-up **NR required** | "follow-up to 2016" is not a duration. State duration or NR; state whether reulceration = same-site or any-site. |
| S33 | Numerical result | "42/73 (57.5%)" | not accessed | Verified (arithmetic only) | Label as crude 3-year proportion (not KM). Confirm the S02 inclusion claim from S02's supplement. |
| S40 | Numerical | 1,140 + 575 = 1,715 | not accessed | Verified (arithmetic only) | KM to 5 years – keep; label which figures are KM. |
| S27 | Numerical | 31 + 11 = 42; 83% ≈ 35/42 | not accessed | Verified (arithmetic only) | – |
| S41 | Outcome | "18.2% among 390 with known outcome" | not accessed | **Minor discrepancy** | 390/888 = 44% ascertainment; say so. The composite "major amputation or death" must not be read as amputation rate. |
| S41 / S42 | Duplicate cohort | "overlapping cohorts from one hospital" | S1 internal | **Minor discrepancy** | S41 = 2016–2019; S42 = 2016 only. Overlap is plausible but patient-level overlap is unproven; word as "same hospital, possibly overlapping" until confirmed. |
| S44 | Design | "retrospective (cross-sectional)" with 2-year graft-occlusion outcome | not accessed | **Minor discrepancy** | A study with a 2-year outcome is a retrospective cohort. Recheck the source's own label; if the authors say "cross-sectional", quote it. Also diabetes status NR. |
| S45 | Citation | "2026;25(1):55–64 (published online 2023)" | not accessed | **Minor discrepancy** | Year/volume/DOI mismatch is unusual; confirm the version of record. |
| S48 | Terminology | "Pooled literature … 5-year mortality DFU 30.5%, minor 46.2%, major 56.6% vs cancer 31.0%" | not accessed | **Minor discrepancy** (recalled figures match my memory, unconfirmed) | If the source is a literature synthesis rather than a meta-analysis, replace "pooled" with "synthesised/weighted". State the metric. |
| S49 | Sample size / diabetes / FU | Not given | not accessed | **NR required** | Add n; diabetes status (dysvascular ≠ diabetic); FU stays NR. |
| S43 | FU / diabetes / period | Not given | not accessed | **NR required** | Add study period, follow-up, diabetes proportion or NR. |
| S17 | Population | "103 randomized trials; 96 surveillance protocols" | not accessed | **NR required** (diabetes) | Diabetes status NR; relevance to diabetic limb indirect. |
| S18, S19, S54 | Diabetes/relevance | S19 = 36% diabetes; S18 and S54 NR | not accessed | **NR required / indirect relevance** | Mark diabetes proportion; note these are generalised PAD/CLTI evidence. |
| S02, S03, S06, S48, S21, S39, S45 | Provenance label | S02, S48 "conceptual"; S03, S06, S21, S39 "observational"; S45 "observational" | S1 internal | **Minor discrepancy** | Same evidence type (secondary synthesis) is labelled differently. Adopt one rule (e.g. narrative review = conceptual; systematic review = observational synthesis; both distinct from primary data) and apply it. |
| S16 | Feasibility | "Demonstrates remote monitoring linked to a defined reviewer" | not accessed | Verified in wording (feasibility, no efficacy claim) | Keep. Confirm n=27/26 and 1.1 days. |
| S12, S04, S05, S37, S38, S01 | Not data studies | conceptual/commentary | – | Verified as non-quantitative | Confirm none of them supply numbers in the manuscript. |
| S46 | Relevance | S1 itself says "no post-revascularization surveillance content" | S1 internal | **Unsupported** for the survivorship framework | A source with no relevant content should not be one of 54 "included" reports. Candidate for exclusion or reclassification as background. |
| S36, S43 | Relevance | "clinical importance of timely expert assessment / delay" | not accessed | **Minor discrepancy** | Active-ulcer/active-CLTI timeliness evidence is indirect for post-healing survivorship; state that. |

## 3. Requested cross-cutting checks

### Duplicate / overlapping cohorts
- S30 and S31: same 2,798-patient programme cohort (companion; S31 adds matched controls and modelling). S1 already flags. **Verified from S1 alone.**
- S29 ↔ S30/S31: same LEAPP programme, Singapore; **not flagged in S1**; patient overlap unknown.
- S34 ↔ S35: parent/secondary analysis (flagged). S06 reuses BEST-CLI reintervention data (**not flagged**).
- S33 ⊂ S02 (flagged); S06 DFU data largely ⊂ S02 (flagged only in S06 row).
- S41 and S42: same hospital, possibly overlapping patients (2016 in both).
- S03 pooled remission cohorts may overlap S02/S33/S06 (check).

### Companion publications
S30/S31, S34/S35, S11/S47 (see version problem above).

### Numerical inconsistencies
S26 (median survival vs 5-yr mortality); S51 (32.5%); S06 vs S02 (58% vs ~60% at 3 y); S03 vs S02 (29.3% at 12 mo vs ~40% at 1 y – explainable but unexplained); S29 vs S30/S31 (amputation direction/level); S35 vs S06 (BEST-CLI n). Arithmetic that reconciles: S13, S24, S25, S27, S33, S40, S53, and the 52 + 2 = 54 count (also 54 rows present).

### Terminology inconsistencies
- Index state: "Healed DFU" (S01, S02, S13, S33), "DFU remission" (S04, S50), "Confirmed DFU remission" (S03), "Healed / high-risk DFU" (S14), "Prior DFU / high-risk foot" (S16), "Recently healed plantar DFU" (S15), "Healed/recurrent DFU" (S53), "At-risk / healed DFU" (S07). Healed ≠ remission (remission needs a defined ulcer-free interval) and "at-risk" mixes incident-ulceration prevention with recurrence prevention.
- Recurrence: "recurrence", "reulceration", "recurrent ulceration", "primary-site" vs "any-site". The distinction between DFU recurrence and incident ulceration is never made explicit.
- Amputation: "reamputation" (S21, S22, S39), "re-amputation" (S51), "LEA" (abbreviation only), "amputation" unqualified (S29). Contralateral events labelled "reamputation" (S39). Minor/major not consistently split.
- Reintervention: "reintervention" (S06, S09, S18, S19), "secondary interventions" (S35 title), "major adverse limb event" (S34). Restenosis is not used; patency is (S18). These are distinct constructs and S1 never states which the source reports.
- Metric type (crude / KM / pooled / adjusted) stated only for S24, S40, S28.
- Design labels: "Longitudinal cohort" (S20, S22), "Program cohort analysis" (S30), "Retrospective registry study" (S19), "Cross-sectional" (S44), author-labelled "case-control" (S29, handled).
- Causal language: S15 ("effectiveness depends on…") and any "improves/reduces" wording should be reserved for randomized ITT results; S13, S28, S41, S44, S53 are associations (S1 mostly flags this correctly).

### Manuscript ↔ S1 (needs manuscript)
- Studies in the manuscript but absent from S1: **cannot assess.**
- Studies in S1 but never used in the manuscript: **cannot assess.** Candidates to check first: S46 (no relevant content per S1), S36, S43, S48, S52, S19, S17.

## 4. Source checks still required (Phase 2)

Provide either the 54 PDFs, or a folder of the key ones, plus the manuscript. Priority order (highest risk first):
1. S26, S29, S51, S06, S34/S35, S39 (numerical/terminology problems above)
2. S11/S47 (guideline version)
3. Numeric extractions for S14, S15, S22, S24, S25, S30, S31, S40, S41, S42
4. All the sample-size, follow-up, diabetes-status and definition fields flagged NR
5. Remaining rows (metadata check: authors, year, volume, pages, DOI)

## 5. Proposed handling once sources are available

When sources are supplied I will (a) re-run this table for all 54 rows against the full text with verdicts, and (b) apply **only source-confirmed** changes to the .docx as Word tracked changes (revision marks with author "Claude"), leaving unresolved items as comments. No edits are made now.
