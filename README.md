# Banking/Financial Transaction Database Generator

This repository contains the Python script used to generate a large-scale, synthetic dataset modeling banking and financial transactions.

The project demonstrates relational database design (3NF) and the creation of realistic data, including intentional inconsistencies for data cleaning exercises.

## Project Details

* **Script:** `Financial_db_generator_24093896.ipynb` (Python 3)
* **Database Output:** `Financial_Transaction_DB.sqlite`
* **Core Tables:** 4 tables (`Branches`, `Customers`, `Accounts`, `Transactions`)
* **Data Volume:** Over **50,000** transaction records generated.
* **Key Design:** Uses a composite key (`CustomerID`, `Currency`) in the `Accounts` table and ensures referential integrity across all tables.

## Data Realism Features

The synthetic data includes deliberate modeling of real-world imperfections:
* **Data Voids:** Approximately 3% of transaction descriptions are `NULL`.
* **Inconsistencies:** Approximately 1% of transactions are duplicated to simulate system errors.

## Requirements

* Python 3.x
* The `sqlite3` library (standard in Python)
* The `faker` library

## How to Run
1.  **Install Faker:** Run `!pip install faker`.
2.  **Execute:** Run all cells in the Google Collab Notebook (`Financial_db_generator_24093896.ipynb`).

The script will create and populate the database file (`Financial_Transaction_DB.sqlite`) in the same directory.
