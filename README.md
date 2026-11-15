# Hi there, I'm Ao Minh Tâm 👋
### 🚀 Data Analyst | Data Engineer | Analytics Engineer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Ao_Minh_Tâm-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ao-minh-tam/)
[![Portfolio](https://img.shields.io/badge/Portfolio-Live_Website-F59E0B?style=flat&logo=google-chrome&logoColor=white)](https://aominhtam-portfolio.vercel.app/)
[![Credential](https://img.shields.io/badge/dbt_Labs-Verified_Credential-FF694B?style=flat&logo=dbt&logoColor=white)](https://credentials.getdbt.com/daf3523f-38ca-48fe-9b95-548d6ca7da8d)
[![Gmail](https://img.shields.io/badge/Email-aominhtam%40gmail.com-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:aominhtam@gmail.com)

I am a **Third-Year IT Undergraduate** (2024 – Expected 2028) at Ho Chi Minh City University of Natural Resources and Environment (HCMUNRE), bridging **Data Analysis (DA)**, **Data Engineering (DE)**, and **Analytics Engineering (AE)**. I design event-driven Cloud ELT pipelines on **AWS** and **Snowflake**, build modular **dbt & Kimball Star Schema** data marts with automated quality tests, and translate e-commerce behavioral data into actionable unit-economic decisions.

---

### 🛠️ Tech Stack & Tooling

| Domain | Technologies & Libraries |
| :--- | :--- |
| **Cloud & Data Infrastructure** | `AWS (S3, SQS, Redshift Serverless, IAM)` • `Snowflake Data Cloud` • `Docker` • `Linux (Ubuntu WSL2)` |
| **Orchestration & Analytics Eng.** | `Apache Airflow 3 (Astro CLI, Astronomer Cosmos)` • `dbt (Core & Cloud)` • `Kimball Star Schema` • `Medallion Architecture` |
| **Languages & Data Processing** | `Advanced SQL (CTEs, Window Functions)` • `Python (Pandas, NumPy, SciPy, mlxtend)` • `Git / GitHub` |
| **BI & Visualization** | `Plotly (Sankey, Funnel)` • `Seaborn` • `Matplotlib` • `squarify` • `Power BI` • `Microsoft Excel (Pivot, Power Query)` |
| **Analytical Methods** | `RFM Segmentation` • `Cohort Retention` • `Conversion Funnels` • `Apriori Market Basket` • `Pareto (80/20) ABC` • `IQR Auditing` |

---

### 📜 Verified Credentials

* 🏅 **[dbt Fundamentals Certified](https://credentials.getdbt.com/daf3523f-38ca-48fe-9b95-548d6ca7da8d)** — *Issued by dbt Labs (Credential ID: `daf3523f-38ca-48fe-9b95-548d6ca7da8d`)*  
  *Demonstrates verified competency in modular SQL models, incremental materializations, automated schema/data quality testing, and DAG lineage documentation using dbt Core and dbt Cloud.*

---

### 📂 Featured Open-Source Technical Projects

#### 🏗️ 1. Cloud Data Engineering & Analytics Engineering Pipelines
* **[aws-data-pipeline](https://github.com/AOMINHTAM/aws-data-pipeline)** *(Flagship Event-Driven ELT)*
  * *Stack: AWS (S3, SQS, Redshift Serverless, IAM), Apache Airflow 3 (Astro CLI, Cosmos), dbt Core, Docker, SQL*
  * Architected push-based ELT ingesting 100,000+ Olist orders with zero S3 `LIST` overhead. Built Airflow 3 `SqsSensor` orchestration (45s timeout, `soft_fail`) skipping idle runs for `$0` Redshift RPU compute cost, enforced 4-RPU guardrails cutting warehouse spend by 50%, and passed 9/9 automated dbt tests across incremental Star Schema marts (`delete+insert`, 3-day lookback).
* **[dbt-snowflake-data-pipeline](https://github.com/AOMINHTAM/dbt-snowflake-data-pipeline)**
  * *Stack: dbt Core, Snowflake, Apache Airflow (Astronomer Cosmos), Docker, Python, SQL*
  * Automated cloud ELT platform orchestrating Snowflake transformations via containerized Airflow & Astronomer Cosmos inside an isolated `dbt_venv`. Eliminated 100% of manual runs, engineered Medallion Staging and Kimball Star Schema marts speeding downstream queries by 35%, and guaranteed 100% data reliability.

#### 📊 2. Commercial Analytics & Customer Intelligence
* **[customer-rfm-segmentation-analysis](https://github.com/AOMINHTAM/customer-rfm-segmentation-analysis)**
  * *Stack: Python, Pandas, NumPy, Seaborn, squarify*
  * Quantile RFM segmentation (`pd.qcut`) across 51,290 orders and 17,415 customers. Proved top 2 tiers (<29% of users) generate >53% of revenue (`Champions`: 13.56% users / 32.8% revenue), isolated 833 *Cant-Lose* accounts (4.78% users, 10.0% value), and profiled ages 25–49 driving >60% of sales.
* **[abc-inventory-analysis](https://github.com/AOMINHTAM/abc-inventory-analysis)**
  * *Stack: Python, Pandas, NumPy, Seaborn, Matplotlib, IQR Anomaly Auditing*
  * Pareto ABC profit segmentation across 51,290 transactions and 17,415 customer accounts, proving 12.94% of Group A VIPs (2,254 users) generate 80% of cumulative net profit. Audited a 500-gift budget shortfall (1,754 gap) to design a tiered physical-plus-digital retention rollout.
* **[cohort-retention-analysis](https://github.com/AOMINHTAM/cohort-retention-analysis)**
  * *Stack: Python, Pandas, NumPy, Seaborn, Matplotlib*
  * Time-based cohort retention heatmaps across B2B/B2C segments exposing a 1%–3% Month-1 drop-off cliff. Eliminated left-truncation bias by anchoring `FirstPurchaseDate` globally across `df_sales` and uncovered B2B cyclical restock bumps (5%–6% at Months 5 and 8) to propose Day 20–25 nurture flows and Month 4/7 CRM alerts.

#### 🛒 3. E-Commerce Diagnostics, Funnels & Network Flows
* **[user-journey-sankey-analysis](https://github.com/AOMINHTAM/user-journey-sankey-analysis)**
  * *Stack: Python, Plotly (Sankey), Pandas, NumPy*
  * Interactive Plotly Sankey diagrams mapping multi-step acquisition and repeat-purchase flows across 1M+ pageview records. Eliminated circular DAG crashes via chronological `.rank()` prefixes, reduced join RAM bloat with `usecols` and pre-aggregation, and pinpointed mobile drop-off and cross-sell paths (`Mr. Fuzzy -> Love Bear`) for 14-day CRM triggers.
* **[product-conversion-funnel-analysis](https://github.com/AOMINHTAM/product-conversion-funnel-analysis)**
  * *Stack: Python, Plotly (Funnel), Pandas, NumPy, Seaborn*
  * Session-level conversion funnels tracking Catalog-to-Checkout survival across flagship product lines. Uncovered the *"Love Bear Paradox"* (10.0% catalog share vs. 55.6% cart-add rate, vs. *Mr. Fuzzy* at 62.2% / 43.0%) and a 66% checkout abandonment bottleneck, proposing 1h/24h retargeting flows.
* **[market-basket-analysis](https://github.com/AOMINHTAM/market-basket-analysis)**
  * *Stack: Python, mlxtend (Apriori), TransactionEncoder, Pandas, NumPy, Seaborn*
  * Apriori association rules mining (0.5% min support) with basket-level deduplication preventing 100% of OOM crashes. Surfaced high-affinity cross-sell pairs (Lift up to 4.25, 45% confidence) across Home Spa and Wellness ecosystems to design a 10% discounted 4-item bundle boosting AOV.
* **[pareto-revenue-analysis](https://github.com/AOMINHTAM/pareto-revenue-analysis)**
  * *Stack: Python, Pandas, NumPy, Matplotlib, Seaborn*
  * Quantified SKU-level net revenue after refunds across 32,000+ e-commerce orders using Pareto 80/20 `cumsum` curves. Validated that 3 core SKUs drive ~82% of net revenue (with 1 flagship SKU holding 45.2% concentration risk), recommending safety-stock guardrails and reallocating 70%–80% of paid ad spend.

---

### 📈 GitHub Analytics & Activity

<p align="center">
  <img src="https://github-stats-extended.vercel.app/api?username=AOMINHTAM&show_icons=true&theme=radical&hide_border=true&title_color=f59e0b&icon_color=f59e0b&count_private=true" alt="Ao Minh Tâm's GitHub Stats" width="48%" />
  <img src="https://github-stats-extended.vercel.app/api/top-langs/?username=AOMINHTAM&layout=compact&theme=radical&hide_border=true&title_color=f59e0b&hide=html,css" alt="Top Languages" width="48%" />
</p>

---

<p align="center">
  <i>📍 Ho Chi Minh City, Vietnam • Open to Data Analyst | Data Engineer | Analytics Engineer (Intern &amp; Fresher) Opportunities</i>
</p>
