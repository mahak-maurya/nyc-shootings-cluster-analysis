# NYC Shootings Cluster Analysis

Clustering NYPD Shooting Incident data to identify spatial and temporal 
crime hotspots across New York City, as part of a First Quadrant Labs 
internship project.

## Overview

This project analyzes the NYPD Shooting Incident Data (Historic) dataset 
to uncover patterns in shooting incidents by location, date/time, and 
demographics. Multiple clustering algorithms are compared to find the 
most meaningful and interpretable segmentation.

## Objectives

- Clean and preprocess raw incident-level shooting data
- Engineer temporal and spatial features (time-of-day, day-of-week, 
  precinct/borough, reprojected coordinates)
- Compare clustering algorithms: K-Means, DBSCAN, and HDBSCAN
- Validate clusters using Silhouette Score, Davies-Bouldin Index, and 
  Calinski-Harabasz Index
- Visualize spatial hotspots at borough and precinct level
- Analyze temporal-spatial patterns (repeat geographic clusters, 
  time-of-day trends, victim characteristics by cluster)

## Methodology

1. **Preprocessing** — missing values, duplicate removal, date/time 
   conversion, outlier analysis, coordinate validation, categorical encoding
2. **Feature Engineering** — year/month/day/hour, day-of-week, time-of-day 
   category, geographic features, demographics, precinct/jurisdiction
3. **Clustering** — K-Means vs DBSCAN vs HDBSCAN
4. **Model Selection** — quantitative validation → spatial validation → 
   interpretability
5. **Spatial & Temporal Analysis** — cluster maps, hotspot visualization, 
   borough/precinct-level characteristics

## Ethical Considerations

Demographic fields (victim/perpetrator race) are analyzed with care. 
Clusters are not framed as inherently "high-risk" based on demographic 
composition. Limitations and potential bias in the data and methodology 
are discussed explicitly in the final report.

## Tech Stack

## Tech Stack

- Python (pandas, numpy, scikit-learn, hdbscan)
- Jupyter Notebook
- Matplotlib / Seaborn for visualization
- Power BI / Tableau
## Note on Data

⚠️ The NYPD Shooting Incident dataset is **not included** in this 
repository per project data-sharing restrictions. To reproduce this 
analysis, download the dataset directly from the NYC Open Data portal.


## Deliverables

- `NYC_Shootings_Cluster_Analysis.ipynb` — full analysis and modeling
- Final report (presentation)
- Power BI / Tableau dashboard
