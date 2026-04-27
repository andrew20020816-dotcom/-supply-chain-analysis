# Supply Chain Analysis — Python & Pandas

A data analysis project exploring supply chain performance using a Kaggle dataset (100 SKUs, 3 product lines, 5 suppliers).

---

## Objective

To identify operational risks and inefficiencies across product lines, suppliers, and logistics — and translate findings into actionable procurement recommendations.

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

---

## Supplier Risk Assessment

Cross-referencing lead time and defect rate data surfaces **Supplier 4** as the highest-priority concern — it ranks worst on delivery speed and shows above-average defect rates, presenting compounded risk to both schedule and quality. **Supplier 5** independently flags as a quality risk with the highest defect rate in the dataset.

---

## Tools

- Python — pandas, matplotlib
- Google Colab
- Dataset: [Kaggle Supply Chain Analysis](https://www.kaggle.com/datasets/harshsingh2209/supply-chain-analysis)

---

## About

Built as a portfolio project to demonstrate data-driven thinking applied to real supply chain problems.
Relevant to roles in procurement, supply chain analytics, and operations management.
