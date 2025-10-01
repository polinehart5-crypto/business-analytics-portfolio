# Bitcoin Market Analysis (2014–2021)

**Goal:** Analyze Bitcoin price/volume trends, daily returns, hypothesis tests and model how volatility relates to trading volume.  
**Data:** coin_Bitcoin (sample of the original CSV provided in `data/sample/`).  
**Tech:** R (ggplot2, readr, dplyr).

## Tasks
1) Trend lines for Close & Volume with summary stats  
2) Daily log returns + histogram + boxplot  
3) Mean tests: 0 (two-sided), 5% and 10% (right-tailed)  
4) Variance test: σ²(return) > 0.10  
5) Regression: `log(Volume) ~ |Return|` + slope significance

## Repo Map
- `src/` — R script (`bitcoin_analysis.R`)
- `data/sample/` — small demo CSV (`coin_Bitcoin_sample.csv`)
- `reports/figures/` — exported plots (see below)
- `reports/` — `Stats_coursework_PH.docx`, `results_summary.txt`

## How to Run (R)
```r
install.packages(c("ggplot2","readr","dplyr"))
setwd("bitcoin_market_analysis/src")
source("bitcoin_analysis.R")
