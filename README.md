<h1 align="center">📈 Indian Stock Market — Power BI Dashboard</h1> <p align="center">Fundamental screening tool for Indian listed equities, built to auto-classify companies as <b>Quality</b>, <b>Value</b>, or <b>Overvalued</b> using rule-based DAX logic.</p> <p align="center"> <img src="https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black" /> <img src="https://img.shields.io/badge/DAX-217346?style=flat-square&logo=microsoft&logoColor=white" /> <img src="https://img.shields.io/badge/25+_Measures-blue?style=flat-square" /> <img src="https://img.shields.io/badge/29_Visuals-blue?style=flat-square" /> </p>
Overview

A single-page, fully interactive Power BI report that screens Indian listed companies across four fundamentals — valuation (PE), capital efficiency (ROCE), scale (market cap), and growth momentum (profit & sales growth) — then auto-tags each one into an investable segment. No manual screening required.

What It Does
Classifies companies automatically into Quality / Value / Overvalued buckets via centralized DAX rules
Surfaces capital-efficiency leaders and laggards through ROCE segmentation
Reads market valuation stance — cheap, fair, or expensive — via PE distribution
Flags growth momentum across the covered universe (expanding vs. contracting)
Enables interactive drill-down by company and market-cap category
Build
	
Tool	Power BI Desktop
Data model	1 source table + a dedicated 25+ measure DAX layer
Report	Single canvas, 29 visuals — KPI cards, bar/donut/column charts, gauge, slicers
Core Screening Logic
Quality      → ROCE ≥ 20%  AND  Profit Growth > 0  AND  Sales Growth > 0
Value        → PE < 20     AND  ROCE > 20
Overvalued   → PE > 50

(Full measure list — 25+ rules covering PE bands, ROCE tiers, and growth signals — is documented in the .pbix.)

Skills Demonstrated

Power BI DAX Data Modeling Business Analytics Equity Fundamentals Dashboard Design

<p align="center"> 📁 <a href="https://github.com/siddharthsagar77/indian-stock-market-dashboard/blob/main/Indain%20Stock%20Market.pbix">Open the .pbix</a> · 📄 <a href="https://github.com/siddharthsagar77/indian-stock-market-dashboard/blob/main/Indian-Stock-Market.pdf">Full project report (PDF)</a> </p> <p align="center"> Siddharth Sagar · <a href="https://www.linkedin.com/in/siddharth-sagar-050a70265/">LinkedIn</a> · siddharth.sagar77@gmail.com </p>
