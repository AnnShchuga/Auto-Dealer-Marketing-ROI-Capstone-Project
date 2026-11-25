# Game Analytics Capstone — UA Performance & Anomaly Investigation

Final capstone project of the **Game Analytics** program (GeekBrains):
a full-cycle analysis of a mobile game — from data validation to
actionable recommendations for product and marketing teams.

> Course capstone based on case-study data. Methodology is real; results
> reflect the provided dataset.

---

## Business questions

1. Is the data trustworthy? — duplicates, logical integrity, cross-table
   consistency (installs ↔ DAU ↔ retention ↔ purchases).
2. What anomalies happened during the period, and why? — spikes and dips in
   installs, retention, PPU, DAU, first purchases; hypotheses tested with
   cohort analysis (geography, organic vs. paid).
3. Which ad campaigns performed best? — CPI, LTV, ROI (ARPU where CPI/LTV
   was not computable) broken down by platform, traffic source and campaign.

---

## Approach

### 1. Data quality audit
- Checked for duplicates and inconsistent records across tables
- Validated logical links: installs → DAU → retention → payments
- Documented gaps and unclear columns (see `notes/data_quality.md`)

### 2. Anomaly detection
- Built daily time series for key metrics: installs, DAU, retention rate,
  PPU, first purchases
- Flagged outliers and structural trend changes
- Formulated hypotheses for each anomaly, then confirmed/refuted them with
  cohort cuts by geography and organic/paid acquisition

### 3. Marketing efficiency
- Calculated CPI per campaign, LTV for the whole user base, ROI by source
  and platform; ARPU where cost data was missing
- Ranked campaig
