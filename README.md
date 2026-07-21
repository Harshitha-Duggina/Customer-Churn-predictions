# Customer Churn Prediction 

An end-to-end Machine Learning and Data Analytics project designed to identify high-risk churn customers for a telecommunications company. This project spans from raw data ingestion and structural data cleaning to building, optimizing, and comparing multiple predictive AI models.

## 📊 Business Problem & Insights
Customer churn occurs when a subscriber stops doing business with a service provider. Through Exploratory Data Analysis (EDA), this project uncovered the primary business drivers behind customer loss:
* **High Monthly Charges:** Customers with higher billing rates show a significantly higher propensity to leave.
* **Contract Types:** Month-to-month subscribers represent the highest churn risk compared to long-term contracts.
* **Low Tenure:** New customers are highly volatile and require immediate engagement strategies.


## 🛠️ Tech Stack & Workflow

* **Data Wrangling & Cleaning:** `pandas`, `numpy`
  * Handled string-to-numeric data type conversions for problematic fields like `TotalCharges`.
  * Processed and patched structurally missing data values.
* **Data Visualization:** `matplotlib`, `seaborn`
  * Created multi-variable distribution plots tracking Churn vs. Tenure and Monthly Spend.
* **Machine Learning Pipelines:** `scikit-learn`, `xgboost`
  * Split data into controlled stratified training and validation sets using `train_test_split`.
  * Developed a comparative pipeline to train and evaluate multiple classification algorithms.


## 📈 Model Performance Leaderboard

To ensure maximum predictive reliability, multiple classification models were evaluated using standard industry metrics. We focused heavily on **Recall** (the ability to catch actual churners) alongside **Accuracy** and **ROC-AUC** (overall separation capability):

| Classification Model | Accuracy | Recall | ROC-AUC |
| :--- | :--- | :--- | :--- |
| **Logistic Regression** | 80.41% | 52.55% | 0.8497 |
| **Random Forest** | 76.58% | 46.92% | 0.7976 |
| **XGBoost** | 80.34% | 50.13% | 0.8445 |

### 🔍 Strategic Takeaway
While **Accuracy** gives us a general baseline, **Recall** is our primary business metric. A high Recall score ensures the company catches the maximum number of true churners, allowing the marketing team to step in with retention offers before the customer leaves.


## 🚀 How to Run the Project

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Harshitha-Duggina/Customer-Churn-predictions.git](https://github.com/Harshitha-Duggina/Customer-Churn-predictions.git)
2.  **Open in VS Code:**
   Launch VS Code,open the project folder,and open the notebook file:customer churn project.ipynb
3.  **Run the notebook:**
   Ensure your Python environment has the required packages installed:
       pip install pandas matplotlib seaborn scikit-learn xgboost

Select 'Run All' in your Jupyter notebook to execute the entire analytics and modeling pipeline.
