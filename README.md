# Supply Chain Analysis — Python & Pandas

A data analysis project exploring supply chain performance using a Kaggle dataset (100 SKUs, 3 product lines, 5 suppliers). Built to simulate the kind of data-driven supplier evaluation and risk assessment done in real procurement roles.

---

## Objective

To identify operational risks and inefficiencies across product lines, suppliers, and logistics — and translate findings into actionable procurement recommendations, including supplier risk ranking, inventory replenishment priorities, and logistics cost optimisation.

---

## Analysis Summary

| # | Analysis | Key Finding |
|---|----------|-------------|
| 1 | Revenue by Product Type | Skincare leads at $244K — 41% of total revenue |
| 2 | Low Stock Warning | 27% of Skincare SKUs below safety stock; SKU68 fully depleted |
| 3 | Defect Rate by Supplier | Supplier 5 records the highest defect rate (2.66%) |
| 4 | Cost by Transportation Mode | Sea freight averages 25% lower cost than air freight |
| 5 | Lead Time by Supplier | Supplier 4 has the longest average lead time (17 days) with the highest variability |
| 6 | Shipping Cost vs Revenue | Shipping cost remains below 0.2% of revenue across all product lines |
| 7 | Inspection Results | Over one-third of products are Fail or Pending — Supplier 4 accounts for the highest Fail count |
| 8 | Order Distribution by Location | Kolkata leads in order volume; Mumbai generates higher revenue despite fewer orders |
| 9 | Supplier Risk Scorecard | Supplier 4 scores 0.848 (High Risk); Supplier 3 scores 0.307 (Low Risk) — composite evaluation across lead time, defect rate, and inspection results |

---

## Supplier Risk Scorecard

A composite scoring model built to evaluate suppliers across three dimensions simultaneously — reflecting how procurement teams assess vendor risk in practice.

| Supplier | Total Risk Score | Risk Level |
|----------|-----------------|------------|
| Supplier 4 | 0.848 | 🔴 High |
| Supplier 2 | 0.655 | 🟠 Medium-High |
| Supplier 5 | 0.547 | 🟡 Medium |
| Supplier 1 | 0.433 | 🟢 Low-Medium |
| Supplier 3 | 0.307 | 🟢 Low |

**Scoring methodology:** Lead Time (40%) + Defect Rate (40%) + Inspection Fail Count (20%)  
Weights are adjustable based on sourcing strategy — e.g. a semiconductor company might weight defect rate higher due to yield sensitivity.

---

## Key Takeaways

- **Skincare** drives the highest revenue ($244K, 41% of total) but carries the greatest operational risk — 27% of SKUs are below safety stock and SKU68 is fully depleted. Recommended action: trigger immediate replenishment for SKU68 and raise safety stock thresholds for Skincare by 15-20% to prevent stockout-driven revenue loss.

- **Supplier 4** is the highest-risk vendor across all dimensions — longest lead time (17 days), above-average defect rate, and highest inspection fail count — composite risk score of 0.848, significantly above the group average. Recommended action: initiate dual-sourcing strategy, reduce Supplier 4's order allocation by 20-30% pending a formal quality review, and set a 90-day performance improvement timeline.

- **Supplier 3** is the strongest overall performer (risk score: 0.307) — recommended as preferred supplier for critical SKUs. Recommended action: consolidate high-priority orders with Supplier 3 and explore long-term contract negotiation to lock in favourable terms.

- **Supplier 5** presents an independent quality risk with the highest defect rate (2.66%) — quality audit recommended regardless of lead time performance. Recommended action: request corrective action report (CAR) from Supplier 5 within 30 days and monitor defect trend over next two quarters.

- **Sea freight** is the most cost-efficient mode at ~25% below air freight — a strategic shift toward sea routing could reduce logistics costs without compromising delivery windows. Recommended action: review current air freight usage and identify SKUs where lead time buffer allows a modal shift to sea freight.

- **Mumbai** generates the highest revenue despite fewer orders than Kolkata — indicating a higher average order value and stronger spending power per transaction. Recommended action: prioritise Mumbai for premium product allocation and targeted marketing investment to maximise revenue per order.
---

## Tools

- Python — pandas, matplotlib
- Power BI — 4-page interactive dashboard with cross-filtering by supplier and KPI cards
- Google Colab
- Dataset: [Kaggle Supply Chain Analysis](https://www.kaggle.com/datasets/harshsingh2209/supply-chain-analysis)

---

## About

Built as a portfolio project to demonstrate data-driven thinking applied to real supply chain problems.  
Relevant to roles in procurement, supply chain analytics, and operations management.
