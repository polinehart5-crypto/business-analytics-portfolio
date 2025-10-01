# Customer Segmentation & Association Rules

**Goal:** Segment bank customers using clustering and extract association rules to provide actionable insights for financial product design.  

**Data:** Bank marketing dataset (sample of original CSV provided in `data/sample/bank_sample.csv`). 

**Tech:** Python (pandas, scikit-learn, seaborn, mlxtend), K-Means clustering, Apriori algorithm.

---

## Key Questions & Insights
1. **How can the bank leverage customer clusters to tailor financial products?**  
   - K-means grouped customers into 3 clusters:  
     - Cluster 0: Middle-aged, low balance  
     - Cluster 1: Younger, average/low balance  
     - Cluster 2: High balance customers
  - Insight: Marital and job status: cluster 1 has the highest proportion of married and single individuals and management jobs are the most prevalent.

2. **How can association rules help improve customer assessment models for predicting loan defaults?**  
   - Single customers in management, not in default → likely no loan + tertiary education.  

3. **How can the bank optimise resource allocation by identifying high-demand segments?**  
   - Offer savings plans for middle-aged, low-balance customers.  
   - Provide investment/wealth planning to financially stable customers.  
   - Offer small, low-interest loans to younger customers.  

---

## Repo Map
- src/ — Python script (`customer_segmenntation_analysis.py`)  
- data/sample/ — small demo subset of `bank_sample.csv`  
- reports/figures/ — exported plots (clusters, rules)  
- reports/ — presentation and documentation  

---

## How to Reproduce
```bash
pip install -r ../../requirements.txt
python src/customer_segmenntation_analysis.py
