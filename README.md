# Retail Sales Performance Analysis and Revenue Prediction Using Machine Learning

## Project Overview

This project focuses on analyzing retail sales data to identify revenue trends, understand product category performance, and explore daily revenue prediction using machine learning.

The project demonstrates a complete data analytics workflow, including data inspection, validation, exploratory data analysis (EDA), visualization, model training, and evaluation.

**Internship:** IBM SkillsBuild Data Analytics with AI Academic Internship Program  
**Author:** Alen Aby  
**Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Jupyter Notebook, VS Code

## Objectives

- Inspect and validate retail transaction data.
- Perform data cleaning and preprocessing.
- Analyze revenue trends across dates and product categories.
- Explore customer purchasing patterns.
- Build and compare regression models for daily revenue prediction.
- Evaluate model performance using MAE, RMSE, and R².
- Present findings through visualizations and a project report.

## Dataset Description

The dataset contains 1,000 retail transactions and nine columns:

| Column | Description |
|---|---|
| Transaction ID | Unique transaction identifier |
| Date | Transaction date |
| Customer ID | Customer identifier |
| Gender | Customer gender |
| Age | Customer age |
| Product Category | Category of the purchased product |
| Quantity | Number of units purchased |
| Price per Unit | Price per unit |
| Total Amount | Total transaction amount |

The dataset is used to analyze revenue patterns and customer purchasing behavior.

**Note:** Include the original dataset in the repository only if its license and sharing permissions allow redistribution. Otherwise, provide the dataset source and instructions for obtaining it.

## Technologies Used

- **Python** — Data analysis and model development
- **Pandas** — Data manipulation and preprocessing
- **NumPy** — Numerical computation
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualizations
- **Scikit-learn** — Machine learning and model evaluation
- **Jupyter Notebook** — Interactive analysis
- **Visual Studio Code** — Development environment

## Project Workflow

### 1. Data Inspection and Validation

- Examined dataset dimensions and column types.
- Checked for missing values and duplicate records.
- Validated transaction dates and numerical fields.
- Checked consistency between quantity, unit price, and total amount.

### 2. Data Cleaning and Preprocessing

- Standardized column names and categorical values.
- Converted date and numerical columns to appropriate data types.
- Removed exact duplicate rows where applicable.
- Prepared the dataset for exploratory analysis.

### 3. Exploratory Data Analysis

The project explores revenue patterns using the following visualizations:

- Monthly revenue trend
- Revenue by product category
- Revenue by customer gender
- Customer age distribution

### 4. Revenue Prediction

Daily transaction revenue is aggregated into a time series. Calendar features and historical revenue features are used to explore prediction.

The following models are compared:

- Mean-prediction baseline
- Linear Regression
- Random Forest Regressor

### 5. Model Evaluation

Model performance is evaluated using:

- **MAE:** Mean Absolute Error
- **RMSE:** Root Mean Squared Error
- **R²:** Coefficient of Determination

The data is split chronologically to evaluate predictions on a later period. Model performance must be interpreted relative to the baseline and the limitations of the available historical data.

## Project Structure

```text
Retail_Revenue_Project/
│
├── retail_revenue_analysis.ipynb
├── requirements.txt
├── README.md
├── AlenAby_ProjectReport.docx
│
├── data/
│   └── retail_sales_dataset.csv
│
└── outputs/
    ├── 01_monthly_revenue.png
    ├── 02_category_revenue.png
    ├── 03_gender_revenue.png
    ├── 04_customer_age_distribution.png
    ├── 05_actual_vs_predicted_revenue.png
    ├── model_evaluation_results.csv
    └── revenue_predictions.csv
```

*The dataset and generated output files should be included only when appropriate for sharing.*

## Installation and Setup

### Prerequisites

- Python installed on your system
- Git
- Visual Studio Code
- Python and Jupyter extensions for VS Code

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/retail-sales-revenue-prediction.git
cd retail-sales-revenue-prediction
```

Replace `YOUR-USERNAME` with your GitHub username.

### Step 2: Create a Virtual Environment

```bash
python -m venv .venv
```

On Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

### Step 3: Install Dependencies

```bash
python -m pip install -r requirements.txt
```

### Step 4: Configure the Dataset

Place `retail_sales_dataset.csv` in the `data/` folder. If the dataset is not included in the repository, obtain it from the source documented by the project owner.

### Step 5: Run the Notebook

Open `retail_revenue_analysis.ipynb` in VS Code, select the `.venv` Python interpreter as the notebook kernel, and execute the cells in order.

## Outputs

The project generates visualizations, model evaluation results, and test-period predictions in the `outputs/` directory. A Word report summarizes the methodology, findings, model metrics, and limitations.

## Limitations

- The dataset covers a limited historical period.
- The data may not represent every transaction or every day of business activity.
- Dates without recorded transactions should not automatically be treated as zero-revenue days without verifying data completeness.
- Predictive performance depends on the data, feature choices, and evaluation period.
- Results are exploratory and require further validation before use in business decisions.

## Conclusion

This project demonstrates the application of Python-based data analytics and introductory machine learning to a retail sales use case. It combines data validation, exploratory analysis, visual storytelling, and regression model evaluation to investigate revenue behavior and assess the feasibility of predicting daily revenue.

## Acknowledgements

Prepared as part of the IBM SkillsBuild Data Analytics with AI Academic Internship Program.

---

**Author:** Alen Aby  
**Project:** Retail Sales Performance Analysis and Revenue Prediction Using Machine Learning
