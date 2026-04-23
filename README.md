# Spatial Analysis of Diabetes in the Census Tracts across Toronto, Peel, and York region

## Overview

This project analyzes the spatial distribution of diabetes across census tracts in Toronto, Peel, and York regions. It uses spatial statistics and regression models to identify geographic patterns and examine how socioeconomic factors such as education and income influence diabetes prevalence.

The study highlights spatial inequalities in health outcomes and demonstrates how GIS can support public health decision-making.

## Objective

Diabetes prevalence is unevenly distributed across the Greater Toronto Area. This project aims to:

Examine whether diabetes is spatially clustered
Analyze relationships between diabetes and education levels
Identify high-risk areas based on socioeconomic conditions
Evaluate how spatial processes influence health outcomes
Data
Diabetes prevalence (CCHS / SimplyAnalytics, 2025)
Census tract boundaries (Statistics Canada, 2021)
Education levels (CHASS Census Data, 2021)
Median income data
Recreational facilities (ODRSF, 2021)

Study Area: Toronto, Peel, and York Regions
Total units: ~1059 census tracts

## Methods
Data cleaning and preprocessing (handling nulls, standardizing variables)
Spatial weights matrix (Queen contiguity)
Exploratory Spatial Data Analysis (ESDA)
Global Moran’s I (spatial clustering)
Local Moran’s I (LISA) for hotspot detection
Bivariate Moran’s I for spatial relationships
Correlation and regression analysis (OLS)
Spatial regression models (Spatial Lag & Spatial Error)
Clustering (K-means & Ward’s method)

## Key Findings
Diabetes shows significant spatial clustering (Moran’s I ≈ 0.53)
Higher diabetes rates are associated with:
Higher % of the population with no certificate
Lower postsecondary education
Weak relationship with high school education alone
Strong spatial divide:
High diabetes + low income/education → Toronto & Brampton
Low diabetes + high education → York Region
Education explains only ~10% of variation → other factors also important
Tools & Technologies
ArcGIS Pro
Python (PySAL, Pandas, NumPy, Matplotlib)
Spatial statistics (Moran’s I, LISA)
Regression modeling
GIS data visualization

## Limitations
Data from different years (2021–2025 mismatch)
Missing census tracts in clustering analysis
Use of aggregated data (ecological fallacy risk)
Limited explanatory power (low R²)
Does not include factors like diet, ethnicity, or healthcare access

## Conclusion
The analysis shows that diabetes prevalence is not random but spatially structured and strongly linked to socioeconomic conditions. Education, particularly postsecondary attainment, plays a key role, but broader environmental and social factors also contribute to health disparities.
