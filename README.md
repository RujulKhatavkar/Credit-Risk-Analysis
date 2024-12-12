# 📊 Credit Risk Analysis

Welcome to the **Credit Risk Analysis** project! This repository contains a Jupyter Notebook that analyzes credit risk using advanced data science techniques. The analysis leverages a dataset of loan data from 2007 to 2014 to identify risk patterns and predict potential defaults. 📈

---

## 🌟 Features

- 🔍 Exploratory Data Analysis (EDA) for insightful visualizations
- 🧠 Machine Learning models for credit risk prediction
- 📂 Data preprocessing and feature engineering
- 📉 Model evaluation metrics and performance tracking
- 📜 Interpretability and explainability of results

---

## 🛠️ Installation

Follow these steps to set up the project:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/credit-risk-analysis.git
   cd credit-risk-analysis
   ---

2. **Install dependencies**:
   Ensure you have Python 3.8+ and pip installed, then run:
```
bash
pip install -r requirements.txt
```
3. **Dataset downloading**:
    Place the dataset in the data/ directory. Ensure the dataset is named appropriately or update the notebook paths accordingly.

Run the notebook: Start Jupyter Notebook or JupyterLab:
```
bash
jupyter notebook Credit\ Risk\ Analysis.ipynb
```
## 📂 Methodology

### 1. Data Import and Exploration
- **Data Loading**: The dataset was read into a DataFrame using pandas, with all columns and rows displayed for better visibility.
- **Initial Shape**: The dataset contained a large number of rows and columns, indicating the complexity and richness of the dataset.
- **Column Overview**: The `Unnamed: 0` column (index) was dropped as it was redundant. The dataset was then divided into numerical and categorical subsets for targeted analysis.

### 2. Data Cleaning
- **Missing Values**: A detailed examination of missing values was performed, and appropriate imputation or column removal strategies were applied.
- **Type Conversion**: Certain columns were converted to their appropriate data types (e.g., numeric or categorical) to enable accurate computations.
- **Outlier Handling**: Numerical columns were analyzed for outliers using statistical summaries.

### 3. Exploratory Data Analysis (EDA)
- **Univariate Analysis**:
  - Visualizations (like histograms) were created to observe distributions of variables such as loan amount, income, and interest rates.
  - Default rates were analyzed to understand the imbalance in the target variable.
- **Bivariate Analysis**:
  - Relationships between loan status and features like credit score or income were studied through plots.
  - Correlation matrices identified significant relationships among numerical features.

### 4. Feature Engineering
- New features, such as debt-to-income ratio and credit utilization rate, were calculated to better represent risk factors.
- Categorical variables were encoded into numerical values using appropriate encoding techniques.

### 5. Model Building
- Multiple machine learning models were trained to predict credit risk. Logistic Regression and ensemble models like Random Forest were tested.
- Hyperparameter tuning was performed to optimize model performance.

### 6. Model Evaluation
- Metrics such as accuracy, precision, recall, F1 score, and ROC-AUC were calculated to evaluate the performance of the models.
- Confusion matrices were used to analyze true positive and false negative rates, especially for imbalanced datasets.

---

## 🔍 Observations

### Dataset Characteristics
- A significant number of missing values were found in columns related to employment history and other borrower characteristics.
- Outliers were prominent in variables like loan amounts and annual income, suggesting diverse borrower profiles.

### Default Patterns
- Borrowers with lower credit scores exhibited higher default rates.
- High debt-to-income ratios were strongly correlated with defaults.

### Feature Importance
- Credit scores, loan amounts, and interest rates emerged as key predictors of credit risk.
- Newly engineered features, like debt-to-income ratio, significantly improved model accuracy.

### Model Results
- Logistic Regression provided a good baseline with moderate accuracy.
- Ensemble models like Random Forest and XGBoost outperformed simpler models, achieving higher precision and recall.

---

## 💡 Insights

### Creditworthiness Indicators
- Borrowers with credit scores below a certain threshold are more likely to default. Adjusting credit score thresholds can reduce default risks.

### Loan Structuring
- Loans with high interest rates and longer durations are more prone to defaults. Structuring loans with balanced rates and durations can mitigate risks.

### Borrower Profiles
- Borrowers with stable employment histories and lower debt-to-income ratios are safer to lend to.

### Risk Management
- Implementing a dynamic risk scoring system based on the derived model can enhance loan approval processes.
