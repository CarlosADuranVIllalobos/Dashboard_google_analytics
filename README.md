# Business Performance and Customer Insights Dashboard using Power BI and SQL

This dashboard, built using Power BI and powered by SQL databases, offers comprehensive insights into sales performance, customer behavior, and user acquisition trends, leveraging advanced analytics and forecasting to support data-driven business decisions.

## Table of Contents

- [Project Overview](#project-overview)
- [Objectives](#objectives)
- [Dataset Citation](#dataset-citation)
- [Tools and Technologies](#tools-and-technologies)
- [Implementation Steps](#implementation-steps)
- [Usage](#usage)
- [Dashboard Components](#dashboard-components)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The dashboard integrates detailed user interaction data from the Kaggle dataset to provide insights into app usage patterns, marketing effectiveness, and user engagement strategies. This analysis supports the organization's goals to enhance user experience and engagement through targeted marketing and app functionality improvements.

## Objectives

- Integrate and analyze detailed user interaction data from the Kaggle dataset.
- Develop and maintain dynamic visualizations in Power BI to reflect comprehensive user engagement metrics.
- Use SQL and Power BI to automate the reporting process, enhancing operational efficiency.
- Implement predictive models to forecast customer behaviors and key business outcomes.

## Dataset citation

Shriyash Jagtap. (2023). E-commerce Customer for Behavior Analysis [Data set]. Kaggle. https://www.kaggle.com/datasets/shriyashjagtap/e-commerce-customer-for-behavior-analysis?resource=download


## Tools and Technologies
- **SQL**: For data querying, manipulation, and efficient storage of large datasets, enabling faster and more scalable analysis.
- **Power BI**: For creating interactive and automated dashboards.
- **Python**: For scripting data extraction, processing tasks, and predictive modeling.
- **Anaconda**: A distribution that includes Python, Spyder, Jupyter Notebooks, and other data science tools, providing a comprehensive environment for data analysis and modeling.
- **DB Browser for SQLite**: A high-quality, open-source tool to create, design, and edit database files compatible with SQLite.
- **SQLite ODBC Driver**: A driver that allows Power BI to connect directly to SQLite databases, enabling efficient data retrieval for dashboards.

## Implementation Steps

1. **Data Access Setup**: Download the Kaggle dataset on user behaviors.
2. **Data Extraction and Transformation**: Use Python scripts to transform and prepare data for analysis.
3. **Metric Calculation**: Compute key metrics such as Customer Lifetime Value (CLV), Churn Rate, and Conversion Rate.
4. **Data Transformation to SQL**: The processed data is transformed and stored in an SQL database. This step leverages SQL's strengths for efficient data querying, storage, and integration with Power BI. 
5. **Dashboard Development**: Design and develop dynamic dashboards in Power BI.
6. **Predictive Modeling**: Implement predictive models to forecast customer churn and lifetime value.

## Usage

Instructions on how to access and interact with the dashboards, including how to perform custom analyses and interpret the data provided.

## Dashboard Components

- **Main Analysis Report**: Total sales, sales indicators, forecasting, gender distribution, customer segmentation by age, churn prediction, and CLV prediction.
- **Other Analytics**: Average sales and CLV by product category, total sales by payment method, and customer purchase frequency.
- **User Acquisition Analysis**: Growth over time by gender and product category.


## Contributing

Guidelines for contributing to the project, including how to propose changes, submit patches, and report issues.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.

## Project File Structure

User_Engagement_Analytics_Dashboard/
├── data/
│   ├── ecommerce_customer_data_custom_ratios.csv        # Dataset from Kaggle
│   ├── ecommerce_customer_data_large.csv        # Dataset from Kaggle
├── notebooks/
│   ├── dashboard_visualization.ipynb # Power BI visualization setup
│   ├── predictive_modeling.ipynb     # Jupyter notebook for predictive modeling
├── scripts/
│   ├── data_preparation.py           # Script for data cleaning and preparation
│   ├── metric_calculation.py         # Script for calculating key metrics
│   ├── predictive_modeling.py        # Script for predictive modeling
│   ├── transform_data.sql            # SQL scripts for data manipulation
├── dashboards/
│   ├── user_engagement_dashboard.pbix# Main Power BI dashboard file
├── README.md                         # Project README with instructions
├── LICENSE.md                        # License information
