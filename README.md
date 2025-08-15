# EDA
This is a basic project which explores the first step of data analysis which is exploratory data analysis, to familiarise myself with knowledge gained about the steps and procedure regarding the same.

Dataset facts (from your file)
Size: 7,043 rows × 21 columns
Missing cells: 11 total (mostly in TotalCharges after coercion)
Duplicate customerIDs: 0
Headline churn metrics

# Overall churn rate: 26.5% (Yes = 1,869, No = 5,174)
-By Senior Citizen
“Senior citizens churn at 41.7% vs 23.6% for non-seniors.”

-By Contract type
“Churn is highest for Month-to-month at 42.7%, much lower for One year at 11.3%, and lowest for Two year at 2.8%.”

-By Payment Method (churn % within each method)
“Electronic check customers churn at 45.3% (highest).”
“Mailed check churn is 19.1%; Bank transfer (auto) 16.7%; Credit card (auto) 15.2% (lowest).”

-By Tenure (bucketed)
“≤ 6 months: 52.9% churn; 6–12: 35.9%; 12–24: 28.7%; 24–60: 18.3%; 60+: 6.6%.”

-Billing & Service mix
"PaperlessBilling = Yes cohort churns at 33.6% vs 16.3% for No.”
“TechSupport = No churn is 41.6%; TechSupport = Yes is 15.2%; customers with No Internet Service churn at 7.4%.”

-“By Internet service: Fiber optic churn is 41.9%, DSL 19.0%, No internet 7.4%.”

## Top high-risk cohorts (Contract × PaymentMethod × Tenure)
“Month-to-month + Electronic check + Tenure ≤ 6 months → 67.6% churn.”
“Month-to-month + Bank transfer (auto) + ≤ 6 months → 57.3%.”
“Month-to-month + Electronic check + 6–12 months → 51.8%.”
“Month-to-month + Electronic check + 12–24 months → 51.3%.”
“Month-to-month + Credit card (auto) + ≤ 6 months → 44.5%.”

![Churn Distribution](reports/Figures/churn_pie.png)
![Churn by Contract](reports/Figures/churn_by_contract_stacked_pct.png)
![Churn by Payment](reports/Figures/churn_by_payment_stacked_pct.png)
![Churn by Senior](reports/Figures/churn_by_senior_stacked_pct.png)
![Churn by Tenure](reports/Figures/churn_by_tenure_stacked_pct.png)

## Contract vs Churn (%)
| Contract       | No   | Yes  |
| -------------- | ---- | ---- |
| Month-to-month | 57.3 | 42.7 |
| One year       | 88.7 | 11.3 |
| Two year       | 97.2 | 2.8  |

## Tenure bucket vs Churn (%)
| Tenure | No   | Yes  |
| ------ | ---- | ---- |
| ≤ 6    | 47.1 | 52.9 |
| 6–12   | 64.1 | 35.9 |
| 12–24  | 71.3 | 28.7 |
| 24–60  | 81.7 | 18.3 |
| 60+    | 93.4 | 6.6  |

## Payment Method vs Churn (%)
| Payment Method            | No   | Yes  |
| ------------------------- | ---- | ---- |
| Electronic check          | 54.7 | 45.3 |
| Mailed check              | 80.9 | 19.1 |
| Bank transfer (automatic) | 83.3 | 16.7 |
| Credit card (automatic)   | 84.8 | 15.2 |



