# Business Performance and Customer Insights Dashboard using Power BI and SQL

This dashboard, built using Power BI and powered by SQL databases, offers comprehensive insights into sales performance, customer behavior, and user acquisition trends, leveraging advanced analytics and forecasting to support data-driven business decisions.

## Table of Contents

- [Project Overview](#project-overview)
- [Objectives](#objectives)
- [Dataset Citation](#dataset-citation)
- [Project Structure](#project-structure)
- [Tools and Technologies](#tools-and-technologies)
- [Implementation Steps](#implementation-steps)
- [Usage](#usage)
- [Dashboard Components](#dashboard-components)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

This dashboard, developed in Power BI and fueled by SQL databases, integrates detailed user interaction data from a Kaggle dataset to provide actionable insights into sales performance, customer behavior, and user acquisition. Through predictive modeling and visual analytics, the dashboard supports key business objectives, including sales growth, customer retention, and more effective marketing strategies. The analysis helps enhance user experience and engagement by informing data-driven decisions in product development and targeted marketing efforts.

## Objectives

- Integrate and analyze detailed business performance and user interaction data from the Kaggle dataset.
- Develop and maintain dynamic visualizations in Power BI to reflect comprehensive user engagement metrics.
- Use SQL and Power BI to automate the reporting process, enhancing operational efficiency.
- Implement predictive models to forecast customer behaviours and key business outcomes.

## Dataset citation

Shriyash Jagtap. (2023). E-commerce Customer for Behavior Analysis [Data set]. Kaggle. https://www.kaggle.com/datasets/shriyashjagtap/e-commerce-customer-for-behavior-analysis?resource=download

## Project Structure

```plaintext
Power_BI_Dashboard/
├── dashboards/
│   ├── BP_CI_dashboard.pbix                 # Main Power BI dashboard file
│   ├── BP_CI_dashboard.pdf                  # Exported version of the dashboard in PDF format
├── data/
│   ├── ecommerce_customer_data_large.csv    # Raw Kaggle dataset for ecommerce customer analysis
│   ├── cleaned_ecommerce_customer_data_with_metrics.csv  # Cleaned dataset after preprocessing and feature engineering
│   ├── sql_database.csv                     # Data extracted from SQL database used in the analysis
├── results/
│   ├── clv_distribution.png                 # Distribution plot of Customer Lifetime Value (CLV) 
│   ├── clv_residuals.png                    # Residuals plot for CLV prediction model evaluation
│   ├── feature_importance_churn.png         # Bar chart showing the most important features driving churn prediction
│   ├── predictions.csv                      # CSV file containing model predictions for both churn and CLV
├── scripts/
│   ├── extract_data.py                      # Python script for data cleaning, preparation, and metrics calculation
│   ├── predictive_modeling.py               # Python script for churn and CLV predictive modeling and evaluation
│   ├── transform_data.sql                   # SQL script for data extraction and transformation
├── README.md                                # Project README with instructions and overview of the dashboard
├── LICENSE.md                               # License information for the project
```

## Tools and Technologies
- **SQL**: For data querying, manipulation, and efficient storage of large datasets, enabling faster and more scalable analysis.
- **Power BI**: For creating interactive and automated dashboards.
- **Python**: For scripting data extraction, processing tasks, and predictive modelling.
- **Anaconda**: A distribution that includes Python, Spyder, Jupyter Notebooks, and other data science tools, providing a comprehensive environment for data analysis and modeling.
- **DB Browser for SQLite**: A high-quality, open-source tool to create, design, and edit database files compatible with SQLite.
- **SQLite ODBC Driver**: A driver that allows Power BI to connect directly to SQLite databases, enabling efficient data retrieval for dashboards.

## Implementation Steps

1. **Data Access Setup**: Download the Kaggle dataset on user behaviours.
2. **Data Extraction and Transformation**: Use Python scripts to transform and prepare data for analysis.
3. **Metric Calculation**: Compute key metrics such as Customer Lifetime Value (CLV), Churn Rate, and Conversion Rate.
4. **Data Transformation to SQL**: The processed data is transformed and stored in an SQL database. This step leverages SQL's strengths for efficient data querying, storage, and integration with Power BI. 
5. **Dashboard Development**: Design and develop dynamic dashboards in Power BI.
6. **Predictive Modeling**: Implement predictive models to forecast customer churn and lifetime value in Python scripts.

## Usage

## Usage

1. **Data Preprocessing**:
   The dataset `ecommerce_customer_data_large.csv` from Kaggle is imported and cleaned using the `extract_data.py` script. Key metrics such as Customer Lifetime Value (CLV) and Churn Rate are calculated. The cleaned data is saved as `cleaned_ecommerce_customer_data_with_metrics.csv`.

2. **Model Predictions**:
   Run `predictive_modeling.py` to train and evaluate predictive models for churn and CLV. The script saves outputs such as predictions and evaluation plots (e.g., feature importance, residuals) to the `results/` folder.

3. **SQL Database Integration**:
   Import the predictions (`predictions.csv`) and cleaned dataset into a SQL database. The `transform_data.sql` script prepares the columns and structures the database for proper usage in Power BI.

4. **Power BI Dashboard**:
   Open `BP_CI_dashboard.pbix` in Power BI. The dashboard uses the SQL database and cleaned CSV data to generate visual insights on sales, churn prediction, and customer segmentation.

## Dashboard Components

- **Main Analysis Report**: Total sales, sales indicators, forecasting, gender distribution, customer segmentation by age, churn prediction, and CLV prediction.
- **Other Analytics**: Average sales and CLV by product category, total sales by payment method, and customer purchase frequency.
- **User Acquisition Analysis**: Growth over time by gender and product category.


## Contributing

Guidelines for contributing to the project, including how to propose changes, submit patches, and report issues.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.


