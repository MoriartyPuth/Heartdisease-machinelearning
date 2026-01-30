# Heart disease machine learning
# Heart Disease Risk Prediction & Analysis

This project utilizes machine learning to identify key clinical and demographic risk factors for heart disease. By analyzing data from multiple clinical studies (Cleveland, Hungary, Switzerland, and VA Long Beach), the model provides insights into which features most significantly influence a diagnosis.

## 📊 Feature Importance Analysis

The following chart illustrates the absolute importance of each feature in our predictive model. Features with higher values have a greater impact on the final prediction.

<img width="555" height="357" alt="Screenshot 2026-01-31 001053" src="https://github.com/user-attachments/assets/7301393d-f58e-4cae-98f4-83a7b9d1508c" />


*The model primarily relies on regional data sources and specific symptoms like chest pain types to make predictions.*

## 🧬 Key Features Explained

| Feature | Importance Rank | Description |
| :--- | :---: | :--- |
| **Regional Datasets** | 1-4 | Indicates the source location (e.g., Long Beach, Switzerland, Hungary). |
| **cp (Chest Pain)** | 3, 6, 7 | Categorized as atypical angina, typical angina, or non-anginal. |
| **sex_Male** | 5 | Gender classification. |
| **oldpeak** | 9 | ST depression induced by exercise relative to rest. |
| **exang** | 10 | Presence of exercise-induced angina. |
| **restecg** | 8, 11 | Resting electrocardiographic results. |

## 🛠️ Project Structure

- `heart_disease_analysis.ipynb`: Jupyter Notebook containing data cleaning, EDA, and model training.
- `feature_importance.csv`: Exported model coefficients and importance scores.
- `feature_importance_plot.png`: Visualization of feature weights.

## 📈 Model Insights
Our model utilizes Logistic Regression coefficients to determine feature influence:
- **Negative Correlation:** Features like `dataset_VA Long Beach` and `cp_atypical_angina` show strong negative coefficients, meaning their presence significantly lowers the predicted probability of heart disease in this specific dataset.
- **Positive Correlation:** Features like `sex_Male` and `oldpeak` show positive coefficients, indicating an increased risk associated with these factors.
