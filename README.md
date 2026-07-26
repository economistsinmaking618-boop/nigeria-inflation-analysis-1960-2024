# The Price of Everything: Nigeria's Inflation Story, 1960–2024

A data analysis of Nigeria's annual inflation rate across 65 years of post-independence economic history, using World Development Indicators (WDI) data.

## Overview

This project analyzes Nigeria's official annual inflation rate from 1960 to 2024 (65 yearly observations) to answer two questions:
1. Is inflation trending upward over time?
2. Does high inflation in one year predict high inflation in the next?

## Key Findings

- **Average inflation (1960–2024):** 16.26%
- **Highest recorded:** 72.84% (1995)
- **Lowest recorded:** -3.73% (1967)
- **Standard deviation:** 14.99%

### Regression Results (AR(1) Model)

| Variable | Coefficient | P-value | Significant |
|---|---|---|---|
| Constant | 10.693 | 0.3925 | No |
| Time Trend | 0.179 | 0.6475 | No |
| AR(1) (prior-year carry-over) | 0.627 | 0.000 | Yes |

**R-squared:** 41.7% · **Durbin-Watson:** 1.663

### Interpretation

- **No significant time trend.** Nigeria's inflation is not on a steady upward march — it spikes during specific shocks (oil boom, SAP devaluation, military-era money printing, 2023 subsidy removal) rather than worsening gradually.
- **Strong persistence.** The AR(1) coefficient (0.627, p < 0.001) shows ~63% of one year's inflation carries into the next — explaining why relief in the headline rate rarely feels immediate to households.
- **Governance-driven, not structural.** Each major spike maps to an identifiable policy decision or failure, rather than an inevitable economic law.

## Decade Breakdown

| Decade | Avg. Inflation | Context |
|---|---|---|
| 1960s | ~0% | Post-independence stability |
| 1970s | ~16% | Oil boom overspending |
| 1980s | ~21% | SAP devaluation shock |
| 1990s | ~31% | Worst decade — military-era money printing, 1995 peak at 72.84% |
| 2000s | ~12% | Democratic transition, inflation targeting |
| 2010s | ~11% | Relative stability |
| 2020s | ~22%+ | COVID supply shocks, 2023 subsidy removal, naira devaluation |

## Dashboard Interpretation

**1960s — The Hopeful Beginning:** Near-zero average inflation. A young, largely agricultural economy with stable prices — the foundation that oil money would later erode.

**1970s — Oil Money Brings a New Problem:** Oil wealth triggered heavy government spending and an import surge. Nigerians were richer on paper, but inflation quietly ate into that wealth.

**1980s — The SAP Shock:** The 1986 Structural Adjustment Programme devalued the naira overnight and removed subsidies. Imported goods became sharply more expensive, and inflation accelerated.

**1990s — Nigeria's Worst Decade:** The highest average inflation of any decade in the dataset. Military governments printed money without discipline, the naira collapsed, and 1995 hit 72.84% — the single worst year in 65 years. Savings were wiped out and the middle class shrank.

**2000s–2010s — Recovery and Relative Calm:** Return of democracy, CBN inflation targeting, and debt restructuring brought averages down to roughly 12% and 11% — still high globally, but genuine relief after the 1990s.

**2020s — The Storm Returns:** COVID-19 supply disruptions, the 2023 fuel subsidy removal, and a sharp naira devaluation pushed inflation back toward 1990s levels. The trend line curves upward at the most recent end of the data — this decade's story is still being written.

## Conclusion: What 65 Years of Data Teaches Us

- **Inflation always comes back down.** Even after 1995's extreme, the data shows inflation reverting toward its long-run average. The problem is not permanent or irreversible.
- **Inflation is not worsening with every generation.** It does not creep upward decade over decade — it explodes during specific crises, most tied to poor governance, then stabilizes when better decisions are made. The enemy is not time; it is policy failure.
- **Once inflation starts, it's hard to stop quickly.** The AR(1) finding — that 63% of one year's inflation carries into the next — means delay is costly. Every month a government waits to act, the problem compounds.
- **Nigeria's inflation story is fundamentally a governance story.** Every major spike traces back to a specific decision or failure: 1970s oil boom overspending, the 1986 SAP devaluation, 1990s military-era money printing, the 2023 subsidy removal. Inflation in Nigeria is not an act of God — it is largely an act, or failure to act, of those who hold power.

## Methodology & Tools

- **Data:** World Development Indicators (WDI), 1960–2024 annual inflation rate
- **Microsoft Excel** — data cleaning and organization
- **EViews** — OLS regression with AR(1) correction, unit root/stationarity testing
- **Tableau** — interactive dashboard (trend line + decade comparison)

## Dashboard

![Nigeria Inflation Rate 1960–2024 Dashboard](images/dashboard.png)

**[Explore the interactive version on Tableau Public →](https://public.tableau.com/views/NigeriaInflationDashboard_17767246903920/Dashboard1)**

## Author

**Mustapha** — Economist & Data Analyst
