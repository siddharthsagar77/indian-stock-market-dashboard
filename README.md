<h1 align="center">📈 Indian Stock Market — Power BI Analytics Dashboard</h1> <p align="center">A Business Intelligence report on company fundamentals, valuation & quality analysis of listed Indian equities.</p> <p align="center"> <img src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" /> <img src="https://img.shields.io/badge/DAX-217346?style=for-the-badge&logo=microsoft&logoColor=white" /> <img src="https://img.shields.io/badge/Domain-Equity%20Research-2E9EF7?style=for-the-badge" /> <img src="https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge" /> </p>
🧭 Overview

The Indian Stock Market dashboard is a single-page, interactive Power BI report that evaluates a universe of Indian listed companies across four fundamental dimensions:

Dimension	Metric
Valuation	PE Ratio
Capital Efficiency	ROCE
Scale	Market Capitalisation
Growth Momentum	Quarterly Profit & Sales Growth

Each company is automatically classified into Quality / Value / Overvalued buckets using rule-based DAX logic — turning raw fundamentals into an instant investment screening tool, with no manual analysis required.

	
Tool	Microsoft Power BI Desktop (.pbix)
Scope	Indian Listed Equities — Fundamentals & Valuation
Report Date	August 2026
🎯 Objectives
Consolidate Fundamentals — unify Market Cap, ROCE, PE Ratio, Profit Growth, and Sales Growth into a single view.
Automate Classification — tag companies as Quality, Value, or Overvalued via rule-based DAX, eliminating manual screening.
ROCE Segmentation — surface capital-efficiency leaders and laggards.
Valuation Stance — assess market-wide cheap vs. fair vs. expensive positioning via PE distribution.
Growth Health Check — instantly see how many companies are growing vs. declining.
Interactive Exploration — drill down by company and market-cap category via cross-filtering slicers.
🏗️ Tools & Data Model
Component	Details
BI Tool	Microsoft Power BI Desktop (.pbix)
Data Table	Indian Stock Market — one row per company (Company, Market Cap Crore, ROCE %, PE Ratio, Current Price INR, Quarterly Profit/Sales Growth %, Market Cap Category, Highest ROCE Value, Largest Market Cap Company)
Measures Table	Indian Stock Market Measures — 25+ DAX measures (totals, averages, min/max, rule-based counts)
Report Canvas	1 page (1366 × 768) — 29 visual objects: 5 KPI cards, 2 bar charts, 2 donut charts, 2 clustered column charts, 1 gauge, 2 slicers
Interactivity	Dropdown slicers for Company and Market Cap Category drive cross-filtering across every visual
📊 Dashboard Layout

The canvas is organized into three functional zones:

🔹 KPI Strip (Top) — Total Market Cap, Quality Companies, Average ROCE %, Average PE Ratio, Total Companies.

🔹 Comparative Charts (Middle) — Top 5 by Market Cap, Top 5 by ROCE %, Quality/Value/Overvalued split, PE Valuation distribution.

🔹 Diagnostics (Bottom) — Growth Health Check, ROCE Quality Split, Average ROCE gauge, Highest ROCE / Largest Market Cap spotlight cards.

<details> <summary><b>Full visual inventory (click to expand)</b></summary>
#	Visual	Type	Fields / Measures Used
1	Total Market Cap	KPI Card	Total Market Cap
2	Quality Companies	KPI Card	Quality Companies
3	Average ROCE %	KPI Card	Average ROCE %
4	Average PE Ratio	KPI Card	Average PE Ratio
5	Total Companies	KPI Card	Total Companies
6	Top 5 by Market Capitalisation	Bar Chart	Company × Sum(Market Cap Crore)
7	Top 5 by ROCE %	Bar Chart	Company × Sum(ROCE Percent)
8	Quality vs Value vs Overvalued	Donut Chart	Quality / Value / Overvalued Companies
9	Valuation Distribution	Donut Chart	High / Fair / Low PE Stocks
10	ROCE Quality Split	Clustered Column	Companies with ROCE <10% / >20%
11	Growth Health Check	Clustered Column	Positive/Negative Profit & Sales Growth
12	Average ROCE Gauge	Gauge	Average ROCE %
13	Highest ROCE Value	KPI Card	Highest ROCE Value
14	Largest Market Cap Company	KPI Card	Largest Market Cap Company
15	Company Filter	Slicer	Company
16	Market Cap Category Filter	Slicer	Market Cap Category
</details>
🧮 KPI & Measure Definitions

All classification logic is defined centrally in the DAX measures table, ensuring consistent, auditable screening criteria across every visual.

Measure / Segment	DAX Logic
Quality Companies	ROCE % ≥ 20 AND Quarterly Profit Growth % > 0 AND Quarterly Sales Growth % > 0
Value Companies	PE Ratio < 20 AND ROCE % > 20
Overvalued Companies	PE Ratio > 50
Low PE Stocks	PE Ratio < 15
Fair PE Stocks	15 ≤ PE Ratio ≤ 30
High PE Stocks	PE Ratio > 30
ROCE Leaders	ROCE % > 20
ROCE Laggards	ROCE % < 10
Positive/Negative Profit Growth	Quarterly Profit Growth % > 0 / < 0
Positive/Negative Sales Growth	Quarterly Sales Growth % > 0 / < 0
Average Profit Margin Indicator	AVERAGE(Profit Growth %) + AVERAGE(Sales Growth %)
Average ROCE-to-PE Ratio	AVERAGE(ROCE %) ÷ AVERAGE(PE Ratio) — blended efficiency-per-valuation score
Average Market Cap per Company	Total Market Cap ÷ Total Companies
🔍 Analytical Insight Framework
Market Composition & Scale — Total/Average Market Cap and Top-5-by-Market-Cap identify the mega-caps driving overall sentiment.
Capital Efficiency (ROCE) — Average ROCE gauge + ROCE Quality Split flag efficient operators vs. potential red flags.
Valuation — PE distribution (Low/Fair/High) shows whether the market is cheap, fair, or running hot.
Quality vs. Value vs. Overvalued Screening — the dashboard's core output: segments the universe for stock-picking or risk flagging.
Growth Momentum — Growth Health Check gives a pulse on how many companies are expanding vs. contracting.
Spotlight Companies — Highest ROCE and Largest Market Cap cards anchor further research.
🚀 How to Use
Open Indian_Stock_Market.pbix in Power BI Desktop.
Use the Company and Market Cap Category slicers to filter the entire report.
Read live KPI values directly off the cards, or use Copy visual as image/data to export any chart.
To refresh with new quarterly data, replace the source rows in the Indian Stock Market table — all 25+ measures and classifications recalculate automatically.
🛠️ Skills Demonstrated

Power BI · DAX · Data Modeling · Business Analytics · Equity Fundamentals · Dashboard Design · KPI Design · Rule-based Classification

📌 Conclusion

This project demonstrates a compact, rule-driven framework for screening Indian listed companies on quality, value, and valuation risk — centralizing 25+ DAX measures into 3 auditable screening buckets across a single, fully refreshable 29-visual canvas.

<p align="center">Built by <a href="https://www.linkedin.com/in/siddharth-sagar-050a70265/">Siddharth Sagar</a> · 📧 siddharth.sagar77@gmail.com</p>
