Customer Churn Prediction
📊 Project Overview
This project implements a comprehensive machine learning pipeline to predict customer churn for a telecommunications company. The analysis includes data preprocessing, exploratory data analysis (EDA), and implementation of three different classification models to identify customers at risk of churning.
📁 Dataset
The dataset (customer.churn.datak.xlsx) contains customer demographic information, service subscription details, account information, and churn status. Key features include:

Demographics: Gender, SeniorCitizen status, Partner, Dependents

Services: PhoneService, MultipleLines, InternetService, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, StreamingMovies

Account Information: Contract type, PaperlessBilling, PaymentMethod, MonthlyCharges, TotalCharges, Tenure

Target Variable: Churn (Yes/No)
🚀 Features
Data Processing
Cleaning: Handling missing values in TotalCharges

Preprocessing:

Numerical features: Standard scaling with median imputation

Categorical features: One-hot encoding with mode imputation

Feature Engineering: Automated pipeline using scikit-learn's ColumnTransformer
Models Implemented
Logistic Regression: Baseline model for classification

Random Forest: Ensemble learning method

XGBoost: Gradient boosting algorithm

Evaluation Metrics
Accuracy

Precision

Recall

F1 Score

ROC-AUC Score

Confusion Matrix
Visualizations
Churn distribution analysis

Feature distributions by churn status

Correlation heatmaps

ROC curves

Feature importance plots
📈 Results
Model	Accuracy	Precision	Recall	F1 Score	ROC-AUC
Logistic Regression	0.5009	0.4925	0.3983	0.4404	0.4746
Random Forest	0.4949	0.4874	0.4672	0.4771	0.4974
XGBoost	0.5026	0.4957	0.4983	0.4970	0.4906
Best Model: Random Forest (based on ROC-AUC)
💡 Key Insights
The project reveals several important findings:

Balanced Dataset: The churn distribution is nearly balanced (50.7% No Churn, 49.3% Churn)

Model Performance: All three models perform slightly above random chance, indicating the complexity of churn prediction

Feature Importance: Key factors influencing churn include tenure, contract type, and monthly charges

Churn Indicators: Customers with month-to-month contracts, shorter tenure, and higher monthly charges show higher churn rates

🛠️ Installation
# Clone the repository
git clone https://github.com/yourusername/customer-churn-prediction.git

# Navigate to the project directory
cd customer-churn-prediction

# Install required packages
pip install pandas numpy matplotlib seaborn scikit-learn xgboost openpyxl
📦 Dependencies
Python 3.7+

pandas

numpy

matplotlib

seaborn

scikit-learn

xgboost

openpyxl (for Excel file handling)

📊 Usage
Upload the dataset: Run the notebook and upload the Excel file when prompted

Data preprocessing: Automatic cleaning and feature engineering

Model training: All three models are trained and evaluated

Prediction: Use the best model for new customer prediction
📈 Visualizations
The project includes:

Churn distribution charts

Box plots of numerical features by churn status

Contract type vs churn analysis

Feature correlation heatmaps

Confusion matrices for each model

ROC curves showing model performance

Feature importance rankings
🔍 Future Improvements
Implement hyperparameter tuning with GridSearchCV

Explore additional algorithms (SVM, Neural Networks)

Feature engineering for interaction terms

Time-series analysis for customer behavior patterns

Deployment as a web service for real-time predictions
📝 Conclusion
This customer churn prediction project demonstrates a complete machine learning workflow for a business problem. While the models show modest predictive power due to the complexity of human behavior, the analysis provides valuable insights into customer churn drivers and establishes a foundation for more advanced predictive systems.

📚 References
Customer Churn Dataset

Scikit-learn Documentation

XGBoost Documentation
👥 Author
kirti Meshram
Bsc(Data Scince)
