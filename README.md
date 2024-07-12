# Advanced-Statistical-Analysis-of-Chronic-Disease-Indicators
The goal is to develop robust predictive models to identify patterns in chronic disease data, aiding public health planning and interventions. This project aims to enhance predictive modeling for chronic diseases, leading to better preventative strategies and health outcomes.

1. Project Introduction
1.1 Background
Chronic diseases are major contributors to global morbidity and mortality. This project leverages advanced statistical techniques to analyze chronic disease data from Data.gov, aiming to identify patterns and trends that can inform public health planning and interventions.

![image](https://github.com/user-attachments/assets/1caa3735-b91a-4a9f-b4da-879e00e35f53)


1.2 Project Goal
Develop robust predictive models to uncover patterns in chronic disease data, aiding public health planning and interventions.

2. Data Acquisition and Exploration
2.1 Data Source
The dataset "U.S. Chronic Disease Indicators (CDI)" from Data.gov includes variables related to chronic diseases, demographics, and healthcare utilization.

2.2 Data Loading in R
The dataset is loaded into R using readr and dplyr for comprehensive examination and preprocessing.

3. Data Preprocessing in R
Convert 'YearStart' and 'YearEnd' columns to datetime format.
Transform 'DataValue' to numeric format, handling non-numeric entries.
Check data types and identify missing values.
Visualize 'LocationAbbr' distribution and topic trends over the years.
Clean 'DataValue' column and perform stratified analysis.

![image](https://github.com/user-attachments/assets/00e323b0-2fee-419d-897b-251323b8648f)


4. Exploratory Data Analysis in R
4.1 Initial Data Check and Summary Statistics
Check for missing values and obtain summary statistics for an overview of the dataset.

4.2 Unique Values in Categorical Columns
Analyze uniqueness in categorical variables for insights.

4.3 Visualizations for Insightful Analysis
Use ggplot2 for visualizing data distribution and trends.

![image](https://github.com/user-attachments/assets/0f021fd7-7985-415b-a04e-e609e157b924)


5. Statistical Learning Techniques in R
5.1 Linear Regression
Model the relationship between 'DataValue' and predictor variables. Evaluate with Mean Squared Error (MSE) of 0.856.

5.2 Shrinkage Methods (Lasso, Ridge)
Lasso: Variable selection and regularization with cross-validation.
Ridge: Prevents overfitting, improves generalization.

5.3 Linear Discriminant Analysis (LDA)
Predict 'LocationID' with predictors 'DataValue' and 'YearStart'. Accuracy: 0.024.

5.4 Logistic Regression
Predict binary 'BinaryOutcome' with 'DataValue' and 'YearStart'. Perfect accuracy: 1.

5.5 Nonparametric Logistic Regression (GAM)
Predict 'BinaryOutcome' using splines for complex relationships. Perfect accuracy: 1.

5.6 Kernel Methods (SVMs)
SVMs with radial basis kernel for binary classification. Perfect accuracy: 1.

![image](https://github.com/user-attachments/assets/e1945b02-238c-412f-9509-8ba7ece3c9d2)


Overall Model Performance
Linear regression MSE: 0.856
Lasso RMSE: 1.697
Ridge RMSE: 2.143
LDA accuracy: 0.024
Logistic regression and nonparametric logistic regression accuracy: 1
SVM accuracy: 1
6. Conclusion
The analysis reveals varying model performances, highlighting the complexity of chronic disease prediction. The study provides a foundation for refining models and emphasizes the importance of diverse statistical approaches. Further research could enhance model robustness, aiding public health planning and interventions.

7. References
Amblàs-Novellas et al. (2016). BMJ Open, 6(9), e012340.
Gómez-Batiste et al. (2014). Palliative Medicine, 28(4), 302-311.
Ljubičić et al. (2020). Psychoneuroendocrinology, 117, 104709.
Pham et al. (2019). JMIR mHealth and uHealth, 7(1), e11941.
Marengoni et al. (2016). European Journal of Internal Medicine, 31, 29-34.
