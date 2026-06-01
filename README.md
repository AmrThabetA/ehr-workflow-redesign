# Project 4 — EHR Workflow Redesign BRD

![Status](https://img.shields.io/badge/Status-Complete-4A9B6F)
![Python](https://img.shields.io/badge/Python-3.x-1E566C)
![Tableau](https://img.shields.io/badge/Tableau-Public-5795A7)
![Jira](https://img.shields.io/badge/Jira-Atlassian-D7A800)

How a manual, non-compliant claims workflow at a UAE health insurer was redesigned end to end — turning a **33.6% denial rate** and **AED 7.55M** in lost revenue into a phased plan to recover **AED 9.2M**.

---

## The Problem: the As-Is Workflow

The current EHR-to-insurer claims process is **15 manual steps** across three parties, with no validation, no integration, and no compliance check before submission. Errors are only caught *after* a claim is rejected — too late to fix inside the 90-day window.

<!-- swap in your actual as-is diagram filename below -->
![As-is claims workflow](notebooks/as_is_process.png)

**Where it breaks:**
- ICD-10 coding errors caught only at rejection (35.5% error rate for GPs)
- Claims re-keyed by hand from EHR into the RCM system
- Pre-authorisation checked manually, 3–5 business days
- No tracking of the 90-day submission deadline
- No compliance check before a claim leaves the building

---

## The Fix: the To-Be Workflow

The redesign collapses **15 manual steps → 10 automated or semi-automated steps** — adding real-time ICD-10 validation, an EHR-RCM integration layer, an automated pre-auth rules engine, and the P3 predictive model for high-cost members.

<!-- swap in your actual to-be diagram filename below -->
![To-be redesigned workflow](notebooks/to_be_process.png)

| | As-Is | To-Be |
|---|---|---|
| Workflow steps | 15 manual | 10 automated |
| Denial rate | 33.6% | < 15% |
| ICD-10 errors | caught at rejection | validated in < 2 sec |
| Pre-auth | 3–5 days, manual | automated, < 5 sec |
| High-cost members | reactive (0%) | flagged early (87%) |
| AR days | 45+ | < 25 |

---

## What That's Worth: AED 9.2M Across 6 Gaps

Each break in the as-is process maps to a quantified gap and a fix, delivered in 3 phases.

![Recovery by gap](notebooks/gap_recovery_chart.png)

| Gap | Fix | Recovery | Risk |
|---|---|---|---|
| ICD-10 coding errors | Real-time validation | AED 1.6M | High |
| No EHR/RCM integration | Auto claim generation | AED 1.1M | High |
| Manual pre-auth | Rules engine | AED 1.2M | Critical |
| No high-cost member ID | P3 model (AUC 0.950) | AED 3.4M | High |
| No denial follow-up | Auto routing + tracker | AED 0.4M | High |
| No compliance check | Pre-submission engine | AED 1.5M | Critical |

Delivered as **6 Epics / 18 Jira stories** over 3 phases (Foundation → Automation → Intelligence), with full FR-01→FR-06 traceability.

---

## The Documents

| Document | What's inside |
|---|---|
| [Full Confluence Export](brd/BRD_full_Confluence.pdf) | 14 sections — stakeholders, requirements traceability, 17 NFRs, constraints, sign-off |
| [Executive Summary](brd/BRD_summary.pdf) | 7-page quick read — gaps, epics, phases, financial case |
| [Tableau KPI Dashboard](https://public.tableau.com/app/profile/amr.thabet/viz/EHRWorkflowRedesignBRDKPIDashboard/EHRWorkflowRedesignBRDKPIDashboard) | Before/after KPI improvement + recovery by gap |

> Notebooks too large for GitHub's preview? Open via [nbviewer](https://nbviewer.org/github/AmrThabetA/ehr-workflow-redesign/tree/main/notebooks/) or click **Raw**.

**Regulatory scope:** DHA · DoH/HAAD · Shafafiya · eSMA · ICD-10 · 90-day window
**Tools:** `Python` · `pandas` · `scikit-learn` · `SQL` · `Tableau` · `Jira` · `Confluence` · `Visio`

---

## Healthcare Analytics Portfolio

| Project | Topic | Link |
|---|---|---|
| P1 | UAE Claims Denial Analysis | [GitHub](https://github.com/AmrThabetA/healthcare-claims-analysis) |
| P2 | RCM Performance Dashboard | [Tableau](https://public.tableau.com/app/profile/amr.thabet/viz/UAE-MENA-RCM-Dashboard/UAEMENARCMPerformanceDashboard2023-2024) |
| P3 | Chronic Disease Cost Modelling | [GitHub](https://github.com/AmrThabetA/chronic-disease-cost-modelling) |
| **P4** | **EHR Workflow Redesign BRD** | **This repo** |
| ✨ | Interactive Visual Suite | [Live](https://amrthabeta.github.io/portfolio-visuals/src/visual_suite.html) |

---

*Amr Thabet · Healthcare Data & Business Analyst · Abu Dhabi, UAE · [GitHub](https://github.com/AmrThabetA)*
