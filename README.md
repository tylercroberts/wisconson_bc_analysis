# Wisconson Breast Cancer Data Exploration and Analysis

This project takes a look at the University of Wisconson's diagnostic data classification of potential breat cancer tumors. In it, I perform feature selection to reduce the number of features used from 30 to 5, which will allow diagnosticians to identify the most important measurements necessary to identify malignant tumors. After performing feature selection, I fit several models in order to compare effectiveness at tumor classification.


All of the analysis is done in a Jupyter notebook, and to replicate it, simply clone the GitHub repository, and run all cells in the notebook.

The dataset can be found inside this repository, but for more information such as a data dictionary, references, and other details, please see the official site [here](http://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29)

### Dataset Description
The data description for my chosen data set can be found [here.](http://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.names)

In our dataset, we have 3 broad groups of features, each of which is a different statistic for a given tumor measurement.

The three broad groups are:
1. Average - denoted `avg`
2. Standard Error - denoted `se`
3. Worst (mean of the 3 largest values) - denoted `wor`


The 10 measurements we have are as follows:
1. radius (mean of distances from center to points on the perimeter) - denoted `_rad`
2. texture (standard deviation of gray-scale values) - denoted `_text`
3. perimeter - denoted `_peri`
4. area - denoted `_area`
5. smoothness (local variation in radius lengths) - denoted `_smooth`
6. compactness (perimeter^2 / area - 1.0) - denoted `_compact`
7. concavity (severity of concave portions of the contour) - denoted `_concav`
8. concave points (number of concave portions of the contour) - denoted `_conc_p`
9. symmetry - denoted `_symm`
10. fractal dimension ("coastline approximation" - 1) - denoted `_fractal`


All features are named according to: `<group><measurement>` in the dataframe used for this analysis


### Software Requirements
|Software|Package Requirements|
|:-:|:-:|
|Python|os, sys, numpy, pandas, matplotlib, sklearn, pickle, seaborn|


### References:
Lichman, M. (2013). UCI Machine Learning Repository [http://archive.ics.uci.edu/ml](http://archive.ics.uci.edu/ml). Irvine, CA: University of California, School of Information and Computer Science.
