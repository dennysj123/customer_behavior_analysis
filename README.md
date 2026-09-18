customer_behavior_analysis
data analytics project showcasing customer behavior analysis using python, SQL, and power BI

Data Analytics Project

 Overview

This project demonstrates an end-to-end **data analytics workflow**, starting from raw data preparation in Python and progressing through exploratory data analysis, data cleaning, SQL analysis using PostgreSQL, and visualization using Power BI.

The project also includes a detailed analytical report and a presentation created using Gamma to communicate key findings and business insights.

The main objective is to transform raw customer data into **meaningful insights that can support data-driven business decisions**.

---

 Dataset

The project uses a customer purchase dataset containing information related to:

* Customer demographics
* Product and category details
* Purchase amount
* Location
* Size and color
* Season
* Review ratings
* Subscription status
* Shipping type
* Discounts and promotional codes
* Previous purchases
* Payment method
* Purchase frequency

The dataset was initially loaded and processed using Python before being imported into PostgreSQL for SQL-based analysis.

---

Tools & Technologies

| Tool                 | Purpose                                |
| -------------------- | -------------------------------------- |
| Python               | Data loading, preprocessing and EDA    |
| Pandas               | Data manipulation and cleaning         |
| Jupyter Notebook     | Python-based analysis                  |
| PostgreSQL           | Database storage and SQL analysis      |
| pgAdmin 4            | PostgreSQL database management         |
| SQL                  | Data analysis and business queries     |
| Power BI             | Dashboard and data visualization       |
| Gamma                | Presentation creation                  |
| Microsoft Excel      | Supporting data analysis/documentation |

---

Project Workflow

text
Raw Dataset
     ↓
Load Data using Python
     ↓
Exploratory Data Analysis (EDA)
     ↓
Data Cleaning & Preprocessing
     ↓
Load Clean Data into PostgreSQL
     ↓
SQL Queries & Business Analysis
     ↓
Power BI Dashboard
     ↓
Analytical Report
     ↓
Gamma Presentation
```

---

Project Steps

 1. Load Dataset in Python

The dataset was imported into Python using Pandas.

Initial checks were performed to understand:

* Dataset dimensions
* Column names
* Data types
* Missing values
* Duplicate records
* Unique values
* Basic statistical information

2. Exploratory Data Analysis

EDA was performed to identify patterns and understand customer purchasing behaviour.

The analysis included:

* Descriptive statistics
* Distribution analysis
* Customer segmentation
* Purchase behaviour analysis
* Category-level analysis
* Frequency analysis
* Identification of potential data quality issues

3. Data Cleaning

The dataset was cleaned and prepared for further analysis.

Key preprocessing activities included:

* Handling missing values
* Checking duplicate records
* Correcting column names
* Standardizing categorical values
* Converting columns into appropriate data types
* Creating calculated columns
* Creating purchase-frequency-related variables
* Preparing the dataset for database analysis

4. PostgreSQL & SQL Analysis

The cleaned dataset was loaded into a **PostgreSQL database**.

SQL queries were then used to answer business-related questions such as:

* Which customer segments generate the most revenue?
* What is the average purchase amount?
* Which product categories perform better?
* How does purchasing behaviour vary by customer demographics?
* What is the relationship between discounts and purchase behaviour?
* How do subscription customers compare with non-subscribers?
* Which customer groups show repeat-purchase behaviour?

SQL aggregation functions, filtering, grouping, sorting, conditional logic, and subqueries were used for analysis.

5. Power BI Dashboard

The analyzed data was connected to Power BI to create an interactive dashboard.

The dashboard focuses on key business metrics and customer purchasing patterns.

Possible KPIs and visualizations include:

* Total Revenue
* Total Customers
* Average Purchase Amount
* Customer Segments
* Purchase Frequency
* Revenue by Category
* Revenue by Gender
* Revenue by Location
* Subscription Status
* Discount Usage
* Customer Purchase Behaviour

The dashboard allows users to explore the data using interactive filters and visualizations.

6. Analytical Report

A detailed report was prepared to document:

* Project background
* Business problem
* Objectives
* Data preparation
* Analysis methodology
* SQL analysis
* Key findings
* Business insights
* Recommendations
* Conclusion

### 7. Presentation

A professional presentation was created using Gamma to communicate the project findings in a concise and visually engaging format.

The presentation covers:

* Project overview
* Dataset
* Methodology
* Key analysis
* Dashboard
* Major insights
* Business recommendations
* Conclusion

---

 Dashboard

The Power BI dashboard provides an interactive view of customer purchasing behaviour.

 Key Dashboard Areas

Customer Analysis

* Customer demographics
* Customer segments
* Previous purchases
* Purchase frequency

Sales Analysis

* Total revenue
* Average purchase value
* Revenue by category
* Revenue by location

Marketing Analysis

* Discount usage
* Promo code usage
* Subscription status

Behavioural Analysis

* Purchase frequency
* Product preferences
* Customer retention indicators

> Add your Power BI dashboard screenshot here.

```markdown
![Power BI Dashboard](images/powerbi-dashboard.png)
```

---

## 📈 Results

The project converts raw customer transaction data into actionable business insights through a complete analytics pipeline.

Key outcomes include:

* Identified customer purchasing patterns.
* Segmented customers based on previous purchase behaviour.
* Analyzed revenue and purchase trends using SQL.
* Identified differences across customer demographics and product categories.
* Examined the impact of discounts, promotions and subscriptions.
* Developed an interactive Power BI dashboard for business reporting.
* Created a structured analytical report and presentation.

The project demonstrates how Python, SQL, and Power BI can be combined to support data-driven decision-making.

---

How to Run

Prerequisites

Install the required Python libraries:

bash
pip install pandas sqlalchemy psycopg2-binary matplotlib seaborn
```

You will also need:

* Python 3.x
* Jupyter Notebook
* PostgreSQL
* pgAdmin 4
* Power BI Desktop

### Step 1: Clone the Repository

```bash
git clone https://github.com/yourusername/data-analytics-project.git
cd data-analytics-project
```

### Step 2: Load the Dataset

Place the dataset inside the project directory.

Example:

```text
data/
└── customer.csv
```

### Step 3: Run Python Analysis

Open the Jupyter Notebook:

```bash
jupyter notebook
```

Run the notebook to:

1. Load the dataset
2. Perform EDA
3. Clean the data
4. Create required columns
5. Prepare the final dataset

### Step 4: Connect to PostgreSQL

Create a PostgreSQL database and configure the connection in Python.

Example:

```python
from sqlalchemy import create_engine

engine = create_engine(
    "postgresql+psycopg2://username:password@localhost:5432/database_name"
)
```

Load the cleaned dataset into PostgreSQL:

```python
dataset.to_sql(
    "customer",
    engine,
    if_exists="replace",
    index=False
)
```

 Step 5: Run SQL Queries

Open pgAdmin 4, connect to the PostgreSQL database, and execute the SQL queries provided in the `sql/` folder.

 Step 6: Open Power BI Dashboard

Open the Power BI `.pbix` file using Power BI Desktop.

If required, update the PostgreSQL connection details and refresh the data.


Project Structure

text
Data-Analytics-Project/
│
├── data/
│   └── customer.csv
│
├── notebooks/
│   └── data_analysis.ipynb
│
├── sql/
│   └── analysis_queries.sql
│
├── powerbi/
│   └── customer_dashboard.pbix
│
├── report/
│   └── data_analytics_report.pdf
│
├── presentation/
│   └── project_presentation.pdf
│
├── images/
│   └── powerbi-dashboard.png
│
└── README.md


 Skills Demonstrated

* Python
* Pandas
* Exploratory Data Analysis
* Data Cleaning
* Data Preprocessing
* SQL
* PostgreSQL
* pgAdmin
* Data Visualization
* Power BI
* Business Intelligence
* Customer Analytics
* Data Interpretation
* Business Reporting
* Presentation Development

 Conclusion

This project demonstrates an end-to-end approach to **data analytics**, from raw dataset preparation to business intelligence and reporting.

By combining Python for data preparation, PostgreSQL for structured analysis, and Power BI for visualization**, the project showcases practical skills required for an entry-level Data Analyst / Business Analyst role.

