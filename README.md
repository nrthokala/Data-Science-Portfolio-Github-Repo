# Neeraj Thokala | Data Science, BI & Machine Learning Portfolio

Welcome to my professional analytics portfolio. This repository brings together **8 projects** across data analytics, business intelligence, data science, machine learning engineering, experimentation, forecasting, customer analytics, pricing analytics, supply chain analytics, recommendation systems, and fraud detection.

Each project is designed to feel like a real workplace deliverable: reproducible code, realistic synthetic data, dashboard ready extracts, statistical rigor, machine learning pipelines, business case studies, visual outputs, testing, and stakeholder ready documentation.

---

## About Me

I am a Data Science graduate from Penn State with experience in Python, SQL, Power BI, Tableau, Excel, AWS, statistics, machine learning, and business analytics. I focus on turning raw data into clear, actionable insights through reproducible analysis, dashboards, reports, and business facing recommendations.

This portfolio demonstrates my ability to work across the full analytics lifecycle:

* Framing business problems
* Creating realistic synthetic datasets
* Cleaning and validating data
* Writing modular Python pipelines
* Performing statistical analysis and machine learning
* Building forecasting and optimization workflows
* Preparing Tableau and Power BI dashboard extracts
* Creating business case studies and reports
* Translating technical results into executive recommendations

---

## Portfolio Projects

| # | Project                                            | Folder                                           | Primary Role Focus                            | Status    |
| - | -------------------------------------------------- | ------------------------------------------------ | --------------------------------------------- | --------- |
| 1 | A/B Test Analysis Framework                        | `04-ab-test-analysis`                            | Data Analyst / Data Scientist                 | Completed |
| 2 | Customer Segmentation                              | `09-customer-segmentation`                       | Data Analyst / Marketing Analytics            | Completed |
| 3 | Customer Churn Prediction                          | `02-customer-churn-prediction`                   | Data Scientist                                | Completed |
| 4 | Time Series Forecasting                            | `05-time-series-forecasting`                     | Data Scientist / Forecasting Analyst          | Completed |
| 5 | Recommendation System API                          | `03-recommendation-system-api`                   | Machine Learning Engineer                     | Completed |
| 6 | Fraud Detection System                             | `07-fraud-detection`                             | ML Engineer / Risk Analytics                  | Completed |
| 7 | Supply Chain & Inventory Optimization Analyzer     | `08-supply-chain-inventory-optimization-tableau` | BI Analyst / Supply Chain Analyst             | Completed |
| 8 | Predictive Pricing & Discount Effectiveness Engine | `09-predictive-pricing-discount-engine-bi`       | BI Analyst / Pricing Analyst / Data Scientist | Completed |

---

# Project 1: A/B Test Analysis Framework

**Folder:** `04-ab-test-analysis`
**Role Focus:** Data Analyst / Data Scientist
**Tools:** Python, SQL, Statistics, Bayesian Analysis, Power Analysis, Data Visualization
**Status:** Completed

## Overview

An end to end A/B testing framework that evaluates whether a new product experience improves conversion rate compared to an existing control experience.

The project includes realistic experiment simulation, statistical testing, Bayesian analysis, power analysis, segmentation, guardrail metrics, SQL extraction examples, notebooks, tests, visualizations, and an auto generated executive report.

## Key Files

```text
04-ab-test-analysis/
├── README.md
├── src/
│   ├── data_generator.py
│   ├── analyze.py
│   ├── power_analysis.py
│   ├── statistics.py
│   └── visualization.py
├── ab_test_report.md
├── ab_test_results.png
├── notebooks/
├── docs/
├── data/
└── tests/
```

## Final Results

| Metric                          |                  Result |
| ------------------------------- | ----------------------: |
| Control Users                   |                  50,000 |
| Treatment Users                 |                  50,000 |
| Control Conversions             |                   5,421 |
| Treatment Conversions           |                   6,396 |
| Absolute Lift                   | +1.95 percentage points |
| Relative Improvement            |                  +18.0% |
| Estimated Annual Revenue Impact |                  ~$9.9M |

## Verification

```bash
python src/data_generator.py
python src/analyze.py
python src/power_analysis.py
pytest -q
```

**Test Result:** `4 passed`

## Skills Demonstrated

A/B testing, hypothesis testing, confidence intervals, Bayesian analysis, power analysis, guardrail metrics, segmentation, SQL extraction, and executive reporting.

---

# Project 2: Customer Segmentation

**Folder:** `09-customer-segmentation`
**Role Focus:** Data Analyst / Marketing Analytics / Customer Analytics
**Tools:** Python, SQL, RFM Analysis, K-Means Clustering, Data Visualization
**Status:** Completed

## Overview

A customer analytics project focused on customer economics and marketing activation using synthetic CRM data, RFM scoring, K-Means clustering, cluster validation, segment profiling, recommendations, visualizations, a SQL extract, a notebook, a model artifact, and tests.

## Key Files

```text
09-customer-segmentation/
├── README.md
├── src/
│   ├── data_generator.py
│   ├── segment.py
│   └── visualize.py
├── customer_segmentation_report.md
├── customer_segments.png
├── notebooks/
├── data/
├── models/
└── tests/
```

## Final Results

| Segment   | Share of Customers |
| --------- | -----------------: |
| Champions |               7.4% |
| Loyal     |              20.3% |
| Promising |              35.3% |
| At Risk   |              24.2% |
| Churned   |              12.8% |

## Business Insight

The top **27.8% of customers generate 74.8% of revenue**, creating a clear opportunity for targeted retention, loyalty, and upsell campaigns.

## Verification

```bash
python src/data_generator.py
python src/segment.py
python src/visualize.py
pytest -q
```

**Test Result:** `4 passed`

## Skills Demonstrated

Customer segmentation, RFM scoring, K-Means clustering, cluster validation, marketing analytics, revenue concentration analysis, customer profiling, and business recommendations.

---

# Project 3: Customer Churn Prediction

**Folder:** `02-customer-churn-prediction`
**Role Focus:** Data Scientist
**Tools:** Python, scikit-learn, Feature Engineering, Model Evaluation, Streamlit
**Status:** Completed

## Overview

A supervised machine learning project that predicts customer churn using a synthetic IBM Telco style fallback dataset. It includes preprocessing, feature engineering, model comparison, trained model artifacts, lift analysis, threshold evaluation, feature importance, Streamlit dashboard code, notebooks, a model card, a case study, a report, and tests.

## Key Files

```text
02-customer-churn-prediction/
├── README.md
├── src/
│   ├── preprocessing.py
│   ├── train.py
│   └── evaluate.py
├── app.py
├── churn_prediction_report.md
├── notebooks/
├── data/
├── models/
├── reports/
└── tests/
```

## Final Model Results

| Metric                         | Result |
| ------------------------------ | -----: |
| Holdout AUC-ROC                |  0.830 |
| Cross-Validated Best Model AUC |  0.841 |
| Average Precision              |  0.606 |
| Lift at Top 20%                |  2.29x |
| Recall at Top 20%              |  45.8% |

## Verification

```bash
python data/sample/generate_sample.py
python src/preprocessing.py
python src/train.py
python src/evaluate.py
pytest -q
```

**Test Result:** `4 passed`

## Note

The Streamlit dashboard code is included and ready. Streamlit must be installed locally before launching the app.

## Skills Demonstrated

Classification modeling, churn prediction, preprocessing, feature engineering, model comparison, threshold evaluation, lift analysis, model interpretation, Streamlit dashboarding, and model documentation.

---

# Project 4: Time Series Forecasting

**Folder:** `05-time-series-forecasting`
**Role Focus:** Data Scientist / Forecasting Analyst
**Tools:** Python, SARIMA, ETS, Regression Forecasting, Ensemble Modeling
**Status:** Completed

## Overview

A professional forecasting project using synthetic retail sales data. It includes SARIMA, ETS, Prophet like regression, inverse MAPE ensemble forecasting, holdout evaluation, 90 day forecasts, prediction intervals, saved models, notebooks, reports, visuals, and tests.

## Key Files

```text
05-time-series-forecasting/
├── README.md
├── src/
│   ├── data_generator.py
│   ├── models.py
│   ├── train.py
│   └── visualize.py
├── forecasting_report.md
├── forecast_results.png
├── notebooks/
├── data/
├── models/
└── tests/
```

## Final Model Results

| Model                   |   MAPE | Coverage |
| ----------------------- | -----: | -------: |
| ETS                     | 14.13% |    96.7% |
| Ensemble                | 14.61% |    96.7% |
| SARIMA                  | 14.93% |   100.0% |
| Prophet-like Regression | 15.13% |    93.3% |

## Best Model

The best model was **ETS**, which fits the business story well: stable recurring retail seasonality where a clean exponential smoothing model beats more complex approaches.

## Verification

```bash
python src/data_generator.py
python src/train.py
python src/visualize.py
pytest -q
```

**Test Result:** `4 passed`

## Skills Demonstrated

Time series forecasting, SARIMA modeling, exponential smoothing, forecast ensembles, prediction intervals, holdout validation, forecast accuracy evaluation, and business forecasting recommendations.

---

# Project 5: Recommendation System API

**Folder:** `03-recommendation-system-api`
**Role Focus:** Machine Learning Engineer
**Tools:** Python, SVD, FastAPI, Docker, Model Serialization, API Testing
**Status:** Completed

## Overview

A deployable recommendation API using synthetic MovieLens style data. It includes preprocessing, SVD based collaborative filtering, serialized model artifacts, a FastAPI app, Dockerfile, docker compose file, tests, notebooks, report, and API demo visual.

## Key Files

```text
03-recommendation-system-api/
├── README.md
├── src/
│   ├── preprocessing.py
│   ├── train.py
│   ├── models.py
│   └── visualize.py
├── main.py
├── Dockerfile
├── docker-compose.yml
├── recommendation_api_report.md
├── notebooks/
├── data/
├── models/
└── tests/
```

## Final Metrics

| Metric                     | Result |
| -------------------------- | -----: |
| RMSE                       |  0.937 |
| MAE                        |  0.774 |
| Training Time              |  0.51s |
| Recommendation Latency p50 | 0.08ms |
| Recommendation Latency p99 | 0.26ms |
| Data Sparsity              |  93.7% |

## Verification

```bash
python data/sample/generate_sample.py
python src/preprocessing.py
python src/train.py
python src/visualize.py
pytest -q
```

**Test Result:** `3 passed, 1 skipped`

## Note

The API code is ready. FastAPI and Uvicorn must be installed locally, or the project can be run through the included Docker setup.

## Skills Demonstrated

Recommendation systems, collaborative filtering, SVD modeling, FastAPI development, Docker, model serialization, latency benchmarking, and ML engineering project structure.

---

# Project 6: Fraud Detection System

**Folder:** `07-fraud-detection`
**Role Focus:** Machine Learning Engineer / Risk Analytics
**Tools:** Python, Random Forest, Rare-Event Modeling, Cost-Sensitive Thresholding, Real-Time Scoring
**Status:** Completed

## Overview

A fraud and anomaly detection pipeline using realistic synthetic transaction data. It includes transaction generation, feature engineering, rare event Random Forest modeling, threshold optimization, business impact analysis, prediction utilities, a visual dashboard, tests, README, and case study.

## Key Files

```text
07-fraud-detection/
├── README.md
├── case_study.md
├── src/
│   ├── data_generator.py
│   ├── features.py
│   ├── train.py
│   ├── predict.py
│   └── visualize.py
├── fraud_detection_report.md
├── fraud_detection.png
├── data/
├── models/
└── tests/
```

## Final Model Results

| Metric                   | Result |
| ------------------------ | -----: |
| Accuracy                 | 99.86% |
| Precision                |  59.4% |
| Recall                   |  55.9% |
| F1 Score                 |  0.576 |
| ROC-AUC                  |  0.998 |
| PR-AUC                   |  0.573 |
| Optimized Threshold      |   0.67 |
| Estimated Annual Savings | $2.83M |

## Verification

```bash
python src/data_generator.py
python src/features.py
python src/train.py
python src/visualize.py
pytest -q
```

**Test Result:** `3 passed`

## Skills Demonstrated

Fraud detection, rare event classification, feature engineering, Random Forest modeling, precision recall tradeoff analysis, cost sensitive thresholding, real time prediction utility, business impact estimation, and investigator ready outputs.

---

# Project 7: Supply Chain & Inventory Optimization Analyzer

**Folder:** `08-supply-chain-inventory-optimization-tableau`
**Role Focus:** BI Analyst / Supply Chain Analyst / Data Analyst
**Tools:** Python, Tableau, Forecasting, Inventory Analytics, KPI Reporting
**Status:** Completed

## Overview

A supply chain analytics project that analyzes warehouse, SKU, inventory, and order data to identify stockout risk, optimize reorder planning, calculate safety stock, and prepare dashboard-ready extracts for Tableau.

The project is designed as a realistic business intelligence deliverable for stakeholders who need visibility into inventory risk, demand patterns, warehouse performance, and expedite cost exposure.

## Included Components

* Synthetic warehouse, SKU, inventory, and order data
* 30 day demand forecast
* Safety stock calculations
* Reorder point calculations
* Warehouse SKU stockout risk scoring
* Tableau dashboard guide
* Tableau calculated fields
* Case study and README
* Dashboard ready CSV extracts

## Key Outputs

| Output File                       |     Shape | Purpose                                                                                 |
| --------------------------------- | --------: | --------------------------------------------------------------------------------------- |
| `inventory_dashboard_extract.csv` |   72 x 24 | Main Tableau dashboard extract with inventory, risk, reorder, and warehouse-SKU metrics |
| `demand_forecast_30d.csv`         | 2,160 x 4 | 30-day SKU-level demand forecast for planning and replenishment views                   |

## Final Business Results

| Metric                  |                 Result |
| ----------------------- | ---------------------: |
| Critical Stockout Risks |                     17 |
| At-Risk Inventory Value |               $913,208 |
| Expedite Cost Exposure  |               $100,381 |
| Main Dashboard Extract  |   72 rows x 24 columns |
| Forecast Output         | 2,160 rows x 4 columns |

## Verification

```bash
cd 08-supply-chain-inventory-optimization-tableau
python src/data_generator.py
python src/forecast_inventory.py
```

**Verification Result:** Extract shape checks passed.

## Skills Demonstrated

Tableau dashboard preparation, inventory optimization, demand forecasting, safety stock calculation, reorder point logic, stockout risk scoring, supply chain KPI design, dashboard-ready data modeling, and executive analytics communication.

---

# Project 8: Predictive Pricing & Discount Effectiveness Engine

**Folder:** `09-predictive-pricing-discount-engine-bi`
**Role Focus:** BI Analyst / Pricing Analyst / Data Scientist
**Tools:** Python, Tableau, Power BI, DAX, Regression Modeling, Pricing Analytics
**Status:** Completed

## Overview

A pricing analytics and BI project that analyzes weekly pricing and promotion data to estimate price elasticity, evaluate discount effectiveness, simulate discount scenarios, and identify profit maximizing discount strategies.

The project is designed as a business facing pricing engine for teams that need to understand how price changes, promotions, and discounts affect unit demand, revenue, and profit.

## Included Components

* Synthetic weekly pricing and promotion data
* Log-log regression model for price elasticity
* Product level elasticity summary
* Discount scenario simulation from 0% to 40%
* Tableau calculated fields
* Power BI DAX measures
* Dashboard build guide
* Case study and README
* Dashboard ready CSV extracts

## Key Outputs

| Output File                      |      Shape | Purpose                                                                                           |
| -------------------------------- | ---------: | ------------------------------------------------------------------------------------------------- |
| `dashboard_extract.csv`          | 5,200 x 21 | Main pricing dashboard extract with weekly product, price, promotion, revenue, and profit metrics |
| `discount_scenarios.csv`         |   410 x 14 | Simulated discount scenarios from 0% to 40% for pricing optimization                              |
| `product_elasticity_summary.csv` |    10 x 11 | Product-level elasticity and pricing performance summary                                          |

## Final Business Results

| Metric                             |                  Result |
| ---------------------------------- | ----------------------: |
| Global Price Elasticity            |                   -1.70 |
| Regression R-Squared               |                   0.876 |
| Average Profit-Maximizing Discount |                    9.7% |
| Dashboard Extract                  | 5,200 rows x 21 columns |
| Discount Scenario Output           |   410 rows x 14 columns |
| Product Elasticity Summary         |    10 rows x 11 columns |

## Verification

```bash
cd 09-predictive-pricing-discount-engine-bi
python src/data_generator.py
python src/pricing_model.py
```

**Verification Result:** Extract shape checks passed.

## Skills Demonstrated

Pricing analytics, price elasticity modeling, log-log regression, discount scenario simulation, Tableau dashboard design, Power BI DAX measures, promotion effectiveness analysis, profit optimization, and executive analytics communication.

---

## Technical Skills Demonstrated Across the Portfolio

| Skill Area                | Tools & Methods                                                                               |
| ------------------------- | --------------------------------------------------------------------------------------------- |
| Programming               | Python, SQL-ready workflows, Bash, Git                                                        |
| Business Intelligence     | Tableau, Power BI, dashboard extracts, calculated fields, DAX measures                        |
| Data Analysis             | pandas, NumPy, exploratory analysis, KPI design, operational analysis                         |
| Statistics                | A/B testing, hypothesis testing, confidence intervals, Bayesian analysis, power analysis      |
| Machine Learning          | Classification, clustering, recommendation systems, forecasting, anomaly detection            |
| ML Engineering            | FastAPI, Docker, serialized models, prediction utilities, API-ready architecture              |
| Forecasting               | Time series modeling, demand forecasting, prediction intervals, model comparison              |
| Supply Chain Analytics    | Safety stock, reorder points, stockout risk, inventory value exposure                         |
| Pricing Analytics         | Price elasticity, discount optimization, promotion effectiveness, profit-maximizing scenarios |
| Risk Analytics            | Fraud detection, rare-event modeling, threshold optimization, business savings estimation     |
| Visualization             | Tableau guides, Power BI measures, matplotlib visuals, executive KPI layouts                  |
| Testing & Reproducibility | Seeded data generation, CLI pipelines, pytest, validation checks                              |
| Documentation             | README files, case studies, reports, model cards, dashboard guides, executive summaries       |

---

## Repository Structure

```text
data-science-bi-ml-portfolio/
│
├── README.md
│
├── 02-customer-churn-prediction/
│   ├── README.md
│   ├── app.py
│   ├── src/
│   ├── data/
│   ├── models/
│   ├── notebooks/
│   ├── reports/
│   └── tests/
│
├── 03-recommendation-system-api/
│   ├── README.md
│   ├── main.py
│   ├── Dockerfile
│   ├── docker-compose.yml
│   ├── src/
│   ├── data/
│   ├── models/
│   ├── notebooks/
│   └── tests/
│
├── 04-ab-test-analysis/
│   ├── README.md
│   ├── src/
│   ├── notebooks/
│   ├── data/
│   ├── docs/
│   ├── reports/
│   └── tests/
│
├── 05-time-series-forecasting/
│   ├── README.md
│   ├── src/
│   ├── data/
│   ├── models/
│   ├── notebooks/
│   ├── reports/
│   └── tests/
│
├── 07-fraud-detection/
│   ├── README.md
│   ├── case_study.md
│   ├── src/
│   ├── data/
│   ├── models/
│   └── tests/
│
├── 08-supply-chain-inventory-optimization-tableau/
│   ├── README.md
│   ├── case_study.md
│   ├── src/
│   │   ├── data_generator.py
│   │   └── forecast_inventory.py
│   ├── data/
│   │   ├── inventory_dashboard_extract.csv
│   │   └── demand_forecast_30d.csv
│   ├── docs/
│   │   ├── tableau_dashboard_guide.md
│   │   └── tableau_calculated_fields.md
│   └── outputs/
│
├── 09-customer-segmentation/
│   ├── README.md
│   ├── src/
│   ├── data/
│   ├── models/
│   ├── notebooks/
│   └── tests/
│
└── 09-predictive-pricing-discount-engine-bi/
    ├── README.md
    ├── case_study.md
    ├── src/
    │   ├── data_generator.py
    │   └── pricing_model.py
    ├── data/
    │   ├── dashboard_extract.csv
    │   ├── discount_scenarios.csv
    │   └── product_elasticity_summary.csv
    ├── docs/
    │   ├── tableau_calculated_fields.md
    │   ├── power_bi_dax_measures.md
    │   └── dashboard_build_guide.md
    └── outputs/
```

---

## How to Run the Portfolio

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/data-science-bi-ml-portfolio.git
cd data-science-bi-ml-portfolio
```

Create and activate a virtual environment:

```bash
python -m venv venv
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Navigate into any project folder and follow that project’s `README.md` instructions.

Example:

```bash
cd 04-ab-test-analysis
python src/data_generator.py
python src/analyze.py
pytest -q
```

---

## Verification Summary

| Project                               | Verification                      |
| ------------------------------------- | --------------------------------- |
| A/B Test Analysis Framework           | `pytest -q` → 4 passed            |
| Customer Segmentation                 | `pytest -q` → 4 passed            |
| Customer Churn Prediction             | `pytest -q` → 4 passed            |
| Time Series Forecasting               | `pytest -q` → 4 passed            |
| Recommendation System API             | `pytest -q` → 3 passed, 1 skipped |
| Fraud Detection System                | `pytest -q` → 3 passed            |
| Supply Chain & Inventory Optimization | Extract shape checks passed       |
| Predictive Pricing & Discount Engine  | Extract shape checks passed       |

---

## Why This Portfolio Is Different

This portfolio is intentionally built to avoid looking like a generic notebook collection. The projects are structured like professional analytics, BI, data science, and ML engineering deliverables.

Each project includes some combination of:

* A clear business problem
* Realistic synthetic data
* Modular Python source code
* Command line execution
* Dashboard ready CSV extracts
* Tableau or Power BI implementation guidance
* Professional reports and case studies
* Model artifacts or analysis outputs
* Visualizations
* Tests or validation checks
* Business recommendations
* Recruiter friendly documentation

---

## Suggested Recruiter Review Path

For a quick review, start with:

1. `04-ab-test-analysis` — experimentation, statistics, and executive reporting
2. `02-customer-churn-prediction` — applied machine learning and retention analytics
3. `03-recommendation-system-api` — ML engineering, API structure, and Docker readiness
4. `07-fraud-detection` — rare-event modeling and business impact analysis
5. `08-supply-chain-inventory-optimization-tableau` — Tableau, supply chain analytics, and forecasting
6. `09-predictive-pricing-discount-engine-bi` — pricing analytics, Power BI / Tableau, and regression modeling
7. `09-customer-segmentation` — customer analytics and marketing activation
8. `05-time-series-forecasting` — forecasting, model comparison, and planning recommendations

---

## Target Roles

This portfolio is especially relevant for roles such as:

* Data Analyst
* Business Intelligence Analyst
* Data Scientist
* Machine Learning Engineer
* Product Analyst
* Marketing Analyst
* Pricing Analyst
* Supply Chain Analyst
* Operations Analyst
* Risk Analytics Analyst
* Analytics Engineer

---

## Contact

**Name:** Neeraj Thokala
**Email:** [neerajthokala@gmail.com](mailto:neerajthokala@gmail.com)
**GitHub:** `https://github.com/nrthokala`
**LinkedIn:** `https://www.linkedin.com/in/neeraj-thokala/`

---

## License

This repository is for portfolio, educational, and demonstration purposes.
