# Titanic Data Analysis and Survival Prediction

## Project Overview

This project presents an end-to-end analysis of the Titanic passenger dataset. The workflow includes data cleaning, exploratory data analysis, visualization, correlation analysis, feature engineering, machine learning, model evaluation, feature importance analysis, and hyperparameter tuning.

The main objective is to identify factors associated with passenger survival and build classification models to predict survival outcomes.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Analysis Performed

- Data cleaning and missing value handling
- Exploratory data analysis
- Survival rate analysis
- Data visualization
- Feature engineering
- Correlation analysis
- Machine learning model training
- Model performance comparison
- Confusion matrix analysis
- Feature importance analysis
- Hyperparameter tuning using GridSearchCV
- Cross-validation
- Final model selection

## Machine Learning Models

Three classification models were evaluated:

- Logistic Regression
- Decision Tree
- Random Forest

## Model Performance

The original Decision Tree produced the best test performance among the three models.

| Model | Accuracy | Precision | Recall | F1 Score |
|---|---:|---:|---:|---:|
| Logistic Regression | 80.45% | 79.31% | 66.67% | 72.44% |
| Decision Tree | 82.68% | 80.65% | 72.46% | 76.34% |
| Random Forest | 82.12% | 79.41% | 70.00% | 74.63% |

## Hyperparameter Tuning

GridSearchCV was used to tune the Decision Tree model.

The parameters considered were:

- criterion
- max_depth
- min_samples_split
- min_samples_leaf

The best parameter combination was:

- criterion = gini
- max_depth = 10
- min_samples_split = 10
- min_samples_leaf = 1

The best cross-validation F1 score was 75.34%.

## Tuned Model Performance

The tuned Decision Tree achieved:

- Accuracy: 79.33%
- Precision: 75.81%
- Recall: 68.12%
- F1 Score: 71.76%

The tuned model performed lower on the test dataset than the original Decision Tree.

Therefore, the original Decision Tree was retained as the final model.

## Feature Importance

The Decision Tree feature importance analysis showed that the main features influencing predictions were:

- Sex
- Age
- Fare
- Pclass

Sex_female had the highest feature importance at 31.66%, followed by Age at 27.71% and Fare at 22.81%.

## Key Findings

- Female passengers had a higher survival rate than male passengers.
- First-class passengers had a higher survival rate than second and third-class passengers.
- Younger passengers, especially children, showed higher survival rates.
- Passengers travelling with family had a higher survival rate than passengers travelling alone.
- Sex, Age, Fare, and Pclass were the most influential features for the Decision Tree model.

## Final Model

The original Decision Tree was selected as the final model because it achieved the strongest test performance among the evaluated models.

- Accuracy: 82.68%
- Precision: 80.65%
- Recall: 72.46%
- F1 Score: 76.34%

## Conclusion

This project demonstrates an end-to-end data analysis and machine learning workflow using the Titanic dataset. It shows how data cleaning, exploratory analysis, visualization, feature engineering, model evaluation, feature importance analysis, and hyperparameter tuning can be combined to generate useful insights and predictive results.
