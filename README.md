# Neeraj Thokala | Data Science & Machine Learning Portfolio

Welcome to my professional data science portfolio. This repository is a centralized home for six end-to-end projects across **Data Analytics, Data Science, Machine Learning Engineering, Experimentation, Forecasting, Recommendation Systems, Customer Analytics, and Fraud Detection**.

Each project is built to feel like a real workplace deliverable: reproducible code, business context, statistical rigor, clear reporting, visual outputs, tests, and stakeholder-ready documentation.

---

## About Me

I am a Data Science graduate from Penn State with experience in Python, SQL, Power BI, Tableau, Excel, AWS, statistics, machine learning, and analytics engineering. I focus on turning raw data into actionable insights, building reproducible workflows, and communicating technical findings clearly to business stakeholders.

This portfolio demonstrates my ability to work across the full data lifecycle:

* Framing business problems
* Generating or preparing realistic datasets
* Cleaning and validating data
* Writing analysis-ready code
* Performing statistical analysis
* Training and evaluating machine learning models
* Building visual reports and dashboards
* Creating production-style project documentation
* Translating results into business recommendations

---

## Featured Projects

| # | Project                     | Folder                         | Primary Role Focus                 | Status    |
| - | --------------------------- | ------------------------------ | ---------------------------------- | --------- |
| 1 | A/B Test Analysis Framework | `04-ab-test-analysis`          | Data Analyst / Data Scientist      | Completed |
| 2 | Customer Segmentation       | `09-customer-segmentation`     | Data Analyst / Marketing Analytics | Completed |
| 3 | Customer Churn Prediction   | `02-customer-churn-prediction` | Data Scientist                     | Completed |
| 4 | Time Series Forecasting     | `05-time-series-forecasting`   | Data Scientist                     | Completed |
| 5 | Recommendation System API   | `03-recommendation-system-api` | ML Engineer                        | Completed |
| 6 | Fraud Detection System      | `07-fraud-detection`           | ML Engineer / Risk Analytics       | Completed |

---

# Project 1: A/B Test Analysis Framework

**Folder:** `04-ab-test-analysis`
**Role Focus:** Data Analyst / Data Scientist
**Tools:** Python, SQL, Statistics, Bayesian Analysis, Power Analysis, Data Visualization
**Status:** Completed

## Overview

This project is a full A/B testing framework designed to evaluate whether a new product experience improves conversion rate compared to an existing control experience.

It includes realistic experiment simulation, statistical testing, Bayesian analysis, power analysis, segmentation, guardrail metrics, visualizations, SQL extraction examples, notebooks, tests, and an auto-generated executive report.

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

* A/B testing
* Hypothesis testing
* Confidence intervals
* Bayesian analysis
* Power analysis
* Guardrail metrics
* Segment analysis
* SQL-based experiment extraction
* Executive reporting

---

# Project 2: Customer Segmentation

**Folder:** `09-customer-segmentation`
**Role Focus:** Data Analyst / Marketing Analytics / Customer Analytics
**Tools:** Python, SQL, RFM Analysis, K-Means Clustering, Data Visualization
**Status:** Completed

## Overview

This project analyzes customer purchasing behavior and creates actionable marketing segments using synthetic CRM data, RFM scoring, K-Means clustering, cluster validation, customer profiling, recommendations, visualizations, a SQL extract, a notebook, a report, a model artifact, and tests.

The project is designed as a business-facing customer economics analysis that helps a marketing or growth team identify high-value customers, retention opportunities, and churn-risk segments.

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

The strongest business result: the top **27.8% of customers generate 74.8% of revenue**, showing a clear opportunity for targeted retention, loyalty, and upsell campaigns.

## Verification

```bash
python src/data_generator.py
python src/segment.py
python src/visualize.py
pytest -q
```

**Test Result:** `4 passed`

## Skills Demonstrated

* Customer segmentation
* RFM scoring
* K-Means clustering
* Cluster validation
* Marketing analytics
* Revenue concentration analysis
* Customer profiling
* Business recommendations

---

# Project 3: Customer Churn Prediction

**Folder:** `02-customer-churn-prediction`
**Role Focus:** Data Scientist
**Tools:** Python, scikit-learn, Feature Engineering, Model Evaluation, Streamlit
**Status:** Completed

## Overview

This project predicts customer churn using a synthetic IBM Telco-style fallback dataset. It includes preprocessing, feature engineering, model comparison, trained model artifacts, lift analysis, threshold evaluation, feature importance, Streamlit dashboard code, notebooks, a model card, a case study, a report, and tests.

The project is designed to show practical machine learning for customer retention and business decision-making.

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

The Streamlit dashboard code is included and ready, but Streamlit must be installed locally before launching the app.

## Skills Demonstrated

* Classification modeling
* Churn prediction
* Feature engineering
* Model comparison
* Threshold evaluation
* Lift analysis
* Model interpretation
* Streamlit dashboard development
* Model documentation

---

# Project 4: Time Series Forecasting

**Folder:** `05-time-series-forecasting`
**Role Focus:** Data Scientist / Forecasting Analyst
**Tools:** Python, SARIMA, ETS, Regression Forecasting, Ensemble Modeling
**Status:** Completed

## Overview

This project forecasts retail sales using synthetic retail time series data. It includes SARIMA, ETS, Prophet-like regression, inverse-MAPE ensemble forecasting, holdout evaluation, 90-day forecasts, prediction intervals, saved models, notebooks, reports, visuals, and tests.

The project is designed to show forecasting judgment, not just model fitting. It compares multiple approaches and explains why the best model fits the business context.

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

* Time series forecasting
* SARIMA modeling
* Exponential smoothing
* Forecast ensembles
* Prediction intervals
* Holdout validation
* Forecast accuracy evaluation
* Business forecasting recommendations

---

# Project 5: Recommendation System API

**Folder:** `03-recommendation-system-api`
**Role Focus:** Machine Learning Engineer
**Tools:** Python, SVD, FastAPI, Docker, Model Serialization, API Testing
**Status:** Completed

## Overview

This project builds a deployable recommendation system API using synthetic MovieLens-style data. It includes preprocessing, SVD-based collaborative filtering, serialized model artifacts, a FastAPI application, Dockerfile, docker-compose configuration, tests, notebooks, a report, and an API demo visual.

The project is designed to demonstrate not only modeling ability, but also ML engineering readiness through deployable API structure and low-latency recommendations.

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

The API code is ready, but FastAPI and Uvicorn must be installed locally or run through the included Docker setup before launching the service.

## Skills Demonstrated

* Recommendation systems
* Collaborative filtering
* SVD modeling
* API development
* FastAPI
* Docker
* Model serialization
* Latency benchmarking
* ML engineering project structure

---

# Project 6: Fraud Detection System

**Folder:** `07-fraud-detection`
**Role Focus:** Machine Learning Engineer / Risk Analytics
**Tools:** Python, Random Forest, Rare-Event Modeling, Cost-Sensitive Thresholding, Real-Time Scoring
**Status:** Completed

## Overview

This project builds a fraud and anomaly detection pipeline using realistic synthetic transaction data. It includes transaction generation, feature engineering, rare-event Random Forest modeling, threshold optimization, business impact analysis, prediction utilities, a visual dashboard, tests, a README, and a case study.

The project is designed to show an ML engineering workflow for a high-impact business problem where accuracy alone is not enough. The model must balance fraud capture, false positives, investigator workload, and business savings.

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

* Fraud detection
* Rare-event classification
* Feature engineering
* Random Forest modeling
* Precision-recall tradeoff analysis
* Cost-sensitive thresholding
* Real-time prediction utility
* Business impact estimation
* Investigator-ready outputs

---

## Technical Skills Demonstrated Across the Portfolio

| Skill Area                | Tools & Methods                                                                          |
| ------------------------- | ---------------------------------------------------------------------------------------- |
| Programming               | Python, SQL, Bash, Git                                                                   |
| Data Analysis             | pandas, NumPy, exploratory analysis, KPI analysis                                        |
| Statistics                | A/B testing, hypothesis testing, confidence intervals, Bayesian analysis, power analysis |
| Machine Learning          | Classification, clustering, recommendation systems, forecasting, anomaly detection       |
| ML Engineering            | FastAPI, Docker, serialized models, prediction utilities, API-ready architecture         |
| Visualization             | matplotlib, stakeholder-ready charts, dashboard-style visuals                            |
| Business Analytics        | Revenue impact, customer segmentation, churn risk, fraud savings, forecast planning      |
| Testing & Reproducibility | Seeded data generation, CLI pipelines, pytest, structured reports                        |
| Documentation             | README files, reports, case studies, model cards, executive summaries                    |

---

## Repository Structure

```text
data-science-portfolio/
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
└── 09-customer-segmentation/
    ├── README.md
    ├── src/
    ├── data/
    ├── models/
    ├── notebooks/
    └── tests/
```

---

## How to Run the Projects

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/data-science-portfolio.git
cd data-science-portfolio
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

## Why This Portfolio Is Different

This portfolio is intentionally built to avoid looking like a generic notebook collection. Each project includes:

* A clear business problem
* Reproducible data generation or preparation
* Modular Python source code
* Command-line execution
* Professional reports
* Visual outputs
* Tests
* Realistic metrics
* Business recommendations
* Recruiter-friendly documentation

The goal is to demonstrate job-ready execution for roles such as:

* Data Analyst
* Data Scientist
* Machine Learning Engineer
* Business Intelligence Analyst
* Product Analyst
* Marketing Analyst
* Risk Analytics Analyst

---

## Suggested Recruiter Review Path

For a quick review, start with:

1. `04-ab-test-analysis` for experimentation and statistics
2. `02-customer-churn-prediction` for applied machine learning
3. `03-recommendation-system-api` for ML engineering and deployment structure
4. `07-fraud-detection` for rare-event modeling and business impact
5. `09-customer-segmentation` for customer analytics
6. `05-time-series-forecasting` for forecasting and model comparison

---

## Contact

**Name:** Neeraj Thokala
**Email:** [neerajthokala@gmail.com](mailto:neerajthokala@gmail.com)
**GitHub:** `https://github.com/YOUR-USERNAME`
**LinkedIn:** `https://www.linkedin.com/in/YOUR-LINKEDIN/`

---

## License

This repository is for portfolio, educational, and demonstration purposes.

