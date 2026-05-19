![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0%2B-orange?logo=scikit-learn&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

# Credit Risk Analysis: Business Owner Financial Segmentation

Unsupervised clustering analysis to segment small business owners by financial characteristics and credit risk profile.

## Project Overview

Applied K-Means clustering and PCA dimensionality reduction to identify distinct financial risk segments among business owners. This analysis helps financial institutions understand their customer base and tailor credit products accordingly.

## Key Techniques

### K-Means Clustering
- Identified optimal number of clusters (k=2 to k=12)
- Tracked inertia and silhouette scores
- Selected k based on silhouette analysis
- Standardized features for distance metric validity

### Principal Component Analysis (PCA)
- Reduced high-dimensional financial features to 2D
- Preserved 80%+ of variance
- Visualized cluster separation in reduced space
- Interpreted principal components as financial metrics

### Feature Analysis
- Identified high-variance financial characteristics
- Analyzed cluster centroids in original feature space
- Inverse transformation to understand business segments
- Profiled each cluster's financial profile

## Dataset Details

**Features:** Financial characteristics of business owners
- Revenue metrics
- Profitability measures
- Debt ratios
- Working capital indicators

**Approach:**
1. Standardized all features (mean=0, std=1)
2. Fit K-Means for k=2 to k=12
3. Calculated silhouette scores for each k
4. Selected optimal k based on silhouette analysis
5. Applied PCA for 2D visualization
6. Analyzed each cluster's characteristics

## Project Structure
```
credit-risk-clustering/
├── credit_risk_us.py
├── requirements.txt
└── README.md
```

## How to Run

```bash
pip install -r requirements.txt
python credit_risk_us.py
```

## Key Learnings

1. **Silhouette Analysis:** More reliable than inertia alone for optimal k selection
2. **Feature Standardization:** Essential for K-Means (distance-based algorithm)
3. **PCA Interpretation:** Principal components often represent composite financial metrics
4. **Cluster Profiling:** Real value comes from understanding what each cluster represents
5. **Inverse Transformation:** Important for translating PCA results back to actionable business insights

## Technologies Used
- **Data Processing:** pandas, numpy
- **Machine Learning:** scikit-learn (KMeans, PCA, StandardScaler)
- **Visualization:** matplotlib, seaborn

## References
- K-Means Clustering: MacQueen, J. (1967). Some methods for classification and analysis of multivariate observations
- PCA: Pearson, K. (1901). On lines and planes of closest fit to systems of points in space
- Silhouette Analysis: Rousseeuw, P. J. (1987). Silhouettes: A graphical aid to the interpretation and validation of cluster analysis

---

**Author:** Harshit  
**GitHub:** https://github.com/Harshit-sys169
