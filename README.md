# LexEuropa: Client Risk, Profitability & Legal Operations Dashboard

> A 3-page Power BI dashboard suite that tracks firm-wide profitability, client risk exposure, and lawyer/operational performance across offices, practice areas, and case types for a pan-European law firm.

<img width="5594" height="3956" alt="Group 1" src="https://github.com/user-attachments/assets/3d2733f9-5e19-47de-98d8-eaf09659e971" />

---

## 📋 Table of Contents

- [Overview](#overview)
- [Dashboard Pages](#dashboard-pages)
  - [LexEuropa Overview](#1-lexeuropa-overview)
  - [Operations & Lawyer Performance](#2-operations--lawyer-performance)
  - [Client, Risk & Profitability Analysis](#3-client-risk--profitability-analysis)
- [Key Metrics & KPIs](#key-metrics--kpis)
- [Relationship Model](#relationship-model)
- [Dataset Schema](#dataset-schema)
- [File Structure](#file-structure)
- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [Usage & Filters](#usage--filters)
- [Insights Summary](#insights-summary)

---

## Overview

The **LexEuropa Dashboard** is a Power BI report built to give firm leadership, practice group heads, and operations managers a single view into how the firm is performing financially and operationally. It brings together case-level financials, client risk scoring, satisfaction data, and lawyer workload metrics so decision-makers can spot which clients and case types drive profit, where risk and collections exposure is concentrated, and which lawyers and offices are carrying the firm's workload all from a single dashboard.

### 🎯 Business Objectives

- Track total revenue, profit, and outstanding balance trends across years and offices
- Quantify client-level risk exposure and flag high-risk, high-value accounts
- Evaluate profitability by case type, industry, and practice area to identify the firm's most valuable work
- Benchmark lawyer utilization, workload, and billable performance to surface over- and under-utilized talent
- Monitor case outcomes (won, lost, settled, withdrawn, ongoing) against satisfaction and risk to assess portfolio health
- Identify where case complexity is eroding profit margins, and where outstanding balances are creating collections risk

---

## Dashboard Pages

### 1. LexEuropa Overview

> *High-level view of firm performance, profitability, and case portfolio.*

<img width="7646" height="4404" alt="LexEuropa Overview" src="https://github.com/user-attachments/assets/d11619ea-80e3-449f-8ca8-378377133093" />

#### KPI Cards

| KPI | Value | Detail |
|-----|-------|--------|
| **Total Revenue** | €2.80bn | vs Previous Year ▲62.1% (€1.73B) \| vs Previous Quarter ▲12.0% (€2.50B) |
| **Total Profit** | €1.59bn | Overall Profit Margin 56.81% \| vs Previous Year ▲62.3% (€981.38M) |
| **Active Cases** | 8K | Cases per Lawyer 75 \| Average Days Open 258 days |
| **Average Satisfaction Score** | 6.64 | Satisfied Cases % 3,806 (25.4%) \| Win/Loss Ratio 1.89 |
| **Outstanding Balance** | €773.38M | Outstanding Balance % of Revenue 27.59% \| Clients with Outstanding Balance 800 |

#### Visuals

**Revenue, Profit & Outstanding Balance Trend : Column Chart** *(Drill down to Year → All Data)*
- Revenue has held broadly steady across 2024–2026, ranging from €1.07bn to €1.11bn per year, with 2025 posting the strongest year at €1.11bn
- Profit tracks closely alongside revenue each year, consistently landing at roughly 55–57% of the revenue figure
- Outstanding balance dropped sharply from €352.33M (2024) to €106.55M in the mid-2025 period, before climbing back to €445.95M by 2026 a pattern worth investigating for collections timing

**Cases by Outcome : Donut Chart**
- Settled cases lead the portfolio at 4.3K (28.72%), narrowly ahead of Won cases at 4.0K (26.83%)
- Ongoing cases account for 3.6K (23.81%) of the total portfolio, still active and unresolved
- Lost (2.1K, 14.17%) and Withdrawn (971, 6.47%) cases together make up roughly one-fifth of resolved outcomes

**Revenue & Case Performance by Office : Bar Chart**
- Frankfurt leads all offices at €365.64M, narrowly ahead of London at €358.64M
- Paris (€292.03M) and Amsterdam (€211.69M) form a clear middle tier
- Brussels trails the group at €210.81M, the lowest-revenue office in the network

**Outstanding Balance vs Client Satisfaction by Risk Category : Scatter Chart**
- x-axis: Outstanding Balance; y-axis: Average Satisfaction Score
- Critical-risk cases carry by far the largest outstanding balance (~€600M) while maintaining a respectable satisfaction score (~6.7), suggesting high-risk clients aren't necessarily dissatisfied clients
- Low-risk cases sit near €0 outstanding balance but post the lowest satisfaction score (~6.5) of any risk tier
- High-risk cases show the highest satisfaction score (~6.7) among all categories, despite carrying meaningful outstanding balance (~€200M)

**Cases by Priority and Complexity : Bar Chart**
- Low-priority cases dominate case volume across nearly every complexity tier, particularly at Low and Medium complexity
- Critical and Urgent priority cases are comparatively rare across all complexity levels, suggesting the firm's caseload is weighted toward routine rather than emergency matters
- Medium complexity shows the most even spread of cases across all four priority tiers

---

### 2. Operations & Lawyer Performance

> *Analyzes legal operations, workload, and resource utilization.*

<img width="7646" height="4404" alt="Operations   Lawyer Performance" src="https://github.com/user-attachments/assets/9862e803-f26e-41a5-a194-424732cecf92" />

#### KPI Cards

| KPI | Value | Detail |
|-----|-------|--------|
| **Total Billable Hours** | 2.10M | Average Billable Hours per Lawyer 10.50K \| Revenue per Billable Hour €1.34K |
| **Average Lawyer Utilization** | 20.50 | Lawyers Above 80% Utilization 155 \| Underutilized Lawyers 200 |
| **Active Cases** | 8K | Average Days Open 258 days \| Cases per Lawyer 75 |
| **Average Workload Index** | 1.43 | Avg Billable Hours per Case 140 hours \| High Workload Cases 413 |
| **Total Documents Produced** | 120K | Total Court Appearances 12K \| Total Meetings 80K |

#### Visuals

**Lawyer Performance Summary : Table**
- Javier Smit generates the highest profit at €41.04M on 56 total cases, with a Win/Loss Ratio of 1.25
- Javier Martinez posts the highest Win/Loss Ratio in the top 9 at 5.67, despite handling fewer cases (46) and generating less total profit (€35.09M)
- Sebastian Rodriguez and Henrik Walsh carry the heaviest caseloads (87 and 91 cases respectively) but rank lowest on Utilization Score among the group, hinting at a possible volume-versus-efficiency tradeoff

**Case Distribution by Type : Donut Chart**
- Contract Dispute is by far the most common case type at 2.4K cases (38.42% of volume)
- Compliance Review (974, 15.70%) and Corporate Restructuring (1.0K, 16.30%) form a clear second tier
- Acquisition Due Diligence and Trade Dispute round out the distribution at the lower end of case volume

**Billable by Practice Area : Bar Chart**
- Litigation leads all practice areas at 301.98K billable hours
- Corporate Law (282.43K) and Regulatory Compliance (266.27K) follow closely behind
- Mergers & Acquisitions (264.91K) and Commercial Law (215.72K) round out the top five, with a relatively tight spread across the leading practice areas

**Billable Hours vs Revenue by Practice Area : Scatter Chart**
- x-axis: Total Billable Hours; y-axis: Total Revenue
- The relationship is broadly positive: practice areas with more billable hours (250K–300K) tend to cluster at higher revenue (€350M–€400M+)
- One practice area near 300K billable hours reports a comparatively lower revenue return (~€250M), breaking the otherwise consistent trend and warranting a closer look at realization rates
- Lower-hour practice areas (~100K–150K) consistently land at the bottom of the revenue range, as expected

**Cases by Department (Drill down to Seniority) : Bar Chart**
- Tax Law handles the highest case volume at 2.1K cases
- Corporate Law and Litigation are tied for second at 2.0K cases each
- Intellectual Property (1.8K) and Employment Law (1.8K) round out the top five departments by case volume

---

### 3. Client, Risk & Profitability Analysis

> *Identifies profitability drivers, client value, and business risks.*

<img width="7646" height="4404" alt="Client, Risk   Profitability Analysis" src="https://github.com/user-attachments/assets/3f56f072-96b2-452e-b71c-f8502e8c12f7" />

#### KPI Cards

| KPI | Value | Detail |
|-----|-------|--------|
| **Total Profit** | €1.59bn | Overall Profit Margin 56.81% \| vs Previous Year ▲62.3% (€981.38M) |
| **Average Satisfaction Score** | 6.64 | Satisfied Cases % 3,806 (25.4%) \| Win/Loss Ratio 1.89 |
| **Outstanding Balance** | €773.38M | Outstanding Balance % of Revenue 27.59% \| Clients with Outstanding Balance 800 |
| **High Risk Cases** | €2.11K | Average Risk Score 41.76 \| Critical Risk Cases 561 |
| **Strategic Client Revenue** | €560.29M | Strategic Clients 132 \| Revenue per Strategic Client €4.24M |

#### Visuals

**Client Risk & Profitability Summary : Table**
- Meridian Crestline SA posts the highest profit margin among top clients at 66.94%, on an Employment Tribunal case open for 238 days
- Summit Vertex Capital carries the highest risk score in the top 10 at 100.00, tied to a Corporate Restructuring matter, yet still returns a strong 66.88% margin
- Baltic Meridian AG shows the lowest satisfaction score among top-margin clients at 2.80, despite a healthy 66.80% profit margin a disconnect between profitability and client experience worth flagging

**Profit Distribution by Case Type : Donut Chart** *(Drill down)*
- Property Transaction leads case-type profitability at 58.38% margin, representing 20.27% of the distribution shown
- Merger Advisory (57.58%) and Custody Dispute (57.55%) form a tight middle cluster
- Tax Investigation posts the lowest margin among the case types shown at 57.13%, though the spread across all types is relatively narrow (roughly one percentage point)

**Profit by Industry (Drill down to Client Region) : Bar Chart**
- Media & Entertainment is the most profitable industry at €123.89M
- Food & Beverage (€122.18M) trails closely behind, within €1.71M of the leader
- Retail (€117.00M), Financial Services (€113.79M), and Manufacturing (€110.00M) round out a tightly clustered top five

**Case Complexity vs Profit Margin by Practice Area : Scatter Chart**
- x-axis: Average Case Complexity Score; y-axis: Overall Profit Margin
- Profit margin generally rises with complexity up to a point (~1.90–1.94 complexity, ~0.57 margin), before tapering off at the highest complexity scores
- The lowest-complexity practice area (~1.87) also posts the lowest profit margin in the group, suggesting simpler matters may be under-priced relative to effort
- The relationship is not strictly linear margins plateau rather than continuing to climb as complexity increases further, indicating diminishing returns on complexity beyond a certain threshold

**Average Risk Score by Case Type : Bar Chart**
- Planning Dispute carries the highest average risk score at 45.34
- Divorce & Asset Division (44.33) and IP Infringement (43.27) follow closely behind
- AML Review (43.22) and Merger Advisory (42.78) round out the top five highest-risk case types, with a relatively tight 2.6-point spread across the group

---

## Key Metrics & KPIs

| KPI | Definition |
|-----|-----------|
| **Total Revenue** | Sum of all billed revenue across active and closed cases in the selected period |
| **Total Profit** | Total Revenue minus total case-related costs |
| **Overall Profit Margin** | Total Profit as a percentage of Total Revenue |
| **Active Cases** | Count of cases currently open or in progress |
| **Average Satisfaction Score** | Mean client satisfaction rating across all rated cases |
| **Win/Loss Ratio** | Ratio of cases won to cases lost |
| **Outstanding Balance** | Total unpaid client balance still owed to the firm |
| **Outstanding Balance % of Revenue** | Outstanding Balance expressed as a percentage of Total Revenue |
| **High Risk Cases** | Count of cases flagged with an elevated or critical risk score |
| **Average Risk Score** | Mean composite risk rating assigned to a case, client, or case type |
| **Strategic Client Revenue** | Total revenue generated by clients designated as strategic accounts |
| **Total Billable Hours** | Sum of all hours billed by lawyers across all cases |
| **Average Lawyer Utilization** | Mean percentage of available lawyer capacity billed to client work |
| **Average Workload Index** | Composite score measuring case load intensity relative to lawyer capacity |
| **Revenue per Billable Hour** | Total Revenue divided by Total Billable Hours |
| **Average Case Complexity Score** | Mean complexity rating assigned to a case, used to assess effort and pricing alignment |
| **Days Open** | Number of days a case has remained active, from opening to current date or closure |

---

## Relationship Model

| From (FK) | To (PK) | Join Column |
|-----------|---------|-------------|
| Fact_Cases.Case ID | Dim_Case.Case ID | Case ID |
| Fact_Cases.Client ID | Dim_Client.Client ID | Client ID |
| Fact_Cases.Lawyer ID | Dim_Lawyer.Lawyer ID | Lawyer ID |
| Fact_Cases.Office City | Dim_Office.Office City | Office City |
| Fact_Cases.Open Date | Dim_Date.Date | Date |
| Fact_Cases.Close Date | Dim_Date.Date | Date *(inactive relationship)* |

---

## Dataset Schema

**Fact_Cases**

| Column | Type | Description |
|--------|------|--------------|
| `Case ID` | String (FK) | Unique case identifier; references Dim_Case |
| `Client ID` | String (FK) | References Dim_Client |
| `Lawyer ID` | String (FK) | References Dim_Lawyer |
| `Office City` | String (FK) | References Dim_Office |
| `Open Date` | Date | Case opening date, used for time-intelligence calculations |
| `Close Date` | Date | Case closing date (inactive relationship to Dim_Date) |
| `Days Open` | Integer | Number of days the case has been active |
| `Billable Hours` | Decimal | Total billable hours logged against the case |
| `Non-Billable Hours` | Decimal | Total non-billable hours logged against the case |
| `Court Appearances` | Integer | Number of court appearances associated with the case |
| `Meetings` | Integer | Number of meetings associated with the case |
| `Documents Produced` | Integer | Number of documents produced for the case |
| `Revenue (EUR)` | Decimal | Total billed revenue for the case |
| `Internal Costs (EUR)` | Decimal | Total internal cost incurred delivering the case |
| `Profit (EUR)` | Decimal *(Calculated)* | Revenue minus Internal Costs |
| `Profit Margin %` | Decimal *(Calculated)* | Profit as a percentage of Revenue |
| `Invoice Amount (EUR)` | Decimal | Total amount invoiced to the client |
| `Outstanding Balance (EUR)` | Decimal | Unpaid balance remaining on the case |
| `Client Satisfaction Score` | Decimal | Client satisfaction rating for the case |
| `Risk Score` | Decimal | Composite risk rating for the case |
| `Lawyer Utilization %` | Decimal | Lawyer utilization rate associated with the case |
| `Workload Index` | Decimal | Composite workload intensity score |

**Dim_Case**

| Column | Type | Description |
|--------|------|--------------|
| `Case ID` | String (PK) | Unique case identifier |
| `Case Name` | String | Descriptive case name |
| `Case Status` | String | Current status of the case (e.g., Pending Closure) |
| `Case Outcome` | String | Final or current outcome (Won, Lost, Settled, Withdrawn, Ongoing) |
| `Case Complexity` | String | Complexity tier (e.g., Low, Medium, High, Critical) |
| `Case Type` | String | Type of case (e.g., Compliance Review, Contract Dispute) |
| `Practice Area` | String | Practice area associated with the case |
| `Priority` | String | Priority tier (Low, Medium, High, Urgent, Critical) |

**Dim_Lawyer**

| Column | Type | Description |
|--------|------|--------------|
| `Lawyer ID` | String (PK) | Unique lawyer identifier |
| `Lawyer Name` | String | Lawyer's full name |
| `Gender` | String | Lawyer's gender |
| `Age Group` | String | Age bracket of the lawyer |
| `Years Experience` | Integer | Years of professional experience |
| `Seniority` | String | Seniority level (e.g., Senior Associate) |
| `Department` | String | Department the lawyer belongs to |
| `Employment Status` | String | Employment type (e.g., Full-Time) |

**Dim_Client**

| Column | Type | Description |
|--------|------|--------------|
| `Client ID` | String (PK) | Unique client identifier |
| `Client Name` | String | Client's full name |
| `Industry` | String | Client's industry sector |
| `Company Size` | String | Client company size tier (e.g., Enterprise) |
| `Client Country` | String | Client's country |
| `Client Region` | String | Client's geographic region |
| `Strategic Client Flag` | Boolean | Flag indicating whether the client is a designated strategic account |
| `Client Since Year` | Integer | Year the client relationship began |

**Dim_Office**

| Column | Type | Description |
|--------|------|--------------|
| `Office City` | String (PK) | City where the office is located |
| `Country` | String | Country where the office is located |
| `Region` | String | Geographic region of the office |
| `Latitude` | Decimal | Office latitude coordinate |
| `Longitude` | Decimal | Office longitude coordinate |
| `Headquarters Flag` | Boolean | Flag indicating whether the office is the firm's headquarters |

---

## File Structure

```
lexeuropa-dashboard/
│
├── 📊 LexEuropa_Client_Risk_Profitability_Dashboard.pbix   # Main Power BI file
│
├── 📁 screenshots/
│   ├── LexEuropa_Overview.png
│   ├── Operations_and_Lawyer_Performance.png
│   └── Client_Risk_and_Profitability_Analysis.png
│
├── 📂 data/
│   └── LexEuropa_Case_Dataset.xlsx                          # Source data file
│
└── 📄 README.md                                             # This file
```

---

## Getting Started

### Prerequisites

| Tool | Version | Purpose |
|------|---------|---------|
| [Power BI Desktop](https://powerbi.microsoft.com/desktop/) | Latest | Open & edit `.pbix` |
| Microsoft Excel | 2016+ | View/edit source dataset (if applicable) |

### Installation & Setup

1. **Clone or download the repository**
   ```bash
   git clone https://github.com/M1deTheAnalyst/LexEuropa-Client-Risk-Profitability-Legal-Operations-Dashboard.git
   ```

2. **Open the dashboard**
   - Launch **Power BI Desktop**
   - Go to `File → Open` and select `LexEuropa_Client_Risk_Profitability_Dashboard.pbix`

3. **Verify data source connection**
   - Navigate to `Home → Transform Data → Data Source Settings`
   - Update the path to your local source dataset if prompted
   - Click `Refresh` to load the latest data

4. **Refresh data**
   ```
   Home → Refresh
   ```

---

## Usage & Filters

The dashboard includes a slicer pane on all pages, accessed via the **Filter icon** in the top-right corner, supporting the following filters:

- **Year / Quarter / Month** : Filter to a specific time range
- **Office / Region** : Focus on a specific office or client geography
- **Practice Area / Case Type** : Isolate performance by legal specialty
- **Risk Category** : Filter by Low, Medium, High, or Critical risk tier

### Navigation

Use the **left-hand page navigator** to switch between:
- `LexEuropa Overview` : top-line revenue, profit, case outcomes, and office performance
- `Operations & Lawyer Performance` : billable hours, lawyer utilization, workload, and practice area analysis
- `Client, Risk & Profitability Analysis` : client-level profitability, risk exposure, and industry performance

Use the **RESET button** (top-right of each page) to clear all active slicer selections at once.
Use the **Filter icon** (top-right of each page) to open or collapse the slicer pane.

### Drill-Down Interactions

Several visuals support drill-down for deeper analysis:

| Visual | Primary Level | Drill-Down Level |
|--------|---------------|-------------------|
| Revenue, Profit & Outstanding Balance Trend | Year | All Data |
| Profit by Industry | Industry | Client Region |
| Cases by Department | Department | Seniority |
| Profit Distribution by Case Type | Case Type | Sub-category |

---

## Insights Summary

1. **Profitability is strong and improving, but collections risk is trending back up** : Overall profit margin sits at 56.81%, up 62.3% year-over-year, yet outstanding balance climbed from a 2025 low of €106.55M back to €445.95M by 2026 nearly matching total profit for that period. This swing suggests the firm should monitor whether growth is being converted to cash as efficiently as it's being converted to booked revenue.

2. **High-risk clients aren't dissatisfied clients the opposite may be true** : Critical-risk cases carry the largest outstanding balance (~€600M) yet post a solid 6.7 satisfaction score, while Low-risk cases show the lowest satisfaction (~6.5) despite minimal outstanding balance. This counterintuitive pattern suggests risk scoring and client experience are being driven by different underlying factors and shouldn't be conflated.

3. **Frankfurt and London lead the network, but Brussels lags meaningfully** : Frankfurt (€365.64M) and London (€358.64M) generate comparable revenue at the top of the office ranking, while Brussels trails at €210.81M roughly 42% below the leader. This gap warrants a closer look at whether it reflects market size, staffing, or case mix differences.

4. **Case volume and lawyer efficiency don't move together** : Sebastian Rodriguez and Henrik Walsh carry the two heaviest caseloads (87 and 91 cases) among top-performing lawyers, yet both post the lowest Utilization Scores in that group. This suggests high case counts alone are a poor proxy for productive capacity and should be paired with utilization data when evaluating lawyer performance.

5. **Profit margin plateaus rather than scaling with complexity** : Margin rises with case complexity up to roughly 1.90–1.94 on the complexity scale, then flattens rather than continuing to climb. The lowest-complexity practice area also shows the lowest margin, hinting that simpler matters may be underpriced relative to the effort involved while the highest-complexity work isn't necessarily where the greatest margin upside lies.

6. **Contract Dispute dominates case volume but sits outside the top profitability tier** : Contract Dispute accounts for 38.42% of all cases by volume, yet the highest-margin case types shown are Property Transaction (58.38%), Merger Advisory (57.58%), and Custody Dispute (57.55%). This points to a potential opportunity to grow the firm's highest-margin practice areas rather than relying on its highest-volume one.

7. **Strategic clients represent an outsized share of firm value** : 132 strategic clients generate €560.29M in revenue averaging €4.24M per client, well above what the broader client base is likely to produce individually. Protecting and expanding this cohort should be a clear retention priority.

8. **Litigation leads billable hours but the hours-to-revenue relationship isn't perfectly linear** : Litigation posts the highest billable hours (301.98K), and billable hours broadly track with revenue across practice areas. However, one practice area near 300K hours reports a noticeably lower revenue return than peers at similar hour totals a signal worth investigating for realization rate or write-off issues.

9. **Africa-style infrastructure gaps have a legal-ops parallel: risk and satisfaction don't always move together by geography or case type** : Planning Dispute carries the highest average risk score (45.34) among case types, while risk scores across the top five case types cluster within a tight 2.6-point band suggesting risk is broadly, rather than narrowly, concentrated across the portfolio rather than driven by one outlier case type.

10. **Lawyer utilization has meaningful headroom** : Average lawyer utilization sits at just 20.50, with 200 lawyers classified as underutilized against 155 above 80% utilization. Given cases per lawyer already average 75, this points less to a capacity shortage and more to uneven workload distribution across the firm's lawyer base.

---

## Author

**M1deTheAnalyst**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/m1detheanalyst)
[![GitHub](https://img.shields.io/badge/GitHub-Profile-181717?style=for-the-badge&logo=github)](https://github.com/M1deTheAnalyst)
[![X](https://img.shields.io/badge/X-Folllow-000000?style=for-the-badge&logo=twitter&logoColor=white)](https://x.com/M1deTheAnalyst)

---

*Built with ❤️ using Power BI | Data-driven insight for legal operations, risk, and firm leadership teams*
