# British Airways Reviews Analysis (2015–2023)

**Goal:** Identify which factors most influence customer satisfaction on British Airways flights and highlight areas of concern.  
**Data:** [British Airways Reviews Dataset on Kaggle](https://www.kaggle.com/datasets) (2015–2023).  
**Tech:** Python (pandas, matplotlib, plotly), text mining, geospatial mapping, Jupyter.

## Key Questions & Insights

1. **How have reviews changed over time?**  
   - Negative reviews (1–4 stars) consistently surpassed positive reviews (8–10 stars).  
   - 2017 showed the sharpest spike in negative ratings, hinting at deeper operational issues.  

2. **Where are the lowest-rated routes?**  
   - Long-haul flights such as **London–Tampa** and **London–Luanda** stand out as worst performing.  
   - Geographic mapping exposed clusters of underperforming long-distance routes.  

3. **What are the most common complaints on these routes?**  
   - Crew complaints dominated, followed by issues with delays, seating, and food.  
   - Suggests service quality is the core driver of dissatisfaction.  

4. **Do these passengers recommend BA?**  
   - Majority on low-rated routes would *not* recommend BA.  
   - London–Luanda route had the strongest negative recommendation rate.  

5. **Which complaints most damage loyalty overall?**  
   - **Delays** had the strongest correlation with “not recommend.”  
   - Operational reliability emerged as the biggest reputational risk factor.

## Repo Map
- src/ — Python scripts (EDA, analysis, visualizations)    
- `data/sample/` — small demo subset of the Kaggle dataset  
- `reports/figures/` — exported charts, maps, and screenshots  

## How to Reproduce
```bash
conda env create -f ../../environment.yml && conda activate ba-portfolio
jupyter lab```
