# NovaTech Generative BI — Amazon QuickSight Q Validation Log

| Metadata Field | Specification |
| :--- | :--- |
| **Lead Analyst** | Gideon Owusu |
| **Evaluation Date** | September 2026 |
| **Platform** | Amazon QuickSight & Amazon QuickSight Q (Generative BI) |
| **Validation Objective** | Cross-verification of natural language responses against visual dashboards |

---

## 1. Executive Summary

This evaluation measures the accuracy and reliability of **Amazon QuickSight Q** when answering executive business questions. Each synthesized answer was audited against validated visual components within the NovaTech Executive Dashboard (Sales Pipeline, Marketing Funnel, and Customer Health).

---

## 2. Natural Language Query Validation Matrix

| # | Business Analytical Query | QuickSight Q Generated Answer | Verification Dashboard Visual | Visual Ground Truth | Validation Status | Analytical Commentary |
| :---: | :--- | :--- | :--- | :--- | :---: | :--- |
| **1** | Which campaign channel yields the highest conversion rate? | Direct Mail achieves the highest conversion rate at 53.0%. | Marketing Funnel — Funnel Stage by Channel | Direct Mail: 53.0% conversion rate | **Exact Match** | High-touch outbound marketing outperforms digital channels in conversion efficiency. |
| **2** | What is the average realized deal size segmented by company scale? | Enterprise: $1,589.17<br>Small: $1,486.49<br>Large: $1,257.47 | Sales Pipeline — Revenue by Company Size | Enterprise: $1,589.17<br>Small: $1,486.49<br>Large: $1,257.47 | **Exact Match** | Enterprise tier delivers highest average deal value. |
| **3** | What is the average ticket resolution time for critical vs. low-priority incidents? | Critical: 1.79 days<br>Low: 1.97 days | Customer Health — Resolution Time by Priority | Critical: 1.79 days<br>Low: 1.97 days | **Exact Match** | SLA compliance prioritizes critical incidents by ~0.18 days. |
| **4** | Identify the top 10 accounts by support ticket volume and aggregate revenue. | Top 10 accounts aggregate 106,842 tickets and ~$169.7M in annual revenue (`ACCT-080`, `ACCT-043`, `ACCT-036`, `ACCT-012`, `ACCT-037`, `ACCT-072`, `ACCT-035`, `ACCT-024`, `ACCT-076`, `ACCT-041`). | Customer Health — At-Risk Accounts Matrix | Top 10 accounts aggregate 106,842 tickets and ~$169.7M in annual revenue. | **Exact Match** | Key enterprise revenue generators also impose the heaviest support load. |
| **5** | Are any marketing campaigns operating at a net loss (negative ROI)? | No active campaigns operate at a net loss. | Marketing Funnel — Spend vs. Revenue Correlation | All campaigns demonstrate positive ROI.<br>Peak: NovaPulse Launch (962.7x)<br>Baseline: NovaEdge Awareness (124.6x) | **Exact Match** | High gross marketing leverage maintained across all campaign cohorts. |

---

## 3. Governance & Generative BI Reliability Assessment

### Where QuickSight Q Succeeded
* **Metric Aggregation:** QuickSight Q exhibited perfect parity with dashboard aggregations across multi-dimensional KPIs (conversion rates, resolution durations, and revenue totals).
* **Entity Disambiguation:** Complex queries filtering specific account keys (`ACCT-XXX`) and categorical tiers (Enterprise vs. Small) parsed without ambiguity.

### Operational Recommendations
* **Ad-Hoc Exploration:** QuickSight Q serves as an accelerated self-service discovery mechanism for operational managers and non-technical stakeholders.
* **Audit Governance:** Executive and compliance-critical reporting should reference verified dashboard visualizations as the definitive system of record.
