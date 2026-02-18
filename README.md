# Dataset Description – Global COVID-19 Statistics (February 2026)

## Overview

This dataset provides a **point-in-time snapshot** of COVID-19 statistics across **238 countries and territories** as of **February 16, 2026**. It captures cumulative pandemic metrics including confirmed cases, deaths, active cases, and testing data, along with population-normalized rates for fair cross-country comparisons.

---

## Source

- **API:** `covid-193.p.rapidapi.com` (api-sports.io)
- **Date Extracted:** February 16, 2026
- **Original Inspiration:** Our World in Data and API-sourced COVID trackers

---

## File Information

| Item | Details |
|------|---------|
| File Name | `covid19_global_statistics_2026.csv` |
| Format | CSV (Comma-Separated Values) |
| Rows | 238 (one per country/territory) |
| Columns | 13 |
| Date of Data | 2026-02-16 (one-time snapshot) |

---

## Column Descriptions

| Column | Type | Description |
|--------|------|-------------|
| `continent` | String | Continent the country belongs to |
| `country` | String | Country or territory name |
| `population` | Float | Estimated population |
| `date` | Date | Date of the snapshot (2026-02-16) |
| `new_cases` | Float | New cases reported on the snapshot date (many missing) |
| `active_cases` | Float | Number of currently active cases |
| `cases_per_million` | Float | Total confirmed cases per 1 million population |
| `total_cases` | Integer | Cumulative confirmed COVID-19 cases |
| `new_deaths` | Float | New deaths reported on snapshot date (many missing) |
| `deaths_per_million` | Float | Total deaths per 1 million population |
| `total_deaths` | Float | Cumulative confirmed COVID-19 deaths |
| `tests_per_million` | Float | Total tests conducted per 1 million population |
| `total_tests` | Float | Cumulative number of COVID-19 tests performed |

---

## Important Notes

- **Historical snapshot only** — this is NOT a live or updating dataset
- **Missing data** is common for `new_cases`, `new_deaths`, `total_tests`, and `tests_per_million`, especially in African nations and small territories
- **Includes territories and small islands** (e.g., Saint Helena, Falkland Islands) — these may skew per-million metrics
- **Use per-million columns** for fair cross-country comparisons to avoid population-size bias
- Data quality varies significantly by country due to differences in reporting infrastructure

---

## Use Cases

- Exploratory Data Analysis (EDA)
- Regional pattern analysis (continental comparison)
- Mortality trend analysis (Case Fatality Rate)
- Testing disparity study
- Practice for data cleaning and imputation techniques

---

## Assignment Submission Contents

1. `covid19_global_statistics_2026.csv` — Dataset file
2. `README.md` — This dataset description file
3. `EDA_COVID19_Assignment1.ipynb` — Jupyter Notebook with full EDA
