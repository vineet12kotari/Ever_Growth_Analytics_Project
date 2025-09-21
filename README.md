# 📂 Ever Growth Data Pipeline: A Power BI Data Engineering Project

A data consolidation and transformation project built to showcase end-to-end data pipeline skills using Power BI. This project focuses on connecting to diverse data sources, performing complex transformations, and building a robust data model for a global sales and distribution company, Ever Growth Enterprises.

## 📜 Short Description / Purpose

This project addresses the real-world challenge of scattered and inconsistent data storage by demonstrating a data engineering solution using Power BI. It focuses on the crucial first steps of a business intelligence project: **data loading**, **transformation**, and **modeling**, which lay the groundwork for any future analytical reports or dashboards.

---

## 🛠️ Tech Stack

This project leverages a powerful suite of tools to handle the entire data preparation workflow:

* **📊 Power BI Desktop** – The central platform used for all data ingestion, transformation, and modeling.
* **📂 Power Query** – Utilized extensively for its capabilities in connecting to multiple data sources (folders, JSON, CSV) and performing a wide range of data cleaning and shaping tasks.
* **❄️ Snowflake** – A cloud data warehouse used to simulate a modern data storage environment, showcasing skills in connecting to and importing data from a cloud-based source.
* **📝 Data Modeling** – The project's core, where relationships were established between a variety of tables to create a star schema, enabling efficient data analysis.
* **🐍 Python (Optional/Future Work)** – The potential for using Python scripts for more complex data cleaning or automation could be a future enhancement.

---

## 📋 Data Sources & Project Flow

The project workflow simulates a common business scenario where data resides in various locations and formats:

1.  **Sellers Data:** Loaded from a local folder, demonstrating the ability to handle multiple files at once.
2.  **Flat Files:** Connections were established to CSV files (**Customers**, **Orders**, **Geolocation**) and a JSON file (**Products**), highlighting proficiency with different file types.
3.  **Snowflake Database:** Data was first loaded into Snowflake tables (**Order Payments**, **Order Items**, **Product Categories**, **Order Reviews**) and then imported into Power BI. This step demonstrates familiarity with cloud data warehousing and data ingestion from a central repository.

---

## ⚙️ Key Transformations & Data Modeling

This section highlights the specific data preparation skills demonstrated in the project:

* **Data Loading from Diverse Sources:** The project successfully ingested data from **folders**, **JSON**, **CSV**, and **Snowflake**, showcasing a versatile skill set.
* **Data Cleaning & Manipulation:**
    * Replaced blank values in the `Review comment title` column with "Review not given."
    * Reduced the decimal values in the `PAYMENT_INSTALLMENTS` and `PAYMENTS_VALUE` columns.
* **Date Dimension Creation:** New columns (`Month`, `Year`, `Name of the Month`, `Quarter of the Year`) were derived from the `shipping_LIMIT_DATA` column, a key step in creating a time-intelligence-ready data model.
* **Data Modeling:** The project's highlight is the creation of a well-structured data model, with relationships established between all the tables. A notepad listing the **primary keys** from each table was also created to document the data model's schema.

---

## 📁 Dataset Location

To make this project reproducible, all data and SQL scripts are included in the repository. The folder structure is as follows:
/Ever_Growth_Analytics_Project
├── .gitignore
├── README.md
├── Ever_Growth_Analytics.pbix
└── Data/
├── Sellers Data/
│   ├── seller_1.csv
│   └── seller_2.csv
│   └── ...
├── Flat Files/
│   ├── JSON File/
│   │   └── products_data.json
│   └── CSV Files/
│       ├── customers_data.csv
│       ├── orders_data.csv
│       └── geolocation_data.csv
└── SQL/
├── create_tables.sql
└── load_data.sql
