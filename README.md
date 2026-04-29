# Exploratory-Data-Analysis

**Dataset Overview**
The Iris Dataset contains 150 observations and 6 columns, including four numerical features , one identifier column, and one categorical target variable.

**Feature Description**
Sepal and petal measurements (SepalLengthCm, SepalWidthCm, PetalLengthCm, PetalWidthCm) are continuous variables
Species represents the target class with three categories are Iris-setosa, Iris-versicolor, Iris-virginica.

**Missing Values**
No missing values are present in the dataset
All columns contain complete data for all 150 entries

**Duplicate Records**
A small number of duplicate entries were identified based on feature values
These duplicates were removed to improve data quality
Final dataset size after cleaning: 147 observations

**Key Insights from Summary Statistics**
Petal features are more informative than sepal features (higher variance and wider range) → better for classification
Petal length has the largest spread, making it the strongest feature for distinguishing species
Sepal width shows the least variation, so it contributes less to classification
Mean ≈ Median for most features, indicating relatively balanced distributions
Petal features show slight skewness, suggesting class separation patterns
Clear difference in petal measurements helps easily identify Iris-setosa
Overlap exists in sepal features, especially between Iris-versicolor and Iris-virginica

**Outlier Detection Method**
Outliers were identified using the Interquartile Range (IQR) method, which detects extreme values based on the spread of the data. This method calculates the first (Q1) and third quartiles (Q3) to define upper and lower boundaries. Values outside these limits are treated as outliers and are removed to improve data quality and model performance.






