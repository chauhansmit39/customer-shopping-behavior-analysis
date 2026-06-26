## 🚀 How to Run the Project

### Prerequisites

Make sure the following software is installed on your system:

* Python 3.10 or later
* Jupyter Notebook or JupyterLab
* PostgreSQL
* pgAdmin 4
* Power BI Desktop
* Git (optional)

---

## 1. Clone the Repository

```bash
git clone https://github.com/chauhansmit39/customer-shopping-behavior-analysis.git

cd customer-shopping-behavior-analysis
```

---

## 2. Install Required Python Libraries

Install all required packages using:

```bash
pip install -r requirements.txt
```

Or install them manually:

```bash
pip install pandas numpy sqlalchemy psycopg2 jupyter
```

---

## 3. Run the Data Cleaning Notebook

Open Jupyter Notebook or JupyterLab:

```bash
jupyter lab
```

or

```bash
jupyter notebook
```

Open:

```
Python/Customer_Shopping_Behavior_Analysis.ipynb
```

Run all cells from top to bottom to:

* Load the raw dataset
* Explore the data
* Remove duplicate records
* Handle missing values
* Standardize column names
* Perform feature engineering
* Create the cleaned dataset
* Load the cleaned data into PostgreSQL

---

## 4. Configure PostgreSQL

Open **pgAdmin 4** and:

1. Create a new PostgreSQL database.
2. Update the PostgreSQL connection details in the Jupyter Notebook.

Example:

```python
database = "customer_db"
user = "postgres"
password = "your_password"
host = "localhost"
port = "5432"
```

Run the notebook again to load the cleaned dataset into PostgreSQL.

---

## 5. Execute SQL Queries

Open:

```
SQL/customer_behavior_sql_queries.sql
```

Run the SQL script in **pgAdmin 4** to perform the business analysis.

The SQL queries answer business questions such as:

* Revenue by Gender
* Top Rated Products
* Customer Segmentation
* Revenue by Age Group
* Shipping Type Analysis
* Subscription Analysis
* Top Products by Category
* Discount Analysis

---

## 6. Open the Power BI Dashboard

Open the Power BI project:

```
Dashboard/Customer_Shopping_Dashboard.pbix
```

If prompted, reconnect the report to the PostgreSQL database or the cleaned dataset.

Refresh the data to view the latest results.

---

## 7. Explore the Dashboard

The interactive dashboard includes:

* KPI Cards

  * Total Customers
  * Average Purchase Amount
  * Average Review Rating

* Interactive Filters

  * Subscription Status
  * Gender
  * Category
  * Shipping Type

* Visualizations

  * Revenue by Category
  * Sales by Category
  * Subscription Distribution
  * Revenue by Age Group
  * Sales by Age Group

---

## Project Workflow

```
Raw CSV Dataset
        │
        ▼
Python (Pandas)
Data Cleaning & Feature Engineering
        │
        ▼
PostgreSQL
Database Creation & SQL Analysis
        │
        ▼
Power BI
Dashboard & Business Insights
```
