# Exercise 10: Linear Discriminant Analysis (LDA) on River Catchments

## About the Project
This repository contains Exercise 10 for the Green Data Science Master's program. The goal is to perform a Linear Discriminant Analysis (LDA) to classify four river basins (Douro, Tejo, Mondego, and Minho) based entirely on their environmental and hydrological profiles. 

To prevent spatial data leakage, geographic coordinates (Latitude/Longitude) were excluded from the model.

## Environmental Variables Used
The analysis relies on the `EFIplus_medit.csv` dataset, using only physical and climatic predictors:
* **`Altitude`**: Topographical gradient.
* **`Actual_river_slope`**: The actual slope of the river segment.
* **`prec_ann_catch`**: Annual precipitation in the catchment.
* **`temp_ann`**: Mean annual temperature.

## Tools & Libraries
* **Python** (Pandas, NumPy)
* **Scikit-learn** (StandardScaler, LinearDiscriminantAnalysis)
* **Plotly** (Interactive data visualization)
## Results
The script generates an **Interactive Biplot** (also exported as `Exercicio_10_Biplot_Interativo.html`). This plot maps the rivers into the new space defined by the LDA and displays the vectors (loadings) showing exactly how climate and topography drive the ecological differences between the catchments.
