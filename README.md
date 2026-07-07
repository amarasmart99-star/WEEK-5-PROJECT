# Bank Marketing Campaign Analysis — Business Analytics Case Study

**AnalystLab Africa Data Analytics Internship — Batch B — Week 5**

## 📌 Project Overview

This project analyzes a direct marketing campaign dataset from a Portuguese banking institution to understand why some customers subscribe to a term deposit while others do not, and which customer segments are most likely to respond positively to future campaigns.

## 🎯 Business Problem

The bank runs phone-based marketing campaigns to sell term deposits, but only 47.4% of contacted customers subscribe. Every unsuccessful call costs staff time and campaign budget. This analysis identifies the key drivers of subscription so the bank can prioritize its calling lists and campaign strategy toward the segments most likely to convert.

## 🗂️ Dataset

- **Source:** [Bank Marketing Dataset (Kaggle)](https://www.kaggle.com/datasets/janiobachmann/bank-marketing-dataset)
- **Records:** 11,162 customer contacts
- **Features:** 17 columns covering demographics, financial profile, campaign contact details, and previous campaign history
- **Target variable:** `deposit` (yes/no — did the customer subscribe to a term deposit)

## 🛠️ Tools Used

- **Python** (Jupyter Notebook) — Pandas, NumPy, Matplotlib, Seaborn
- **Power BI** — dashboard build (in progress / for practice)

## 🔍 Analysis Process

1. Dataset overview — shape, data types, duplicate check
2. Missing value assessment (none found; two data quirks noted and kept as-is: legitimate negative balances, and `pdays = -1` as a "never contacted before" placeholder)
3. Summary statistics
4. Visualizations:
   - Pie chart — subscription distribution
   - Bar chart — subscription by job type
   - Histogram — age distribution by subscription
   - Box plot — account balance by subscription
   - Correlation heatmap — numeric variables vs subscription
5. Key driver analysis (job type, previous campaign outcome, contact method, balance, call duration)

## 📊 Key Findings

| Driver | Finding |
|---|---|
| Job type | Student: 74.7% subscribe, Retired: 66.3% vs Blue-collar: 36.4% |
| Previous campaign outcome | Prior success: 91.3% subscribe again vs 40.7% with no history |
| Contact method | Cellular: 54.3% vs Unknown method: 22.6% |
| Account balance | Subscribers average $1,804.3 vs $1,280.2 for non-subscribers |
| Call duration | Subscribers average 537.3 sec vs 223.1 sec for non-subscribers |

## 💡 Business Insights

- Call engagement (duration) is the strongest single signal of a successful outcome
- Life stage — students and retirees — matters more than job prestige
- Past campaign success is the strongest predictor of future subscription
- Cellular contact significantly outperforms unknown/unlogged contact methods
- Higher account balances give a modest edge in subscription likelihood

## ✅ Recommendations

1. Prioritize recontacting past campaign responders (91.3% re-subscription rate)
2. Target students and retirees with life-stage-specific offers
3. Invest in agent training to extend meaningful call engagement
4. Improve contact data quality — prioritize verified cellular numbers
5. De-prioritize low-yield segments during high-volume campaign periods

## 📁 Repository Contents

```
├── Bank_Business_Analytics_Report.docx
├── Bank_Presentation.pptx
└── README.md
```

## 📝 Author

Amara — Batch B Intern, AnalystLab Africa Data Analytics Internship Program
