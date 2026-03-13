# 💼 Global Job Market & Skills Demand Dashboard

> **An end-to-end Power BI analytics project built on 122,000+ real LinkedIn job postings (Dec 2023 – Apr 2024) — revealing in-demand skills, salary benchmarks, hiring trends, and geographic job concentration across the global market.**

[![Power BI](https://img.shields.io/badge/Built%20With-Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com)
[![Dataset](https://img.shields.io/badge/Dataset-LinkedIn%20Job%20Postings-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.kaggle.com/datasets/arshkon/linkedin-job-postings)
[![Kaggle](https://img.shields.io/badge/Source-Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/datasets/arshkon/linkedin-job-postings)
[![License: Apache2.0](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)]()
[![PDF Size](https://img.shields.io/badge/PDF%20Export-Under%2010%20MB-blue?style=for-the-badge)]()

---

## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [Live Dashboard](#-live-dashboard)
- [Key Insights at a Glance](#-key-insights-at-a-glance)
- [Dashboard Pages](#-dashboard-pages)
- [Dataset Structure](#-dataset-structure)
- [Tech Stack](#-tech-stack)
- [Project Architecture](#-project-architecture)
- [Power Query Transformations](#-power-query-transformations)
- [DAX Measures](#-dax-measures)
- [Data Model — Star Schema](#-data-model--star-schema)
- [How to Run This Project](#-how-to-run-this-project)
- [File Size & PDF Export](#-file-size--pdf-export)
- [Project Structure](#-project-structure)
- [Problem Statement](#-problem-statement)
- [Results & Key Findings](#-results--key-findings)
- [Future Scope](#-future-scope)
- [Connect With Me](#-connect-with-me)

---

## 🎯 Project Overview

The **Global Job Market & Skills Demand Dashboard** is a fully interactive Power BI project designed to answer four critical questions that job seekers, recruiters, HR analysts, and workforce planners face every day:

| ❓ Question | 📊 Answered On |
|---|---|
| Which skills are most in demand globally? | Page 2 — Skills Analysis |
| What salaries are companies offering? | Page 3 — Salary Benchmark |
| Where are jobs geographically concentrated? | Page 4 — Geographical Job Map |
| Which industries and roles are hiring most? | Page 1 — Executive Summary |

### Why This Project Matters

> 🌍 The global talent market generated **over 122,000 LinkedIn job postings** between December 2023 and April 2024 alone. Without a consolidated analytical view, job seekers and hiring organizations are forced to make critical decisions based on incomplete, fragmented, or anecdotal information.

This dashboard bridges that gap — turning raw CSV data into a decision-ready intelligence platform in under 10 MB.

---

## 🚀 Live Dashboard

| Resource | Link |
|---|---|
| 🔗 Live Power BI Report | [Click to View Dashboard](https://app.powerbi.com/view?r=YOUR_EMBED_TOKEN) |
| 📄 PDF Export (all 4 pages) | [Download PDF](./exports/LinkedIn_JobMarket_Dashboard.pdf) |
| 📦 Download .pbix File | [LinkedIn_JobMarket_Dashboard.pbix](./LinkedIn_JobMarket_Dashboard.pbix) |
| 📁 Raw Dataset | [Kaggle — LinkedIn Job Postings 2023-24](https://www.kaggle.com/datasets/arshkon/linkedin-job-postings) |

> ⚠️ Replace `YOUR_EMBED_TOKEN` with your actual Power BI publish-to-web token from: **Power BI Service → File → Embed Report → Publish to Web**

---

## 📊 Key Insights at a Glance

| Metric | Value | Insight |
|---|---|---|
| 📋 Total Job Postings | **122,000+** | Covers Dec 2023 – Apr 2024 |
| ⚡ Apply Rate | **72%** | 3 in 4 viewers apply — high competition |
| 🏠 Remote Jobs | **12.13%** | On-site roles dominate the market |
| 🏆 #1 In-Demand Skill | **Information Technology** | 25,000+ skill tags across all postings |
| 💰 Highest-Paying Role | **Intellectual Property** | Avg Max Salary: 572M (package-based) |
| 🗺️ Top Hiring State | **California (CA)** | Leads all US states by posting volume |
| 📈 Peak Hiring Month | **April 2024** | 120K postings — major seasonal surge |
| 🏢 Most Posted Title | **Sales Manager** | 669 postings in dataset period |

---

## 📄 Dashboard Pages

### Page 1 — Executive Job Market Summary

> *The command center. See the entire market at a glance.*

**Visuals included:**
- 🔢 **3 KPI Cards** — Total Job Postings (122K), Apply Rate % (72), Remote Jobs % (12.13)
- 📈 **Line Chart** — Monthly job posting trend (Jan → Dec), revealing the April 2024 spike
- 🗺️ **World Map** — Total job postings by country (filled map with color intensity)
- 📊 **Horizontal Bar Chart** — Top job titles: Sales Manager (669), Customer Service (473), Project Manager (348)
- 📅 **Date Range Slicer** — Filters all visuals simultaneously (Dec 2023 – Apr 2024)

---

### Page 2 — Skills Analysis

> *The star page — only possible with the LinkedIn dataset's job_skills.csv.*

**Visuals included:**
- 📊 **Top 10 Demanded Skills Bar Chart** — Information Technology leads with 25K+ tags
- 🌲 **Treemap** — Skill demand broken down by industry (IT, Sales, Management top 3)
- 🔵 **Scatter Plot** — Apply Rate % vs Skill Demand Count — reveals which skills attract the most applicants
- 🔍 **Industry Search Slicer** — Filter all visuals by any of 148 industries
- 📅 **Date Range Slicer** — Synced across all pages

**Top 5 Skills Found:**

```
1. Information Technology   ████████████████████  25K
2. Sales                    █████████████████     21K
3. Management               ████████████████      20K
4. Manufacturing            ██████████████        18K
5. Health Care Provider     █████████████         17K
```

---

### Page 3 — Salary Benchmark

> *Know your worth. Compare salaries across roles, seniority, and geography.*

**Visuals included:**
- 📊 **Top 15 Avg Max Salary Bar Chart** — by job title
- 📊 **Clustered Bar Chart** — Average min & max salary by experience level (Executive → Internship)
- 📊 **Top 10 Countries/States Bar Chart** — Avg max salary by geography (Illinois Metro leads)
- 🔍 **Job Name Search Slicer** — Filter all salary visuals by specific role
- 📋 **Reference Table** — country, industry, title cross-reference lookup

> ⚠️ Note: ~70% of LinkedIn postings do not include salary data. All salary visuals are filtered to non-blank rows only.

---

### Page 4 — Geographical Job Map

> *Where in the world is the work?*

**Visuals included:**
- 🌍 **Filled Map (Country Level)** — Global job concentration heatmap
- 🔵 **Bubble Map (City Level)** — Job density by city (bigger bubble = more jobs)
- 📊 **Horizontal Bar Chart** — Top 7 US states: CA, TX, NY, FL, NC, IL, PA
- 🔍 **Job Name Slicer** — Filter maps by specific job title
- ✅ **Experience Level Slicer** — Associate, Director, Entry, Executive, Internship, Mid-Senior
- 📅 **Date Range Slicer** — Synced from Page 1

---

## 📦 Dataset Structure

**Source:** [kaggle.com/datasets/arshkon/linkedin-job-postings](https://www.kaggle.com/datasets/arshkon/linkedin-job-postings)

| File | Records | Role in Dashboard |
|---|---|---|
| `postings.csv` ⭐ | 122,000+ | **Main Fact Table** — job titles, salaries, dates, views, applies |
| `companies.csv` ⭐ | ~25,000 | Company profiles, industry, employee count |
| `job_skills.csv` ⭐ | ~400,000 | Maps every skill to every job posting |
| `skills.csv` | ~2,800 | Skill lookup (PY = Python, SQL = SQL) |
| `industries.csv` | ~148 | Industry name lookup table |
| `job_industries.csv` | ~120,000 | Maps each job to its industry |
| `benefits.csv` | ~60,000 | Benefits offered per posting (Medical, Dental, 401K) |

### Key Columns Used

```
postings.csv
├── job_id              → Primary key for all joins
├── title               → Job title (Sales Manager, Data Analyst...)
├── company_id          → Foreign key → companies.csv
├── location            → "City, State, Country" (split in Power Query)
├── min_salary          → Normalized to Yearly_Salary
├── max_salary          → Normalized to Yearly_Salary
├── pay_period          → HOURLY / MONTHLY / YEARLY
├── formatted_work_type → Full-time / Part-time / Contract
├── remote_allowed      → 0 or 1 (binary flag)
├── experience_level    → EN / MI / SE / EX (renamed in Power Query)
├── views               → Page view count per posting
├── applies             → Application count per posting
└── original_listed_time→ Unix ms timestamp (converted to Date)
```

---

## 🛠️ Tech Stack

| Tool | Version | Purpose |
|---|---|---|
| **Microsoft Power BI Desktop** | Latest (Free) | Dashboard development & visualization |
| **Power Query Editor** | Built-in | ETL — data cleaning & transformation |
| **DAX (Data Analysis Expressions)** | Built-in | Calculated measures & KPIs |
| **Power BI Model View** | Built-in | Star Schema relationship building |
| **Bing Maps / TomTom** | External tiles | Geographic map visual rendering |
| **Power BI Service** | Free tier | Publishing & PDF export |
| **Microsoft Excel / CSV** | — | Raw dataset format (7 CSV files) |

---

## 🏗️ Project Architecture

```
Raw CSVs (Kaggle)
       │
       ▼
┌─────────────────────────┐
│   Power Query Editor     │   ← ETL Layer
│   - Remove columns       │
│   - Convert timestamp    │
│   - Normalize salary     │
│   - Split location       │
│   - Rename codes         │
│   - Fix data types       │
└─────────────────────────┘
       │
       ▼
┌─────────────────────────┐
│   Star Schema Model      │   ← Data Model Layer
│   postings (FACT)        │
│   ├── companies          │
│   ├── job_skills         │
│   ├── skills             │
│   ├── job_industries     │
│   ├── industries         │
│   └── benefits           │
└─────────────────────────┘
       │
       ▼
┌─────────────────────────┐
│   DAX Measures           │   ← Analytics Layer
│   - Total Job Postings   │
│   - Apply Rate %         │
│   - Remote Jobs %        │
│   - Avg Max Salary       │
│   - Skill Demand Count   │
└─────────────────────────┘
       │
       ▼
┌─────────────────────────┐
│   4 Dashboard Pages      │   ← Presentation Layer
│   P1: Executive Summary  │
│   P2: Skills Analysis    │
│   P3: Salary Benchmark   │
│   P4: Geographical Map   │
└─────────────────────────┘
       │
       ▼
  PDF Export (< 10 MB) + Power BI Service (Public URL)
```

---

## 🔧 Power Query Transformations

All transformations were applied in **Power Query Editor** (Home → Transform Data):

### 1. Remove Unused Columns
```
Removed: description, application_url, posting_domain, listed_time
Reason: Reduce file size and improve dashboard performance
```

### 2. Convert Unix Timestamp → Date
```m
// Add Column → Custom Column → Name: PostedDate
#datetime(1970,1,1,0,0,0) + #duration(0,0,0,[original_listed_time]/1000)
// Then: Change Type → Date
```

### 3. Extract Date Parts
```m
PostYear     = Date.Year([PostedDate])
PostMonth    = Date.ToText([PostedDate], "MMMM")
PostMonthNum = Date.Month([PostedDate])
```

### 4. Rename Experience Level Codes
```
EN  →  Entry Level
MI  →  Mid Level
SE  →  Senior Level
EX  →  Executive Level
```

### 5. Normalize All Salaries to Annual USD
```m
Yearly_Salary =
    if [pay_period] = "HOURLY"   then [max_salary] * 40 * 52
    else if [pay_period] = "MONTHLY" then [max_salary] * 12
    else if [pay_period] = "YEARLY"  then [max_salary]
    else null
```

### 6. Split Location Column
```
"New York, NY, US"  →  JobCity="New York" | JobState="NY" | JobCountry="US"
Transform → Split Column → By Delimiter → Comma → At Each Occurrence
Then: Trim all 3 columns
```

### 7. Add Remote Work Label
```m
RemoteLabel =
    if [remote_allowed] = 1 then "Remote Allowed"
    else "On-Site Only"
```

### 8. Fix Data Types
```
job_id, company_id          → Whole Number
max_salary, min_salary      → Decimal Number
views, applies              → Whole Number
PostedDate                  → Date
PostYear, PostMonthNum      → Whole Number
```

---

## 📐 DAX Measures

All measures stored in a dedicated `_Measures` table (Home → Enter Data → name: _Measures).

### Job Count Measures
```dax
Total Job Postings = COUNTROWS(postings)

Total Companies Hiring = DISTINCTCOUNT(postings[company_id])

Total Unique Skills = DISTINCTCOUNT(job_skills[skill_abr])

Avg Views per Posting = AVERAGE(postings[views])

Avg Applies per Posting = AVERAGE(postings[applies])

Apply Rate % =
    DIVIDE([Avg Applies per Posting], [Avg Views per Posting], 0) * 100
```

### Remote Work Measures
```dax
Remote Jobs Count =
    CALCULATE(COUNTROWS(postings), postings[remote_allowed] = 1)

Remote Jobs % =
    DIVIDE([Remote Jobs Count], [Total Job Postings], 0) * 100
```

### Salary Measures
```dax
Avg Max Salary =
    CALCULATE(
        AVERAGE(postings[Yearly_Salary]),
        NOT(ISBLANK(postings[Yearly_Salary]))
    )

Median Salary =
    CALCULATE(
        MEDIAN(postings[Yearly_Salary]),
        NOT(ISBLANK(postings[Yearly_Salary]))
    )

Jobs With Salary Count =
    CALCULATE(COUNTROWS(postings), NOT(ISBLANK(postings[Yearly_Salary])))
```

### Skills Measure
```dax
// Used as value axis in all skills bar charts and treemaps
Skill Demand Count = COUNTROWS(job_skills)
```

---

## 🗂️ Data Model — Star Schema

```
                    ┌──────────────┐
                    │ companies    │
                    │ (company_id) │
                    └──────┬───────┘
                           │ Many:1
          ┌────────────────┼────────────────────┐
          │                │                    │
┌─────────┴──────┐  ┌──────┴────────┐  ┌───────┴──────┐
│  job_skills    │  │  postings     │  │  benefits    │
│  (job_id)      │  │  ★ FACT TABLE │  │  (job_id)    │
│  (skill_abr)   │  │  (job_id) PK  │  └──────────────┘
└─────────┬──────┘  │  (company_id) │
          │         │  (PostedDate) │
       Many:1       └──────┬────────┘
          │                │
    ┌─────┴───┐      ┌─────┴─────────┐
    │ skills  │      │job_industries │
    │(skill_  │      │  (job_id)     │
    │  abr)   │      │(industry_id)  │
    └─────────┘      └──────┬────────┘
                            │ Many:1
                     ┌──────┴───────┐
                     │  industries  │
                     │(industry_id) │
                     └─────────────┘
```

**Relationship Summary:**

| From | To | Key | Type |
|---|---|---|---|
| postings | job_skills | job_id | 1:Many |
| postings | job_industries | job_id | 1:Many |
| postings | benefits | job_id | 1:Many |
| postings | companies | company_id | Many:1 |
| job_skills | skills | skill_abr | Many:1 |
| job_industries | industries | industry_id | Many:1 |

---

## ▶️ How to Run This Project

### Prerequisites
- Windows 10/11 (64-bit)
- Power BI Desktop — [Download Free](https://powerbi.microsoft.com/desktop)
- Free Kaggle account — [Sign Up](https://www.kaggle.com)
- Minimum 8 GB RAM (recommended for 400K+ row job_skills.csv)

### Step-by-Step Setup

**Step 1 — Download the Dataset**
```
1. Go to: kaggle.com/datasets/arshkon/linkedin-job-postings
2. Click the Download button
3. Extract the ZIP to: C:\PowerBI\LinkedIn_Dataset\
   You should have 7 CSV files inside.
```

**Step 2 — Open the .pbix File**
```
Option A (Recommended):
  Download LinkedIn_JobMarket_Dashboard.pbix from this repo
  Double-click to open in Power BI Desktop

Option B (Build from scratch):
  Follow the Power Query and DAX sections above
  Load all 7 CSVs via: Home → Get Data → Text/CSV
```

**Step 3 — Refresh Data**
```
Home → Refresh
Power BI will reload all 7 tables from your local CSV files
(Update the file path in Power Query if needed)
```

**Step 4 — Enable Map Visuals**
```
File → Options and Settings → Options
→ Security → tick "Use Map and Filled Map visuals" → OK
(Required for the Geographical Map page)
```

**Step 5 — Explore the Dashboard**
```
Use the Page Navigator buttons at the bottom to switch pages
Use the Date Range slicer to filter all pages simultaneously
Use the Experience Level slicer on Page 4 to filter the map
Use the Job Name search slicer to explore specific roles
```

---

## 📁 Project Structure

```
LinkedIn-JobMarket-PowerBI-Dashboard/
│
├── 📊 LinkedIn_JobMarket_Dashboard.pbix    ← Main Power BI project file
│
├── 📄 exports/
│   └── LinkedIn_JobMarket_Dashboard.pdf   ← 4-page PDF export (< 10 MB)
│
├── 📦 data/
│   ├── postings.csv                       ← Main fact table (122K+ rows)
│   ├── companies.csv                      ← Company dimension
│   ├── job_skills.csv                     ← Skills fact (~400K rows)
│   ├── skills.csv                         ← Skills lookup
│   ├── industries.csv                     ← Industry lookup
│   ├── job_industries.csv                 ← Job-industry bridge
│   └── benefits.csv                       ← Benefits dimension
│
├── 📸 screenshots/
│   ├── page1_executive_summary.png
│   ├── page2_skills_analysis.png
│   ├── page3_salary_benchmark.png
│   └── page4_geographical_map.png
│
└── 📖 README.md                            ← This file
```

---

## ❓ Problem Statement

In the modern digital recruitment landscape, both job seekers and organizations lack a centralized, interactive view of:
- Which skills are truly valued across industries
- What salaries are realistically being offered by role, level, and location
- Where in the world hiring activity is most concentrated
- How hiring trends have shifted over recent months

**This dashboard solves all four problems in a single, filterable interface** — turning 122,000+ raw job records into clear, actionable market intelligence accessible to any user without requiring technical expertise.

---

## 📈 Results & Key Findings

### Skills Market
- **Information Technology** is the #1 demanded skill with **25,000+ tags** — appearing in ~20% of all job postings
- The top 5 skills (IT, Sales, Management, Manufacturing, Healthcare) account for over **50% of all skill demand**
- Engineering and Finance skills command **significantly higher salaries** despite lower posting volumes

### Salary Intelligence
- Executive-level roles earn **3-5× more** than Entry-level roles in the same industry
- **Illinois Metropolitan** area leads all US regions in average max salary
- **California** leads all states by both job volume AND salary level

### Geographic Insights
- **North America dominates** — US accounts for the vast majority of postings
- **Top 3 US states**: California (CA) → Texas (TX) → New York (NY)
- Global reach: postings visible across Europe, Asia-Pacific, and Australia

### Market Conditions
- An **Apply Rate of 72%** signals intense competition — job seekers must differentiate aggressively
- Only **12.13% of roles offer remote work** — confirming on-site employment still dominates post-pandemic
- **April 2024 showed a 120K posting spike** — the single largest monthly volume in the dataset

---

## 🔮 Future Scope

- [ ] **Real-Time Data Feed** — Connect to LinkedIn Jobs API for daily auto-refresh via Power BI Service Scheduled Refresh
- [ ] **ML Salary Predictor** — Integrate Python visual with XGBoost model to predict salary from title + skills + location inputs
- [ ] **Skills Gap Analyzer** — Input your current skills → dashboard highlights the gap vs top demanded skills in your target industry
- [ ] **Benefits Analysis Page** — Use `benefits.csv` to show which industries offer the best Medical/Dental/401K packages
- [ ] **Global Expansion** — Add data from Indeed, Naukri, and government labor APIs (BLS, Eurostat) for genuine worldwide coverage
- [ ] **Mobile Layout** — Publish mobile-optimized view via Power BI Service for smartphone access
- [ ] **Q&A AI Page** — Add Power BI Q&A visual for natural language queries ("top skills in finance with salary above 100K")

---

## 🤝 Connect With Me

If you found this project useful, interesting, or inspiring — let's connect!

| Platform | Link |
|---|---|
| 💼 LinkedIn | [Ashish Raj](https://www.linkedin.com/in/ashish-raj-ashishraj/) |
| 🐙 GitHub | [Ashish Raj](https://github.com/ashishraj-hub)  |
| 📧 Email | ashishrajara16@gmail.com |


### ⭐ Support This Project

If this README or project helped you:
- **Star** ⭐ this repository
- **Fork** 🍴 it and build your own version
- **Share** it with someone who is learning Power BI

---

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

The dataset is sourced from Kaggle under its respective terms of use:
[kaggle.com/datasets/arshkon/linkedin-job-postings](https://www.kaggle.com/datasets/arshkon/linkedin-job-postings)

---

<div align="center">

**Built with 💙 using Microsoft Power BI and LinkedIn Job Postings Data**

*Last updated: 2024 | Dataset period: December 2023 – April 2024*

</div>
