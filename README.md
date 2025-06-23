# Data-Cleaning-Preprocessing

This project involves building a machine learning model to predict passenger survival on the Titanic using structured tabular data. The following steps were carried out:

- **Data Loading & Exploration:** The Titanic dataset was loaded and inspected to understand feature distributions, missing values, and data types.
- **Missing Value Treatment:** Missing values in the `Age` and `Embarked` columns were filled using appropriate statistical methods (median and mode).
- **Categorical Encoding:** The `Sex` and `Embarked` columns were converted into numerical format using label and one-hot encoding techniques.
- **Outlier Detection:** Boxplots were used to visually identify outliers in numerical features such as `Age`, `Fare`, `SibSp`, and `Parch`.
- **Outlier Removal:** Outliers were removed using the Interquartile Range (IQR) method to improve model generalization.
- **Model Training:** A logistic regression model was trained on the cleaned data.
- **Model Evaluation:** The model was evaluated using accuracy, confusion matrix, and a detailed classification report.

Final model accuracy achieved: **84.07%**, demonstrating improved performance after outlier handling.

- 72 passengers who did not survive were correctly predicted
- 23 passengers who survived were correctly predicted
- 7 were wrongly predicted as survived (false positives)
- 11 were actual survivors wrongly predicted as not survived (false negatives)

**Overall Metrics:**
- **Accuracy**: 84.07%
- **Macro Avg F1-Score**: 0.80
- **Weighted Avg F1-Score**: 0.84

The model performs very well in predicting passengers who did not survive and moderately well for those who survived. While a few survivors were missed, overall performance is strong and balanced.
