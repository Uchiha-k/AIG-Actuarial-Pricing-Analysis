# AIG Actuarial Pricing — Data Analyst Case Study

## Goal
Analyze historical claims data to understand patterns (frequency, severity, geography, cause of loss), then build a transparent premium breakdown and sensitivity insights for decision-making.

## Key questions
- Which claim types and locations drive severity?
- How does claim frequency trend over time?
- What is the baseline premium and how do loadings contribute?
- How sensitive is the premium to severity shocks (+6%)?

## Data understanding
- **Source fields:** Claim ID, Date, Location, Type of Claim, Cause of Loss, Net inflation adjusted claim, Gross Tonnage (exposure), Claim Status.
- **Granularity:** Claim-level rows.
- **Primary metrics:** Frequency (counts), Severity (averages, sums), Exposure proxies (e.g., tonnage).

## Methods (data analyst workflow)
- **Cleaning:** Checked missing values, normalized categories (Type of Claim, Cause of Loss), validated outliers in claim amounts.
- **Exploration:** Trends by year, distribution by type/cause, geography heatmap, severity statistics (mean/median/95th percentile).
- **Feature engineering:** Calculated frequency & severity, derived pure premium, then added loadings (large loss, expenses, profit) for a transparent build-up.
- **Sensitivity:** Applied +6% shock to severity to quantify premium impact.

## Visuals
- **Premium Breakdown Waterfall:** Shows pure premium → loadings → final premium.
- **Sensitivity Impact (cards):** Base vs. +6% severity premium.
- **Claim Type Distribution (donut):** Portfolio composition.
- **Frequency Trend (line):** YOY claims.
- **Geography (bar/map):** Severity hotspots.

## Findings (high-level)
- **Dominant drivers:** [Fill with your observed top claim type/cause]
- **Trend:** [E.g., frequency stable, severity volatile in 2020–2021]
- **Pricing impact:** +6% severity increases premium by ~X%.
- **Actionable:** Focus reviews on high-severity causes and regions; monitor sensitivity bands.

## Tools
Power BI (DAX, visuals, slicers), data profiling and categorization.

## How to view
Dashboard screenshots in `/dashboard-screenshots/`. DAX measures and methods documented for transparency.


