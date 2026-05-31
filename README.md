# Project 4 — EHR Workflow Redesign BRD

![Status](https://img.shields.io/badge/Status-Complete-4A9B6F)
![Python](https://img.shields.io/badge/Python-3.x-1E566C)
![Tableau](https://img.shields.io/badge/Tableau-Public-5795A7)
![Jira](https://img.shields.io/badge/Jira-Atlassian-D7A800)

## Overview

A compliance-driven Business Requirements Document (BRD) for the redesign of the EHR-to-insurer claims workflow at a leading UAE health insurer. The current workflow is manual, fragmented, and non-compliant — generating a 33.6% denial rate across 4,500 claims and AED 7.55M in unrecovered revenue.

This project identifies 6 gaps across three parties (Provider, Insurer, Regulator), quantifies their financial impact, and produces a formal BRD with full requirements traceability — delivered across Confluence, Jira, Jupyter, Tableau, and Visio.

---

## BRD Documents

Two versions of the BRD are committed to this repository under `brd/`:

| Document | Description |
|---|---|
| [BRD — Full Confluence Export](brd/BRD_full_Confluence.pdf) | Complete 14-section BRD produced in Confluence — stakeholder register, requirements traceability (FR-01 to FR-06), 17 non-functional requirements, assumptions, constraints, and sign-off matrix |
| [BRD — Executive Summary](brd/BRD_summary.pdf) | 7-page overview covering gap analysis, Jira epics/stories, delivery phases, and financial case — quick-read version for stakeholder review |

The live BRD and Jira backlog are maintained in Atlassian Confluence and Jira. These PDFs are static snapshots committed for portfolio accessibility.

---

## Key Numbers

| Metric | Value |
|---|---|
| Total claims | 4,500 |
| Denial rate | 33.6% |
| Denied value | AED 7,550,894 |
| Inpatient denial rate | 32.7% |
| Total gap recovery | AED 9,200,000 |
| P3 model AUC | 0.950 |
| High-cost member detection | 87% (projected at 70% conservative deployment rate) |

---

## 6 Gaps Identified

| Gap | Party | Recovery | Risk |
|---|---|---|---|
| Gap 1 — ICD-10 coding errors | Provider | AED 1,600,000 | High |
| Gap 2 — No EHR/RCM integration | Provider/Insurer | AED 1,100,000 | High |
| Gap 3 — Manual pre-authorisation | Insurer | AED 1,200,000 | Critical |
| Gap 4 — No high-cost member ID | Insurer | AED 3,400,000 | High |
| Gap 5 — No automated denial follow-up | Insurer | AED 400,000 | High |
| Gap 6 — No compliance check | All parties | AED 1,500,000 | Critical |

Recovery figures reflect estimated recoverable amount after solution implementation. Raw AED impact figures and full derivations are in `brd/BRD_full_Confluence.pdf` and Notebook 02.

---

## Deliverables

| Deliverable | Tool | Status |
|---|---|---|
| BRD Document — 10 sections | Confluence | ✅ Complete |
| User Stories — 6 Epics · 18 Stories | Jira | ✅ Complete |
| As-Is Analysis | Jupyter Notebook | ✅ Complete |
| Gap Analysis | Jupyter Notebook | ✅ Complete |
| To-Be Process Design | Jupyter Notebook | ✅ Complete |
| BRD Data and Charts | Jupyter Notebook | ✅ Complete |
| KPI Dashboard | Tableau Public | ✅ Complete |
| BPMN As-Is Process Map | Visio | ✅ Complete |
| BRD PDF — Full Confluence Export | PDF | ✅ Committed |
| BRD PDF — Executive Summary | PDF | ✅ Committed |

---

## Delivery Phases

| Phase | Scope | Timeline | Recovery |
|---|---|---|---|
| Phase 1 — Foundation | ICD-10 validation + EHR-RCM integration | Months 1–3 | AED 2,700,000 |
| Phase 2 — Automation | Pre-auth engine + denial routing + compliance check | Months 4–6 | AED 3,100,000 |
| Phase 3 — Intelligence | P3 predictive model deployment | Months 7–9 | AED 3,400,000 |

---

## Regulatory Context

- **DHA** — Dubai Health Authority — Shafafiya portal compliance
- **DoH/HAAD** — Abu Dhabi Department of Health
- **eSMA** — Emirates Health Insurance Portal
- **ICD-10** — Mandatory coding standard for all UAE claims
- **Pre-authorisation** — Mandatory for all inpatient claims
- **90-day window** — Hard DHA/DoH submission deadline

---

## Tools Used

`Python` `pandas` `matplotlib` `scikit-learn` `SQL` `Tableau` `Jira` `Confluence` `Visio`

---

## Portfolio

This is Project 4 of 4 in the UAE Healthcare Analytics Portfolio.

| Project | Topic | Link |
|---|---|---|
| P1 | UAE Claims Denial Analysis | [GitHub](https://github.com/AmrThabetA/healthcare-claims-analysis) |
| P2 | RCM Performance Dashboard | [Tableau Public](https://public.tableau.com/app/profile/amr.thabet/viz/UAE-MENA-RCM-Dashboard/UAEMENARCMPerformanceDashboard2023-2024) |
| P3 | Chronic Disease Cost Modelling | [GitHub](https://github.com/AmrThabetA/chronic-disease-cost-modelling) |
| P4 | EHR Workflow Redesign BRD | This repository |
| Visual Suite | Healthcare Analytics — Observable Plot | [Live Dashboard](https://amrthabeta.github.io/portfolio-visuals/src/visual_suite.html) |

---

## Links

- [Tableau KPI Dashboard](https://public.tableau.com/app/profile/amr.thabet/viz/EHRWorkflowRedesignBRDKPIDashboard/EHRWorkflowRedesignBRDKPIDashboard)
- [BRD — Full Confluence Export](brd/BRD_full_Confluence.pdf)
- [BRD — Executive Summary](brd/BRD_summary.pdf)
- [Healthcare Analytics Visual Suite](https://amrthabeta.github.io/portfolio-visuals/src/visual_suite.html)
- [GitHub Profile](https://github.com/AmrThabetA)

---

*Author: Amr Thabet · Healthcare Data and Business Analyst · Abu Dhabi, UAE*
