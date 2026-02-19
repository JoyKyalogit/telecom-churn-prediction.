# Telecom Customer Churn Prediction 

## Project Goal
The objective of this project is to build a machine learning model that predicts customer attrition (churn) for a telecommunications provider. By identifying at-risk customers, the business can implement targeted retention strategies to reduce revenue loss.

## The Dataset
The analysis is performed on a dataset containing 7,043 customer records with 21 features, including:
- **Demographics:** Gender, Senior Citizen status, Partners, and Dependents.
- **Services:** Phone service, Multiple lines, Internet (DSL/Fiber optic), and Security/Support add-ons.
- **Account Info:** Tenure, Contract type (Month-to-month, One year, Two year), Payment method, and Charges.

## Technical Workflow
1. **Data Cleaning:** - Handled non-numeric values and nulls in the `TotalCharges` column.
   - Performed data type conversion to ensure all features were ready for modeling.
2. **Exploratory Data Analysis (EDA):** - Visualized churn distribution across different categories.
   - Identified that customers with month-to-month contracts and fiber optic internet had higher churn rates.
3. **Feature Engineering & Scaling:**
   - Encoded categorical variables for machine learning compatibility.
   - Scaled numerical features using `StandardScaler`.
4. **Machine Learning Modeling:**
   - Trained a **Logistic Regression** model for interpretability.
   - Trained a **Random Forest Classifier** to maximize predictive power.
5. **Evaluation:**
   - Utilized a Confusion Matrix to track True Positives/Negatives.
   - Calculated the ROC-AUC score to measure the model's ability to distinguish between churners and non-churners.

## Libraries Used
- **Pandas & NumPy:** Data manipulation and cleaning.
- **Matplotlib & Seaborn:** Statistical data visualization.
- **Scikit-Learn:** Model building, scaling, and evaluation metrics.

