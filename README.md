# Digital Advertising Experiment: Statistical Analysis & Business Decisioning in R

## Executive Overview
This project presents an end-to-end analysis of a large-scale digital advertising experiment,
designed to evaluate the effectiveness of multiple Instagram ad creatives using
statistical testing, ROI analysis, and counterfactual reasoning.

The work demonstrates my ability to:
- Design and analyze randomized experiments
- Apply statistical hypothesis testing correctly
- Translate analytical results into actionable business decisions
- Work fluently in R for data analysis and reporting
- Communicate insights clearly to non-technical stakeholders

---

## Business Problem
A digital retailer ran a randomized experiment across four groups:
three different advertisement creatives (A, B, C) and a control group.
Each impression incurred a fixed cost, and the business needed to decide:

1. Which advertisement(s) should be continued based on profitability
2. Whether the experiment could have been run more efficiently using
   adaptive allocation (e.g., multi-armed bandits)

The goal was not just statistical significance, but **profit-driven decision-making**.

---

## Experiment Design
- Platform: Instagram
- Total sample size: 100,000 users
- Allocation: 25,000 users per group
- Conditions:
  - Ad A
  - Ad B
  - Ad C
  - Control (no ad exposure)
- Cost per impression: $0.20

### Observed Metrics
- Conversion (binary outcome)
- Revenue conditional on conversion

---

## Analytical Approach

### Statistical Testing
- Two-sample proportion tests to estimate incremental conversion lift
- Multiple-testing correction to control false discovery
- Two-sample t-tests to compare revenue among converters
- Confidence intervals used to quantify uncertainty

### Business Metrics
- Incremental cost per conversion
- Profit per incremental conversion
- Return on investment (ROI) by advertisement

### Decision Analysis
- Identification of underperforming ads
- Comparison of traditional A/B testing vs adaptive allocation
- Estimation of lost conversions and profit due to inefficient experimentation

---

## Key Findings
- Ads A and C generated statistically significant lift in conversions and revenue
- Ad B showed poor ROI and should be discontinued
- ROI-based decisioning led to a different conclusion than conversion rates alone
- A multi-armed bandit approach could have:
  - Identified weaker ads earlier
  - Reduced wasted impressions
  - Increased total profit through faster learning

---

## Skills Demonstrated
- Experimental design & causal reasoning
- Hypothesis testing and statistical inference
- Business-driven KPI construction (ROI, CPIC)
- Counterfactual analysis
- R programming and reproducible analysis (R Markdown)
- Translating data into executive-level recommendations

---

## Repository Contents
- `analysis.Rmd` — Fully reproducible R Markdown analysis
- `analysis.pdf` — Rendered report with executive summary
- `IGAds.RData` — Experimental dataset

---

## Context
This project was completed in an academic setting but is intentionally presented
as an applied analytics case study, reflecting how similar analyses are conducted
in real-world marketing, product, and growth analytics roles.

## Collaboration & Contribution
This analysis was completed as part of a small project team.
All statistical analysis, experiment evaluation, and business conclusions
were jointly developed and reviewed by the group.

My personal focus included:
- Implementing the statistical tests in R
- Interpreting results and translating them into business recommendations
- Structuring the analysis for clarity and reproducibility