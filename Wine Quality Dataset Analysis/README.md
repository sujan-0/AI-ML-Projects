Wine Quality Dataset Analysis

Overview

This repository contains a Python-based analysis of the Wine Quality Dataset from Kaggle (2021, M Yasser H). The project, implemented in the Jupyter Notebook Wine_Model.ipynb, examines chemical properties of wines and their quality ratings through data loading, inspection, cleaning, and visualization.

Dataset

The WineQT.csv dataset includes 1143 rows and 13 columns, capturing wine characteristics such as:





Fixed Acidity: Non-volatile acidity.



Volatile Acidity: Evaporative acidity.



Citric Acid: Freshness contributor.



Residual Sugar: Post-fermentation sugar.



Chlorides: Salt content.



Free/Total Sulfur Dioxide: Preservatives.



Density: Mass per volume.



pH: Acidity/alkalinity measure.



Sulphates: Flavor and preservation aid.



Alcohol: Alcohol percentage.



Quality: Quality score (target).



Id: Unique identifier.

Tasks Performed





Data Loading: Loaded WineQT.csv from Google Drive using pandas.



Data Inspection: Analyzed dataset size (1143 rows, 13 columns), data types (float64), and missing values (e.g., 36 in fixed acidity, 32 in quality).



Data Cleaning: Imputed missing values with the median to handle outliers and skewed distributions.



Visualization: Generated a correlation matrix heatmap (heatmap_beautiful.png) using seaborn, revealing:





Positive correlations: fixed acidity & density, free sulfur dioxide & total sulfur dioxide.



Negative correlations: volatile acidity & quality, pH & fixed acidity.

Repository Contents





Wine_Model.ipynb: Jupyter Notebook with the complete analysis.



Output: heatmap_beautiful.png (saved to Google Drive).



Dataset: WineQT.csv (not included; source from Kaggle or place in Google Drive).

Requirements





Python 3.x



Libraries: pandas, seaborn, matplotlib, google.colab



Google Drive for dataset access and output storage