## Repository contents

| File | Description |
|---|---|
| `fraud_detection.ipynb` | Main notebook: EDA, silver and gold tables, features (Parts 2-3). Later parts will be added here. |
| `<kaggle_loader>.ipynb` | Downloads the full Kaggle dataset (2010-2019) and loads it into Databricks. |
| `README.md` | Project overview, results and screenshots. |

## Screenshots

### Part 2: EDA
![Fraud rate by month](images/eda_fraud_by_month.png)
*Fraud rate by month. The rate is not stable over time.*

![Fraud rate by hour](images/eda_fraud_by_hour.png)
*Fraud rate by hour of day. Fraud peaks at night (3:00-5:00).*

![Fraud rate by transaction type](images/eda_fraud_by_type.png)
*Fraud rate by transaction type. Online transactions are far riskier than swipe.*

![Amounts, fraud vs normal](images/eda_amounts.png)
*Transaction amounts: fraudulent transactions are larger (median and p95).*

### Part 3: tables and features
![Medallion layers](images/layers.png)
*Bronze, silver and gold tables in Unity Catalog.*

![Gold features check](images/gold_check.png)
*`gold_fraud_features`: 8,914,963 rows (one per labelled transaction), 13,332 fraud.*
