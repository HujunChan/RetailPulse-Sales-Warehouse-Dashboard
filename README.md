# RetailPulse — Sales Warehouse & KPI Dashboard

**RetailPulse** is a beginner-friendly data engineering project that demonstrates a complete end-to-end ETL workflow. It processes raw retail data to generate actionable insights through a centralized warehouse and interactive dashboard.

##  Overview

This project simulates a real-world data pipeline:

1. **Extracts** raw sales data from CSV files.
2. **Transforms** and cleans the data using Python.
3. **Loads** the structured data into a PostgreSQL warehouse.
4. **Analyzes** key metrics using SQL.
5. **Visualizes** performance trends in Power BI.

##  Tech Stack

* **Language:** Python (Pandas)
* **Database:** PostgreSQL
* **Querying:** SQL
* **Visualization:** Microsoft Power BI

##  ETL Workflow

The data flows through the pipeline in the following stages:

1. **Extract:** Ingest raw data from local CSV files.
2. **Transform:** Clean data, handle missing values, and format types using Pandas.
3. **Load:** Insert processed records into the PostgreSQL database.
4. **Analyze:** Generate KPI calculations directly within the database using SQL.
5. **Visualize:** Connect Power BI to PostgreSQL to build the dashboard.

##  Key Performance Indicators (KPIs)

The dashboard focuses on tracking the following core metrics:

* **Total Sales:** Gross revenue generated.
* **Total Orders:** Count of distinct transactions.
* **Total Customers:** Unique customer count.
* **Average Order Value (AOV):** Mean revenue per transaction.
* **Sales by Category & Region:** Performance breakdown by dimension.
* **Monthly Sales Trend:** Time-series analysis of revenue.

##  How to Run

### Prerequisites

* Python 3.8+
* PostgreSQL installed and running locally
* Power BI Desktop

### Steps

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/retailpulse.git
cd retailpulse

```


2. **Install dependencies**
```bash
pip install -r requirements.txt

```


3. **Configure Database**
Update the `config.py` file with your PostgreSQL credentials:
```python
DB_HOST = "localhost"
DB_NAME = "retail_db"
DB_USER = "your_user"
DB_PASS = "your_password"

```


4. **Run the ETL Pipeline**
Execute the script to clean and load data:
```bash
python etl.py

```


5. **Launch Dashboard**
* Open Power BI Desktop.
* Select **Get Data** > **PostgreSQL Database**.
* Connect to your local database and load the tables.
* Open the `.pbix` file included in this repo (if applicable) or build visuals using the imported data.



