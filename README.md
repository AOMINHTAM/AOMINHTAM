# Hi there, I'm Ao Minh Tâm 👋
### 🚀 Data Analyst | Data Engineer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Ao_Minh_Tâm-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ao-minh-tam/)
[![Portfolio](https://img.shields.io/badge/Portfolio-Live_Website-F59E0B?style=flat&logo=google-chrome&logoColor=white)](https://aominhtam-portfolio.vercel.app/)
[![Credential](https://img.shields.io/badge/dbt_Labs-Verified_Credential-FF694B?style=flat&logo=dbt&logoColor=white)](https://credentials.getdbt.com/daf3523f-38ca-48fe-9b95-548d6ca7da8d)
[![Gmail](https://img.shields.io/badge/Email-aominhtam%40gmail.com-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:aominhtam@gmail.com)

I am a **Third-Year IT Undergraduate** (2024 – Expected 2028) at Ho Chi Minh City University of Natural Resources and Environment (HCMUNRE), focused on **Data Analytics (DA)** and **Data Engineering (DE)**. I use SQL, Python, Power BI, and modern cloud data tools (**AWS**, **Snowflake**, **Airflow 3**, **dbt Core**) to turn raw data into reliable datasets, actionable insights, and testable business recommendations.

---

### 🛠️ Tech Stack & Tooling

| Domain | Technologies & Libraries |
| :--- | :--- |
| **Data Analytics & BI** | `SQL (Joins, CTEs, Window Functions)` • `Python (Pandas, NumPy, SciPy, mlxtend)` • `Power BI (DAX, Power Query)` • `Microsoft Excel` |
| **Visualization & Methods** | `Plotly (Sankey, Funnel)` • `Seaborn` • `Matplotlib` • `squarify` • `RFM` • `Cohort Retention` • `Apriori` • `Pareto ABC` • `IQR Auditing` |
| **Cloud & Warehousing** | `AWS (CloudFormation IaC, S3 Versioning, SQS + DLQ, CloudWatch, SNS, Redshift Serverless, IAM)` • `Snowflake Data Cloud` |
| **Orchestration, Modeling & CI** | `Apache Airflow 3 (AssetWatcher, Astro CLI, Cosmos)` • `dbt Core` • `Kimball Star Schema` • `Docker` • `GitHub Actions CI (Ruff, cfn-lint, Pytest)` |

---

### 📜 Verified Credentials

* 🏅 **[dbt Fundamentals Certified](https://credentials.getdbt.com/daf3523f-38ca-48fe-9b95-548d6ca7da8d)** — *Issued by dbt Labs (Credential ID: `daf3523f-38ca-48fe-9b95-548d6ca7da8d`)*  
  *Demonstrates core competency in modular SQL models, incremental materializations, automated schema/data quality testing, and DAG lineage documentation using dbt Core and dbt Cloud.*

---

### 📂 Featured Open-Source Technical Projects

#### 🏗️ 1. Cloud Data Engineering Pipelines
* **[aws-data-pipeline](https://github.com/AOMINHTAM/aws-data-pipeline)** *(V5.0.1 — CloudFormation IaC, Event-Driven ELT & CloudOps)*
  * *Stack: AWS (CloudFormation, S3, SQS + DLQ, CloudWatch, SNS, Redshift Serverless, IAM), Airflow 3 (`AssetWatcher`, Cosmos), dbt Core, Docker, Pytest*
  * Provisioned declarative AWS CloudFormation IaC (15 core + 4 conditional resources) ingesting **99,441 Olist orders** (`~120 MB`). Replaced cron polling with **Airflow 3 `AssetWatcher`** (`20s` SQS Long Polling, 0 empty runs), Two-Phase atomic `TEMP TABLE` swaps with CSV header &amp; empty-stage guards, `ops.pipeline_ingestion_audit` Safe ACK (`900s`), SQS DLQ (`maxReceiveCount=3`), 4 CloudWatch Alarms + SNS email, and 11 dbt schema tests (**5.0.0** live-verified on AWS `17/17` tasks + DLQ Redrive; **5.0.1** passing `21/21` unit tests &amp; 3-job CI).
* **[dbt-snowflake-data-pipeline](https://github.com/AOMINHTAM/dbt-snowflake-data-pipeline)**
  * *Stack: Snowflake, dbt Core, Apache Airflow (Astronomer Cosmos), Docker, Python, SQL*
  * Automated cloud ELT platform orchestrating Snowflake transformations via containerized Airflow &amp; Astronomer Cosmos inside an isolated `dbt_venv` on TPC-H benchmark data. Modeled Medallion Staging &amp; Kimball Star Schema marts speeding queries by ~35% vs. normalized joins with automated schema/referential checks.

#### 📊 2. Commercial Analytics & Customer Intelligence
* **[customer-rfm-segmentation-analysis](https://github.com/AOMINHTAM/customer-rfm-segmentation-analysis)**
  * *Stack: Python, Pandas, NumPy, Seaborn, squarify*
  * Quantile RFM segmentation (`pd.qcut`) across **51,290 line-items** (`25,728` unique orders, `17,415` customers, 2020–2023 simulated dataset). Proved top 2 tiers (&lt;29% of users) generate &gt;53% of revenue (`Champions`: 13.56% users / 32.8% revenue), isolated 833 *Cant-Lose* accounts (4.78% users, 10.0% value), and formulated A/B-testable campaign hypotheses.
* **[abc-inventory-analysis](https://github.com/AOMINHTAM/abc-inventory-analysis)**
  * *Stack: Python, Pandas, NumPy, Seaborn, Matplotlib, IQR Anomaly Auditing*
  * Pareto ABC profit segmentation across **51,290 transactions** (`25,728` orders, `17,415` accounts, 2020–2023), proving 12.94% of Group A VIPs (2,254 users) generate 80% of cumulative net profit. Audited a 500-gift budget shortfall (1,754 gap) to propose a measurable tiered physical-plus-digital retention pilot.
* **[cohort-retention-analysis](https://github.com/AOMINHTAM/cohort-retention-analysis)**
  * *Stack: Python, Pandas, NumPy, Seaborn, Matplotlib*
  * Time-based cohort retention heatmaps across B2B/B2C segments (51,290 transactions, 2020–2023) exposing a 1%–3% Month-1 drop-off cliff. Eliminated left-truncation bias by anchoring `FirstPurchaseDate` globally across `df_sales` and uncovered B2B cyclical restock bumps (5%–6% at Months 5 and 8).

#### 🛒 3. E-Commerce Diagnostics, Funnels & Network Flows
* **[product-conversion-funnel-analysis](https://github.com/AOMINHTAM/product-conversion-funnel-analysis)**
  * *Stack: Python, Plotly (Funnel), Pandas, NumPy, Seaborn*
  * Session-level conversion funnels across **472,871 sessions** and **32,313 orders** (Maven Fuzzy Factory, 2012–2015). Calculated Net Revenue After Refunds, uncovered the *"Love Bear Paradox"* (10.0% catalog share vs. 55.6% cart-add rate) and a 66% checkout abandonment bottleneck, proposing A/B recovery flows.
* **[user-journey-sankey-analysis](https://github.com/AOMINHTAM/user-journey-sankey-analysis)**
  * *Stack: Python, Plotly (Sankey), Pandas, NumPy*
  * Interactive Plotly Sankey DAGs across **1.18M+ pageview records** (`472,871` sessions, `32,313` orders). Eliminated circular DAG crashes via `.rank()` prefixes, reduced join RAM bloat with `usecols` and pre-aggregation, and pinpointed mobile drop-off and cross-sell paths (`Mr. Fuzzy -> Love Bear`).
* **[market-basket-analysis](https://github.com/AOMINHTAM/market-basket-analysis)**
  * *Stack: Python, mlxtend (Apriori), TransactionEncoder, Pandas, NumPy, Seaborn*
  * Apriori association rules mining (0.5% min support) with basket deduplication across `25,728` baskets preventing OOM crashes. Surfaced high-affinity cross-sell pairs (Lift up to 4.25, 45% confidence) to design A/B bundle hypotheses.
* **[pareto-revenue-analysis](https://github.com/AOMINHTAM/pareto-revenue-analysis)**
  * *Stack: Python, Pandas, NumPy, Matplotlib, Seaborn*
  * Quantified SKU-level Net Revenue After Refunds across **32,313 orders** (Maven Fuzzy Factory, 2012–2015) using Pareto 80/20 `cumsum` curves. Validated that 3 core SKUs drive ~82% of net revenue (with 1 flagship SKU holding 45.2% concentration risk).

---

### 📈 GitHub Analytics & Activity

<p align="center">
  <img src="https://github-stats-extended.vercel.app/api?username=AOMINHTAM&show_icons=true&theme=radical&hide_border=true&title_color=f59e0b&icon_color=f59e0b&count_private=true" alt="Ao Minh Tâm's GitHub Stats" width="48%" />
  <img src="https://github-stats-extended.vercel.app/api/top-langs/?username=AOMINHTAM&layout=compact&theme=radical&hide_border=true&title_color=f59e0b&hide=html,css" alt="Top Languages" width="48%" />
</p>

---

<p align="center">
  <i>📍 Ho Chi Minh City, Vietnam • Open to Data Analyst &amp; Data Engineer Intern Opportunities</i>
</p>
