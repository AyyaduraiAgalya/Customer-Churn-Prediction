# Customer-Churn-Prediction (On-going)
This project predicts customer churn for a telecommunications company using a full machine learning pipeline. It demonstrates a range of essential data science skills: data preprocessing, feature engineering, model building with hyperparameter tuning, and model interpretability with SHAP.

## Dataset
- **Source**: [Telco Customer Churn Dataset on Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Features**: Includes demographic, account, and service details such as `tenure`, `MonthlyCharges`, `TotalCharges`, `Contract`, and `PaymentMethod`.
- **Target**: `Churn` (Yes/No), indicating whether the customer left the service.

## Initial Data Exploration and Analysis

### Exploratory Data Analysis (EDA)
- **Target Variable**: Examined the distribution of `Churn` to identify any class imbalance.
- **Numerical Features**:
  - **Tenure**: High churn rate among customers with short tenure, with some long-term loyal customers.
  - **Monthly Charges**: Bimodal distribution suggesting different service or pricing tiers.
  - **Total Charges**: Right-skewed distribution, indicating many customers with lower cumulative charges, possibly due to short tenure or low monthly plans.
- **Categorical Analysis**:
  - **Contract Type**: Month-to-month contracts have significantly higher churn compared to one-year or two-year contracts.
  - **Payment Method**: Higher churn rate among customers using Electronic check as their payment method, while automatic payment methods (bank transfer, credit card) correlate with lower churn.

### Key Findings
- Customers on month-to-month contracts and those paying via Electronic check are more likely to churn.
- High churn among new customers and those with low total charges suggests that retention strategies should focus on engaging newer customers and incentivizing longer contracts.

## Skills Demonstrated
- Data Wrangling and Exploration
- Exploratory Data Analysis (EDA) and Visualization
- Business Insight Generation from Data

## Project Setup
1. **Clone the Repository**:
   ```bash
   git clone <repository_url>
    ```
## Install Dependencies
Ensure you have Python 3.6+ and install required libraries:

```bash
pip install -r requirements.txt
```
## Run the Jupyter Notebook
Open `notebooks/1_data_exploration_and_preprocessing.ipynb` to view the analysis and findings:

```bash
jupyter notebook notebooks/1_data_exploration_and_preprocessing.ipynb
```
## Repository Structure
- `notebooks/`: Jupyter notebooks for exploration and analysis.
- `data/`: Placeholder for dataset (note: dataset is not uploaded to GitHub).
- `README.md`: Project documentation and overview.
- `requirements.txt`: List of dependencies required to run the project.
