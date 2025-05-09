# FSRDC Research Output Dashboard (CIT5900 Project 3)

An interactive dashboard presenting enriched, classified, and analyzed research outputs from Federal Statistical Research Data Centers (FSRDC). Deployed via GitHub Pages.

---

## Live Demo

🔗 https://ruiweny316.github.io/CIT5900_project3/

---

## Overview

This project collects, cleans, and analyzes research outputs from multiple sources (OpenAlex API, RePEc, FSRDC-verified Excel), then:

1. **Data Enrichment & Curation**  
   - Merged 8 Excel metadata tables via `pandas`  
   - Standardized 17 fields, removed duplicates, imputed missing values  
   - Applied exact & fuzzy matching to filter true FSRDC outputs  
   - Queried OpenAlex API & web-scraped RePEc for citations, dates, abstracts, topics  

2. **Topic Classification & Modeling**  
   - Fine-tuned BERT to assign each paper to one of five topic categories  
   - Tracked topic shares over time; surfaced late-series upticks in Growth & Rural Infrastructure  

3. **Exploratory Data Analysis**  
   - Top RDCs by volume & average citations  
   - Publication trends (year vs. count)  
   - Top 10 authors by output & citations (h-index & raw counts)  
   - Citation trajectories vs. age (scatter/density)  

4. **Statistical Modeling**  
   - Linear regression: citation count ~ age + topic + interactions (R²≈0.07)  
   - Random Forest: moderate predictive power (R²≈0.08)  
   - PCA & k-means clustering on topic embeddings  

5. **Network Analysis**  
   - Built undirected graph linking outputs by RDC & topic  
   - 918 nodes, 13 635 edges, 51 connected components (largest: Boston + Demographics)  

6. **Supplementary Figures**  
   - Comparison with FSRDC-verified 2024 dataset  
   - Static topic evolution and BERTopic breakdown  

---

## Repository Structure

