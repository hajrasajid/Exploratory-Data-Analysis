Exploratory Data Analysis (EDA) – Iris Dataset
📊 Dataset Overview

The Iris dataset contains 150 observations and 6 columns, including:

4 numerical features
1 identifier column
1 categorical target variable (Species)

The dataset is widely used for classification tasks in machine learning.

📌 Feature Description
SepalLengthCm, SepalWidthCm, PetalLengthCm, PetalWidthCm → Continuous numerical features
Species → Target variable with three classes:
Iris-setosa
Iris-versicolor
Iris-virginica
🧹 Missing Values
No missing values were found in the dataset
All 150 entries are complete and clean
🔁 Duplicate Records
A small number of duplicate rows were identified
These duplicates were removed to improve data quality
Final dataset size after cleaning: 147 observations
📈 Key Insights from Summary Statistics
Petal features show higher variance and wider range, making them more informative than sepal features
Petal length has the largest spread → strongest feature for classification
Sepal width shows the least variation → weaker predictive power
Mean ≈ Median for most features → indicates relatively balanced distributions
Slight skewness observed in petal features → helps in species separation
Clear separation in petal values for Iris-setosa
Overlap exists in sepal features, especially between Versicolor and Virginica
🚨 Outlier Detection

Outliers were detected using the Interquartile Range (IQR) method:

Q1 (25th percentile) and Q3 (75th percentile) were calculated
Values outside the IQR bounds were treated as outliers
Outliers were removed to improve model performance and data quality
📊 Distribution Analysis
Petal features (PetalLengthCm, PetalWidthCm) show high variation and clear class separation
Sepal features (SepalLengthCm, SepalWidthCm) are more normally distributed with less separation power
KDE plots confirm that:
Iris-setosa is clearly separable
Versicolor and Virginica show slight overlap
Overall, petal features are more effective for classification than sepal features
🔗 Pairplot Analysis
🌿 Sepal Features
Weak separation between species
Slight positive relationship between sepal length and width
High overlap between Versicolor and Virginica
🌸 Petal Features
Strong clustering of species
Clear separation of Iris-setosa
Strong positive correlation between petal length and width
🧠 General Insights
Petal features are the most informative predictors
Iris-setosa is easily separable from other species
Versicolor and Virginica show some overlap
Sepal features contribute less to classification accuracy
Strong correlation exists between petal length and petal width
🎯 Conclusion

Petal measurements are the most powerful features for distinguishing Iris species, while sepal measurements provide limited predictive value. This makes petal-based features highly important for classification models.data. This method calculates the first (Q1) and third quartiles (Q3) to define upper and lower boundaries. Values outside these limits are treated as outliers and are removed to improve data quality and model performance.

**Distribution Analysis**
The histograms show that petal features (PetalLengthCm, PetalWidthCm) have higher variation and clearer class separation compared to sepal features. This makes petal measurements more important for classification.In contrast, sepal features (SepalLengthCm, SepalWidthCm) are more normally distributed with less variation and weaker class separation.

The KDE plots of the Iris dataset show that petal length and petal width are the most powerful features for species separation, clearly distinguishing Setosa from the other two species. Setosa forms a completely separate cluster, while Versicolor and Virginica show slight overlap mainly in sepal features. Overall, petal measurements are much more effective for classification than sepal measurements.


