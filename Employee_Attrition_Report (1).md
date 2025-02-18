# Employee Attrition Prediction Report

## Objective
The objective of this project is to build a classification model to predict whether an employee will leave a company based on HR data and derive actionable retention strategies.

## Dataset Description and Preprocessing Steps

### Dataset Description
The dataset used for this project is the IBM HR Analytics Dataset, which contains various features related to employees' demographics, job roles, and performance metrics. The target variable is `Attrition`, which indicates whether an employee has left the company.

### Preprocessing Steps
1. **Load the Dataset**: The dataset was loaded into a Pandas DataFrame for analysis.
2. **Understand the Dataset**: Basic information about the dataset, such as data types and missing values, was explored.
3. **Handle Missing Values**: Any missing values in the dataset were either imputed or removed.
4. **Encode Categorical Variables**: Categorical variables were converted into numerical format using one-hot encoding to prepare them for machine learning models.
5. **Scale the Data**: Numerical features were standardized to ensure they are on a similar scale, which is important for certain models like Logistic Regression.

## Models Implemented with Rationale for Their Selection

### Models Implemented
1. **Random Forest Classifier**: Random Forest is an ensemble method that is known for its robustness and ability to handle large datasets with higher dimensionality. It can also capture complex interactions between features.
2. **Logistic Regression**: Logistic Regression is a simple and interpretable model that works well for binary classification tasks. It provides insights into the relationship between the target variable and the predictors.

### Rationale for Selection
- **Random Forest**: Selected due to its high performance, ability to handle overfitting, and providing feature importance which helps in understanding the influential factors for attrition.
- **Logistic Regression**: Selected for its simplicity, interpretability, and effectiveness in binary classification problems.

## Key Insights and Visualizations

### Exploratory Data Analysis (EDA)
- **Distribution of Attrition**: Visualized the distribution of the target variable `Attrition` to understand the class imbalance.
- **Age vs Attrition**: Created box plots to visualize the relationship between `Age` and `Attrition`.
- **Feature Relationships**: Analyzed relationships between various features and `Attrition` to identify key factors influencing employee attrition.

### Model Performance
- **Random Forest Classifier**:
  - Classification Report: Provided precision, recall, F1-score, and support for each class.
  - ROC-AUC Score: Evaluated the model's discrimination ability.
- **Logistic Regression**:
  - Classification Report: Provided precision, recall, F1-score, and support for each class.
  - ROC-AUC Score: Evaluated the model's discrimination ability.

### Model Interpretation
- **SHAP (SHapley Additive exPlanations)**: Used to explain the output of the Random Forest model and visualize feature importance.
- **LIME (Local Interpretable Model-agnostic Explanations)**: Used to explain individual predictions of the Logistic Regression model and understand the contribution of each feature.

### Visualizations
- **SHAP Summary Plot**: Visualized the overall feature importance and their impact on the model's output.
- **LIME Explanation**: Visualized the contribution of each feature to an individual prediction.

## Challenges Faced and Solutions

### Challenges
1. **Class Imbalance**: The dataset had an imbalance between the classes for the target variable `Attrition`.
2. **Feature Selection**: Identifying the most important features influencing attrition was challenging due to the high dimensionality of the dataset.
3. **Model Interpretability**: Explaining the predictions of complex models like Random Forest required advanced techniques.

### Solutions
1. **Class Imbalance**: Addressed by using techniques such as stratified sampling during train-test split and using evaluation metrics like ROC-AUC that are less sensitive to class imbalance.
2. **Feature Selection**: Used feature importance scores from Random Forest and SHAP values to identify key features influencing attrition.
3. **Model Interpretability**: Utilized SHAP and LIME to explain model predictions and provide insights into the factors contributing to employee attrition.

## Conclusion
A classification model for employee attrition was successfully built and interpreted using the IBM HR Analytics Dataset. The key factors influencing attrition were identified, and actionable insights were derived to help HR departments develop effective retention strategies.
